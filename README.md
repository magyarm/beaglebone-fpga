beaglebone-fpga
===============

My attempt at making an FPGA add-on cape for the Beaglebone.

2012/10/22

Now that midterms are done, I'm back to development.They ate up all my time the last 3-4 weeks, but now I'm back to the world of the living. The big changes this time 'round are cmpletely changing the power supply from two dual rail Linear Technology LTC 3546 switching regulators to 3 Texas Instruments TPS6213x. Two reasons for this change. 1) is a ~14$ reduction in BOM cost. The Linear Tech chips were expensive. 2) Now with only 3 voltage rails, and no jumper to choose voltage for the IO Banks the routing and layout will be a lot simplier, and a lot less messy. This was a strong recommendation that I redo the stack up and internal layout by my manufacturer, so this is working towards that.

I also fell victim to a bit of scope creep this week. I moved the 20 IO pins from Bank_1 to Bank_0. Now Bank_0 has all 40 of them. Onto Bank_1 I have now added 32MB of SDRAM assigned to the Spartan 6's Memory Controller Block interfaces. Adding external RAM was something I had idially considered, but didn't do due to laziness, but figured I'd do it now. It was on my original features list, but I thought I'd do it on a later revision, now I'm thinking I want to try to get everything I want on this first revision for testing. Hoping, I'll have less revision over all this way.

The current battle plan is to due the layout in the next week or so, including the remaining changes the manufacturer suggested (still 8 pages or so of them...).  With the largest chunk of my midterms over, I will hopefully have the time to commit to this again.


2012/09/24

Finding an affording manufacturer has been difficult, due in large part 
to weird thigns with my board design. Thankfully, I have found a great 
one that is working with me to clean up my design. After reviewing my 
design, they have submitted a list of improvements I should make. I am 
currently working my way down that list. I expect it will take most of 
this week. Then, it's off again to see if its ok, and whether it's 
affordable to build.

2012/09/10
Right now the schematics in this repository are not correct. I had 
(still have) mostly poor revision control/backup discipline and lost a 
couple weeks worth of work on the schematics. Thankfully, the netlist 
and pcb design were untouched, and are included here. 

Right now I am shopping around to have this made. It has been reviewed 
by a few people, and I'm mostly confident it will work. 
