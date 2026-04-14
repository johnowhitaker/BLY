# BLY

## Update: Biliverdin v2

The pre-transformed one I streaked out isn't looking very green, tragically. Also, after checking and checking, I re-did the order and forgot to click away from the default vector. Luckily I had a tiny bit of ampicillin left, so could make a few plates, but still - lame. Trying a more iron-rich media and attempting a transform into BL21 soon in case it is just this cloning strain not expressing much protein, we shall see.....

## Update: Biliverdin diffusion

I got the first biliverdin one, and the colonies themselves didn't really show much color, but the agar itself did - as feared the biliverdin is likely diffusing out. Bottom plate has a streak expressing this:

<img width="1086" height="505" alt="image" src="https://github.com/user-attachments/assets/677d1a5e-bd84-425a-a195-d7a0c1f40d80" />

Anyway, on to the final attempt: using a protein from tree frogs to hopefully bind the biliverdin and keep it in place. Notebook has the deisgn for v2. I also went for a high-copy plasmid. Risky bet but hopefully we get enough expression to show some actual color!


## Update: Biliverdin

I got the first plasmid and transformed it into e. c. but it had very low expression. Eventually some blue color was visible (aeBlue) but only after a long time at room temp.

As a new attempt, I looked at other sources of green coloration in nature, settling on producing biliverdin. ~~New plasmids ordered, wish me luck.~~ EDIT: order cancelled, since my business address is a residential address.

I have now ordered it from GenScript, in their [pET-24a(+)](https://www.genscript.com/vector/detail?vector_name=cEVULTI0YSglMkIp&refer=gensmart) vector.  I set the 5' RE to EcoRI and the 3' to NotI. $198 inc ~50 shipping and 10 for glycerol stock as an add-on. The T7 promoter shouldn't do anything in the strains I plan on using. Wish me luck :) 

## Old stuff

Attempting my first ever plasmid design.

## The Plan

I want a visible-light green to complement the [set of chromoproteins](https://atinygreencell.com/products/rainbow-chromoprotein-expression-plasmid-set) I've bought. The plan is as follows:

- Practise some sterile technique on some basic experiments
- Get a gene transformation kit (I've ordered one from Carolina bio) that is made to let students transform bacteria. This will 1) serve as practice with a known-good plasmid and 2) fill a few small gaps in what I have on hand for doing transformations
- Attempt a transformation with the plasmid described in this repo
- If it works and it looks cool, share it around!
- Make some dope agar art

## Progress

I came up with what I thought was a clever idea, but alas I made a mistake that means it probably wouldn't work. A pity - I really like the thought if it. `attempt_1_flawed` hides the evidence.

The more sensible route is to set up a seq that includes a yellow protein and a blue one, and hope that they mix to for an OK green. BLYv2_easy builds up the cassette. It's essentially: J23106 promoter → RBS (B0030) → fwYellow → RBS (B0030) → aeBlue → B1006 terminator (plus some spacers). `_green` is one dumb idea for a fun modification that I decided to do ;)

The cassette gets placed into GenScript's pUC57-Kan vector. Here it is annotated:

<img width="823" height="829" alt="image" src="https://github.com/user-attachments/assets/0f2c0e36-4708-4cdf-9b69-df08a8ea629b" />

Casette details:

```
Component                      Start    End      Length  
------------------------------------------------------------
Promoter J23106                0        35       35      
Spacer 1                       35       46       11      
RBS B0030 (fwYellow)           46       58       12      
RBS spacer                     58       64       6       
fwYellow (modified) CDS        64       796      732     
Intergenic spacer              796      804      8       
RBS B0030 (aeBlue)             804      816      12      
RBS spacer                     816      822      6       
aeBlue CDS                     822      1518     696     
Terminator B1006               1518     1557     39      

Total cassette length: 1557 bp
```


## Current Status

Plasmid is in production. About to receive a transformation kit. Might have growing colonies by Christmas.

