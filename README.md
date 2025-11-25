# BLY

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

