---
title: "Character Level RNN"
layout: single-portfolio
excerpt: "Trained an RNN on State of the Union Adresses to predict sentences given a few letters."
collection: projects
diplay_order: 2
header: 
    og_image: ""
---
For this project, I used [Karpathy's char RNN model](http://karpathy.github.io/2015/05/21/rnn-effectiveness/) which is trained on character sequence probabilities.

The jupyter notebook with this code can be found [here](https://github.com/curtiscjohnson/deep-learning/blob/main/Char-RNN.ipynb).

I first trained on the Lord of the Rings text, but then trained on my own dataset. I chose to use the State of the Union addresses from 1790-2019 as my corpus.  

The RNN picked up on important words like "United States" and "economy". It is also interesting that lots of the longer formal words that are compound words are mixed up -- like "intercation", "effectment", or "presentional". There are still some weird characters floating around and random numbers. The RNN also picked up on punctuation decently. Capital letters generally come after periods, but not after commas or quotations.

Here are some results! The first two letters are the input, and the sequence that follows are the outputs. 

> wh
> which bether but its former of the interminity interest and for they cher not herise the loOge the caused and value of Xxagy the economy of .ure resist of the fund by our elication is refendments by at 
>
> ra
> ray and the praged to consilies that this labor that the bost has hope breach the a aimiture.', zendor have furnectors are the enforce of the States the 6ther [+fitly and us the stear of its educy of th 
>
> he
> here and not enount it a vanic considerative for suple.',y Xreed in the our enacted provision and friend met to its bost has relification for thrang the last in#ur and country and commandast in such is  
>
> Th
> The bread of pay of the long.', "at this entired and inend in the righter proves and securing |urred housing, exill this brouse not be are some has Korethen and of our achoopication resourcensiomed that 
>
> lo
> local pro/urds. Its adriplic \nfor+ther }here not the property. It interests addecity to affect the country effectment in the him presentional been sates of the purposed that it are inspection of <evote 
>
> ra
> ray of the not inmlease of a conduction of persons to this it able of those communignted the considerations in the publy for the submitted have bean 9, our the peace depends, have liWe the provides of t 
>
> ra
> ratures, this from this still our suggeaustisulations and sinst fthat responsices vrimor, than the great against intercation of our dains and it affidy great to the interment should pace of upon the dis 
>
> lo
> lo	' centroy and a longers are increase of the has to at discredurent, body of the Sesvation, and of preats on the States for the right other out is in the national states in the purpose the bord to str 
>
> he
> here to be the and our proper the relations, and the inrade in oning for the finst several as mone dugient of the last in day to messure become and the Interestly or the mune the great be repartments to 
>
> I 
> I necessary bubusing the United States in 9 the ralion progotion and and improver.', "$Ge/her on the aL its be progress to the dair to incomes from the inflicts of the progress of the commerce made by b 