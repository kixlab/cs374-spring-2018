# 09-Human Abilities

# Recap

- This week we'll talk about human cognition, and start a series of implementation classes.

# Admin

# UI HOFS (4:03, 7 mins)
Scrollbars

On the left is Ghostview, a Unix program that displays Postscript files. Ghostview has no scrollbars; instead, it scrolls by direct manipulation of the page image.  Clicking and dragging on the page scrolls it around, and it turns out that dragging downward moves the page image upward.  That is, when you drag the mouse down, more of the page image come into view at the bottom of the window.  Does this make sense?  What mental model, or physical analogy, does this correspond to?
On the right is Acrobat, which displays PDF files.  Acrobat has scrollbars, but you can also directly manipulate the page image, as in Ghostview – only now clicking and dragging downward moves the page downward, revealing more page image at the top of the window.  What mental model does this correspond to?

What if you used both Acrobat and Ghostview frequently (one for PDF, say, and the other for Postscript)?
The Ghostview model is like a glass window that you’re dragging around on top of the page.  You’re pressing on the glass and pushing it to the left should indeed make more of the page become visible on the left.  
The Acrobat model treats the window like an empty frame, and you’re actually reaching through and pushing the page itself around.  Pushing it to the left should make more of the page visible on the right. 
So two different physical analogies are possible here.  Principles of direct manipulation alone don’t help us decide.  And Ghostview at least uses a consistent model –the light gray rectangle in the leftside toolbar (underneath the Save Marked button) is a miniature representation of the position of the glass window over the page, and you push it around using the same dragging direction that you use on the page image itself.
If you had to use both Acrobat and Ghostview frequently, however, the inconsistency between them would be very painful.  Yet we do have to use *both* models these days: direct-touch scrolling (smartphones and tablets) uses one model, and scrollbars and mouse scrollwheels use the opposite model.  The directness vs. indirectness of the interaction and differences in the low-level muscle interaction may give enough cues to keep the model straight.  But touchpads on laptops may be the hardest point of overlap, since they are indirect, and yet use the same finger swiping motion as direct touch.  Apple decided to make a significant transition recently with Mac OS X Lion, switching its default touchpad scrolling from one mental model (the scrollwheel) to the other (direct touch).

## Xerox Star, Mac

Let’s look at scrolling some more.  Scrollbars have evolved considerably over the history of graphical user interfaces.

The Xerox Star offered the earliest incarnation of a graphical user interface, and its scrollbar already had many of the features we recognize in modern scrollbars, such as a track containing a scrollbar thumb (the handle that you can drag up and down). Even its arrow buttons do the same thing – e.g., pushing on the top button makes more of the page appear at the top of the window, just like the modern scrollbar.  But they’re labeled the opposite way – the top button has a down arrow on it.  Why is that?  What mental model would lead you to call that button down?  Is that consistent with the mental model of the scrollbar thumb?

Another interesting difference between the Star scrollbar and modern scrollbars are the - and + buttons, which move by whole pages. This functionality hasn’t been eliminated from the modern scrollbar; instead, the modern scrollbar just drops the obvious affordance for it. You can still click on the track above or below the thumb in order to jump by whole pages.  
The button labels actually refer to the page-pushing model of scrolling – when you click on the top button, the page itself moves down.  Alas, this is completely inconsistent with the thumb, which uses the glass-pane model of scrolling – the thumb represents the glass pane, and you can drag it up and down the document.  So the Xerox Star scrollbar couldn’t make up its mind about which model to represent.

Removing the +/- buttons makes the scrollbar simpler, by forcing the track to do double-duty.  But it also makes the page-jumping functionality less visible, so new users are unlikely to discover it on their own.
We can also say something about natural mapping here – the arrow buttons are on opposite sides of the scrollbar, so their positions map appropriately to the direction that they move the thumb.  (But, alas, the Xerox Star’s arrow labels disagree with the natural mapping.)
Another improvement in the scrollbar is that the height of the thumb now indicates what fraction of the whole document is visible.

## Flash Scrollbar

Here’s another example of a Flash scrollbar that lacks clear affordances (from http://www.bcg.com/join_bcg/interview_prep/interactive_case/default.aspx).  It turns out that the bright, highly salient part of this scrollbar is NOT the thumb, but the track!  The thumb is a dark color – in fact, it’s the same dark color that’s used as a background color of some of the widgets on the right (Used and Remaining).  (example suggested by Eryn Maynard)





# Nanoquiz (4:10, 3 mins)



# MHP / Distributed Cognition (4:15)

## Math: Motivation for Representation (4:15, 3 mins)
Engaging start, worked quite well.

Intermediate "variable" tracking was mentioned as a reason for the slowed performance in the memory group.

## Tetris: Epistemic Action (4:18, 5 mins)
Asked students to guess experts vs novices, which would exhibit more epistemic actions. Many got the answer wrong.

But the explanation was a bit too long. Make it concise and to the point.

Tetris: people move blocks more than they need to. Experts rely more heavily on moving objects in the world. Cheaper to do it in the world than to mentally rotate them.


## Getting things done & Brainstorming (4:23, 1 min)
=> write it down, empty your working memory, move on


# Video Break (4:25, 7 mins)
inFORM
https://www.youtube.com/watch?v=ouP9xNujkNo

TransFORM
https://www.youtube.com/watch?v=lCARHatJQJA
Play the first 2 minutes

- Ask students how distributed cognition was applied to physical objects, helping remote collaboration and externalization of ideas.

# Power of Representation (4:32)

Representation dramatically affects our problem solving ability.


## Oranges and Bagels

Had volunteers and come out and solve.

Two reasons the bagels version is easier.

- The physical property of "stacking" bagels makes the rule easier to understand and apply. Reasoning task => transferred to a perceptual task of visually verifying.
- Also, it resembles the tower of Hanoi game, which many of us are familiar with.

## Card Game and Tic-Tac-Toe

Had volunteers play different versions.

Tic-Tac-Toe takes significantly shorter time, and ta-da, these games are actually isomorphic!

https://en.wikipedia.org/wiki/Tic-tac-toe

Herb Simon
- math proof: true also at the beginning. What has changed is the fact that the proof is true is rendered clear to the reader.

Why is it hard?
Embed the constraints of the problem in the UI: offload working memory, so that limited resources become available.

Naturalness principle
- experiential cognition is aided when the properties of the representation match the properties of the thing that's represented.


## Subway Map Examples

London underground map
- what physical property is preserved?
- what task does it support well? what task does it fail to support well?
- context + overview (suberbs are sparse)
- "As a schematic diagram, it does not show the geographic locations but rather the relative positions of the stations, lines, the stations' connective relations, and fare zones."

slow reasoning task => fast perceptual task



# Chunking
Need better explanation on the activity: what does the command do, and what is the partition % for?

===

# Diff with Reading


# Post Class Notes
Add GOMS?

Time-wise the full 75 mins were spent, even without the UI HOFS.

- the oranges game took much longer than I expected, but with the easier game version it should be faster next time.

- Distributed congnition: look at Chapter 3 of "Interaction Design"

- Zhang & Norman reading: add some of the content into the reading and video eventually.

## Distributed Cognition Notes from Scott
when interfaces help people distribute congnition, it can
- encourage experimentation (Tetris)
- scaffold learning and reduce errors (Montessouri blocks)
- Show differences that matter (London Underground)
- Convert slow calculation into fast perception (Map coloring)
- Support chunking, especially by experts (Chess & gestures)
	- moving text from A to B: copy A, move to B, paste A
- increase efficiency (diagrams)
- facilitate collaboration (cockpits)
	- artifacts help pilots coordinate action
	- speed dial
	- 
## Locus of attention

Locus of attention is important, because as a UI designer, we can leverage this to direct people's attention in a meaningful way. If there's important information you want to display, it'd be useful to make sure they are in the locus of attention. Status bar is a bad example indeed.



## EXAMPLE: iPhone selection zoom

- because the finger obscures feedback, it shows a zoomed in view of the current text being selected.
- dual purpose: provide visual feedback and help with precise selection
- fat finger problem: fingers occlude information and prevent precise actions when using touch devices.
     - clearly user's goal is not met due to design issues.
     - what are some ways you can fix that?

Attention is tricky in that it handles only one channel at a time,
but yet it's so easy to shift that channel when external stimuli are available.


	
## Case Study: active reading 
- what are the common tasks in reading?
- what are some of the cognitively challenging tasks a reader experiences?
	- highlighting, keeping track of various interesting parts, going back and forth between the body and ref, etc.
- LiquidText: https://www.youtube.com/watch?v=gpA_bGUm3Wo

- Not sure if I want to keep this. Fun app, but not sure the take-home message is clear enough.
