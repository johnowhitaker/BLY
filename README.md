# BLY

## Attention! The current design is flawed :) 

I'd checked through, asked a council of AI's for opinions (Sonnet 4.5, GPT-5.1-Thinking and Gemini 3 Pro), chatted to a friend about it, stewed over it... I was happy with the plan, I'd even submitted the order. Then, lying awake on a Sunday night, I went for one final sanity check and asked Gemini to list anything that could lower the chance of success, and while thinking away it hit on something I'd completely missed at the start... aeBlue is a **tetramer**! In other words, the piece I was working with was one of four subunits that group together to do their thing, and tacking on fwYellow would likely mess that up and result in a clumpy mess. There's still a chance it could work out, but I managed to halt the order and will change gears and shift to a plasmid design that makes the two pieces separately within an operon. Phew!

## (Old stuff, ignore until I get organised)

Attempting to make a green protein! I've designed and ordered a plasmid for it. This repo has my process, the relevant DNA bits, and will house results once I get it and try to get it into something living :)

<img width="925" height="834" alt="image" src="https://github.com/user-attachments/assets/2890887a-9025-4512-87d5-4c4df2c5c769" />

The notebook ('BLY_Designing_The_Plasmid.ipynb') documents the construction of a casette containing the core protein sequence (which consists of aeBlue and fwYellow proteins joined with a flexible linker) along with a promoter, terminator, RBS and some other bits. This casette goes in a GenScript pUC57-kan flash gene vector (pictured above) - but I included NcoI and SacI sites so that hopefully interested parties could snip it out and pop it into their vector of choice? (TBH these were a last-minute addition).

I've added the files from GenScript ('Fasta_Final U700D316G0.txt' and '2_bly_op2_p06_pUC57-Kan.gb') as well as an annotated version of the latter ('BLY_pUC57-Kan_Annotated.dna', pictured above) from snapgene.

<img width="650" height="389" alt="image" src="https://github.com/user-attachments/assets/12609124-fec6-46fd-8dac-67556118ee0e" />

You can check out the predicted structure on alphafold [here](https://alphafoldserver.com/fold/193dd24a4e8a80bc)

## The Plan

I want a visible-light green to complement the [set of chromoproteins](https://atinygreencell.com/products/rainbow-chromoprotein-expression-plasmid-set) I've bought. The plan is as follows:

- Practise some sterile technique on some basic experiments
- Get a gene transformation kit (I've ordered one from Carolina bio) that is made to let students transform bacteria. This will 1) serve as practice with a known-good polasmid and 2) fill a few small gaps in what I have on hand for doing transformations
- Attempt a transformation with the plasmid described in this repo
- If it works and it looks cool, share it around!
- Make some dope agar art

I included some specific bits that should allow others to cut out just the protein's DNA with two 'sticky ends' so that it can be transferred to different vectors as well, without having to pay again for it to be printed. This isn't something I'll do, but maybe someone else will :)

## Potential Pitfalls

If you really wanted to dial in a green based on a blue protein and a yellow protein, you would probably set up a design with two separate promoters so that you could tweak the expression levels individually. Instead, I've opted to make this fusion, which prevents tweaking the ratios and might mess up the colors of one or both barrels. This is *cool* (the main motivation), and also I don't have the budget to try lots of variants anyway. If you wanted to, you could first spend some time with a version that let you moderate expression levels without changing the genes and figure out from there what mix looks best.

I've also been a little naive on the codon optimization side. For the aeBlue seq, I went with the wild-type gene (derived from Actinia equina) - it is known to express in E. coli, but there are better-optimized variants around I'm sure. For fwYellow I chose the most common codon for each AA in E. coli - again, possibly not the best approach. (I also then made a couple of substitutions to avoid accidental NcoI sites). There's method to the madness here too though - I have a friend playing with codon optimization, if I have this "unoptimized" naive version, maybe in the future we can make an 'optimized' one and compare.

There's a risk I just consistently mess up the actual transformation. I ordered the pasmid in 8 aliquots, and each tube of liquid will have enough DNA for a number of attempts, so I'll get a few tries. But I'm a noob in a messy basement, there are *so* many ways to screw this part up!

And finally, the big risk is that I don't know what I'm doing at all, and as a result I've made some foundational mistake that will doom this whole enterprise :)
