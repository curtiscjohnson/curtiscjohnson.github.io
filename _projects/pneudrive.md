---
title: "PneuDrive: Embedded Pressure Control"
layout: single-portfolio
excerpt: "An embedded pressure control system I designed for low-level control of pneumatic robots. <br/><br/><img src='/images/PneuDrive_Boards.png'>"
collection: projects
---

Most existing pressure control systems on the markers are either too small in terms of flow rates, or too bulky in terms of size. I designed PneuDrive to fit a few key requirements:

1. **Large Scale**  
   - Regulate pressures of up to 80 psi  
   - Provide high-flow rates with proportional flow valves

2. **Distributed Control**  
   - Control at least 12 valve/chamber pairs  
   - Minimize wiring and tubing over distances of about one meter

3. **Expandable**  
   - Capability to incorporate additional sensors (e.g., IMUs) for future work

4. **Easy to Use**  
   - Use low-cost, off-the-shelf components that are easy to replace  
   - Open-source software that is customizable

5. **Communication**  
   - Easy connection to other devices with low latency  
   - Reliable communication for real-time control loops

PneuDrive works by daisy-chaining multiple board together on a robust RS485 communication bus. 

![daisy-chain](/images/DaisyChainDiagram.png "daisy-chain")

Each board has a microcontroller that reads pressure sensors and controls proportional flow valves. 

The accompanying C++ library is easy to use via ROS or with Python bindings:

```python
import numpy as np
from pneudrive_py import PressureController

uart_port = '/dev/ttyS1'
num_devices = 4
my_controller = PressureController(uart_port, num_devices)

#check communication with all expected devices
my_controller.ping_devices()

pressure_cmd = np.array([1,2,3,4])
for i in range(num_devices):
    my_controller.set_pressure_commands(i, pressure_cmd)
    data = my_controller.get_pressure_data(i)
```

For more info, check out the publication pages [here](/_publications/pneudrive.md).