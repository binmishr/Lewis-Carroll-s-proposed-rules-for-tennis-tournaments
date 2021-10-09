# Lewis-Carroll-s-proposed-rules-for-tennis-tournaments-by-ellis2013nz



A Brief Introduction
=====================

Seeding is one way to increase the chance of the top players making it to the final rounds of a single elimination tournament, leading to fairer outcomes and to a higher chance of the best matchups happening in the finals. Basically it’s to overcome this problem:

    “At a Lawn Tennis Tournament, where I chanced, some while ago, to be a spectator, the present method of assigning prizes was brought to my notice by the lamentations of one of the Players, who had been beaten (and had thus lost all chance of a prize) early in the contest, and who had had the mortification of seeing the 2nd prize carried off by a Player whom he knew to be quite inferior to himself.”

Charles Dodgson (Lewis Carroll)
==================================
The incident related above led nineteenth century Oxford University mathematician Charles Dodgson to propose an alternative to the unseeded single elimination tournament that was standard at the time. His monograph on the subject, LAWN TENNIS TOURNAMENTS: The True Method of Assigning Prizes with a Proof of the Fallacy of the Present Method, can be found from page 1,082 of his complete works. Of course, Dodgson’s side hustle was as part time children’s author Lewis Carroll, of works including the astonishingly good Alice’s Adventures in Wonderland, Through the Looking Glass and The Hunting of the Snark; and the deservedly forgotton Sylvie and Bruno.

Here are the basic elements of Dodgson’s proposed system, which he describes for a tournament of 32 male players:

    1.“A list is kept, and against each name is entered, at the end of each contest, the name of any one who has been superior to him – whether by actually beating him, or by beating some one who has done so (thus, if A beats B, and B beats C, A and B are both ‘superiors’ of C). So soon as any name has 3 ‘superiors’ entered against it, it is struck out of the list”
    2.“only one contest that (first) day – the 32 Players being arranged in 16 pairs”
    3.“For the 2nd day … the 16 unbeaten men are paired together, and similarly the 16 with 1 superior (the Losers in these last-named pairs will now have 3 superiors each, and will therefore be struck off the list). In all other contests they are paired in the same way; first pairing the unbeaten, then those with 1 superior, and so on, and avoiding, as far as possible, pairing two Players who have a common superior.”
    4.“By the middle of the 3rd day the unbeaten are reduced to two… These two … have a whole-day match on the 4th day…”
    5.“By the end of the 4th day, the ‘First-prize-man’ is known (by the very same process of elimination used in the existing method): and the remaining Players are paired by the same rules as before, for the 2 contests on the 5th day.”

The essence of the method is that no-one is knocked out until they are definitely not one of the three best players, as proven by having three or more “superiors” who have either beaten them in a match or beaten someone who beat them. By this method, the actual top three bubble to the top of the competition.

One interesting observation is that under Dodgson’s rules there is no requirement to have the number of players a power of two, as is the case in a standard single-elimination tournament if the organisers wish to avoid unbalanced byes.

Dodgson argues that his proposed method is guaranteed to allocate the first, second and third prizes accurately to the best three players in order. However, his monograph makes some key assumptions:

    1.superiority is transitive eg if A is superior to B and B to C, then A is superior to C
    2.superiority is deterministic, consistent and persistent

Obviously, the real world isn’t like this. How does his method stand up when we make the results of individual matches uncertain and inconsistent with eachother in line with the realistic Elo-based simulation of results I used last week?

To check this out, I simulated Dodgson-style tournaments with the same 128 top women players from 1990 that I used last week with more conventional tournaments. I built the program to do this so the user had a choice in how individual matchups between players resulted – either deterministically (higher rated player is guaranteed to win, as per Dodgson’s own 32 player demonstration) or realistically probabilistically (chances are random but still depend on the Elo ratings of the two players).
