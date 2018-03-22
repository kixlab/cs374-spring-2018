# 04-Learnability Part 2



# Admin (4:02, 10m)
- nanoquiz: link on the board? N1-201 doesn't have good board space.
- For activities, links should stay on the slide.

- Design Project info
- Thermostat exercise follow-up


# UI HOFS: RealCD (4:12, 7m)

## RealCD home view
IBM’s RealCD is CD player software, which allows you to play an audio CD in your CD-ROM drive.
Why is it called “Real”?  Because its designers based it on a real-world object: a plastic CD case.  This interface has a metaphor, an analogue in the real world.  Metaphors are one way to make an interface more learnable, since users can make guesses about how it will work based on what they already know about the interface’s metaphor. Unfortunately, the designers’ careful adherence to this metaphor produced some remarkable effects, none of them good.

Here’s how RealCD looks when it first starts up.  Notice that the UI is dominated by artwork, just like the outside of a CD case is dominated by the cover art.  That big RealCD logo is just that – static artwork.  Clicking on it does nothing.
There’s an obvious problem with the choice of metaphor, of course: a CD case doesn’t actually play CDs. The designers had to find a place for the player controls – which, remember, serve the primary task of the interface – so they arrayed them vertically along the case hinge.  The metaphor is dictating control layout, against all other considerations.
Slavish adherence to the metaphor also drove the designers to disregard all consistency with other desktop applications.  Where is this window’s close box?  How do I shut it down?  You might be able to guess, but is it obvious?  Learnability comes from more than just metaphor.


- How is a metaphor used here?
- Player uses a CD case, not a CD player as a metaphor. why is this problematic?
- What's tricky about metaphors is that sometimes it's not clear to what extent the interface follows the rules of the original object.
- What would you hope to do with a real CD case?
- One of the metaphors: It's a CD case so you can open it. How do you open it?
- Why use green light to turn off the interface?

## Opened view

But it gets worse.  It turns out, like a CD case, this interface can also be opened.  Oddly, the designers failed to sensibly implement their metaphor here.  Clicking on the cover art would be a perfectly sensible way to open the case, and not hard to discover once you get frustrated and start clicking everywhere.  Instead, it turns out the only way to open the case is by a toggle button control (the button with two little gray squares on it).
Opening the case reveals some important controls, including the list of tracks on the CD, a volume control, and buttons for random or looping play.  Evidently the metaphor dictated that the track list belongs on the “back” of the case.  But why is the cover art more important than these controls?  A task analysis would clearly show that adjusting the volume or picking a particular track matters more than viewing the cover art.
And again, the designers ignore consistency with other desktop applications.  It turns out that not all the tracks on the CD are visible in the list.  Could you tell right away?  Where is its scrollbar?


- Playmode options: disabled buttons
- Volume: shift up and down, not left and right as shortcut
- What other information did it lose with this "creative" scrollbar? Where you are.
     - scrolls one track at a time. not paginated!
- Green dots: disable a track. Somewhat consistent with the power off button.

- Bullets to the right of track names: reordering control
- Track names are editable
- Help book: when you open it, now the interface has three sides open.

## Mouse over

We’re not done yet.  Where is the online help for this interface?
First, the CD case must be open.  You had to figure out how to do that yourself, without help.
With the case open, if you move the mouse over the lower right corner of the cover art, around the IBM logo, you’ll see some feedback.  The corner of the page will seem to peel back.  Clicking on that corner will open the Help Browser.
The aspect of the metaphor in play here is the liner notes included in a CD case.  Removing the liner notes booklet from a physical CD case is indeed a fiddly operation, and alas, the designers of RealCD have managed to replicate that part of the experience pretty accurately.  But in a physical CD case, the liner notes usually contain lyrics or credits or goofy pictures of the band, which aren’t at all important to the primary task of playing the music.  RealCD puts the instructions in this invisible, nearly unreachable, and probably undiscoverable booklet.
This example has several lessons: first, that interface metaphors can be horribly misused; and second, that the presence of a metaphor does not at all guarantee an “intuitive”, or easy-to-learn, user interface.  (There’s a third lesson too, unrelated to metaphor – that beautiful graphic design doesn’t equal usability, and that graphic designers can be just as blind to usability problems as programmers can.)
Fortunately, metaphor is not the only way to achieve learnability.  In fact, it’s probably the hardest way, fraught with the most pitfalls for the designer. In this lecture, we’ll look at some other ways.


- What makes it so hard to learn?
- They are professional designers. They must have thought this was a great idea. What do you think that idea was?
- Hope: transfer real-world knowledge into a computer representation.


# Nanoquiz (1:19, 4m)


# Consistency and Metaphor 

## Metaphor (4:23, 3m)
Amazon's Kindle e-book reader

- What is the metaphor here? Physical book
- How does this metaphor break down? How is it enhanced?
- How is it better than a physical book? How is it worse?
- What kinds of affordances are there?

- desktop: very successful, everyone knows it, now it's not really a metaphor anymore.

- for metaphors that are outdated, what do we do? e.g., call icon, floppy disk icon, even camera icon


## Skeuomorphism (4:26, 3m)
- form of metaphor
- pros: good learnability, familiarity, visually pleasing
- cons: too much unnecessary visual detail, awkward, metaphor breaks at some point anyway

## Activity: Kinetic Scrolling (4:30, 7m)

Law of physics in interfaces: motion and touching

- consistency between real-world vs GUI experience
- gaining popularity with touch devices and skeuomorphism
- swiping behavior in a touch device: natural deceleration
- discuss other physics-inspired interface widgets

## Design Guidelines & External Consistency (4:37, 3m)

- Material design by google
- style guides by many big product companies
- why?
- across various products within and across the entire ecosystem
- Efforts to maintain consistency across multiple apps


# Affordance

## Examples (1:40, 5m)
1) Hello, computer (Star Trek 4): http://youtu.be/LkqiDu1BQXY?t=1m4s
THERE’S that memorable scene in 1986’s Star Trek IV: The Voyage Home where the crew of the starship Enterprise has travelled back in time from the 23rd to the 20th century. Chief Engineer Scotty (James Doohan) attempts to use a Macintosh.
 
Facing the screen, he speaks to it (of course): “Computer? … Computer!”
 
His crewmate Dr ‘Bones’ McCoy (DeForest Kelley) looks as puzzled as him, then notices the mouse, which he hands over to Scotty. Scotty goes, “Ah!”, then speaks into the mouse, “Hello, computer.”
 
It doesn’t work. The 20th century engineer they’re trying to impress says, “Just use the keyboard” to which Scotty responds, “Keyboard. How quaint.” 

2) Baby swiping a magazine like a book: https://www.youtube.com/watch?v=aXV-yaFmQNk

- knowledge in the world is different
- learned to interact with touchscreen devices before interacting with paper books.
- Implication: keep in mind your target users. They are not you. What "you" believe to be consistent, good feedback, and metaphors might just not work.
- What's our solution then? Learn from users. Observe them. Talk to them. Watch them. Ask them. Pilot test with them. More in upcoming user-centered design and prototyping classes.




# Video Break (4:45, 10m)
Draco (CHI 2014)

- learnability: complex animation parameter setting is made easy with immediate feedback and direct manipulation.


# Feedback


## Case study: web browser status bar (4:55, 3m)

Status bar in a web browser as a case study

- Too far from the actual link: not a good job of providing useful feedback about the ramification of an action. Poor learnability
- Do we really need progress bars when page loading is fast enough with fast internet connection? But how long is long? We need to understand human perception and capabilities.

JavaScript progress bar
- sometimes in conflict with the browser progress bar?
- what do they actually show progress of? sometimes works like scrollbar, other times loading bar.


## Activity: Unix Shell (4:58, 10m)

Unix may be beautiful for many reasons, but learnability is not one of them.

- The actions available to the user are completely invisible; the user must recall a command name from memory, along with the syntax for its arguments.

- The state of the underlying system is likewise mostly hidden.  Many users customize their prompts to make some state visible, such as the current directory or the hostname.  The contents of the current directory are not visible, even though many commands operate on files.

- The feedback from a command is minimal – in fact, one Unix design principle is that commands should say nothing when they succeed.  But that’s not a good thing.  It’s true that a generic feedback message like “command completed successfully” would indeed be useless; the subsequent appearance of a command prompt is sufficient feedback that the command has completed.  So what kind of visible feedback would be useful?

- show my custom shell prompt with syntax highlighting and custom shell: in what way does this help and not?



# Information Scent

## Activity: How does Google try to improve information scent? (5:08, 5m)

Try searching for different information types




===

# Diff with Reading
- removed perceptual fusion & response time: moved to human capabilities
- locus of attention: moved to human capabilities


# Post Class Notes
- students really liked Draco 
- db.vu doesn't support keyboard input on mobile / tablet.

===

# Unused
Here's a quick exercise. Consider the lights in your room. Design a panel of light switches to control the room's lights, for installation next to one of the entrance doors. Devise a natural mapping between your switch panel and the lights it controls, so that a user can easily learn and remember how to use it. Don't stop with just one design, but sketch out a few.

A few things to think about:

1. It may not make sense to control every light individually. How should the lights be grouped?
2. Think about consistency. Will your panel be recognizable as light switches from across the room? On the other hand, are there better choices than the standard North American flip switches?
3. If you use flip switches, how should they be oriented?



## Activity: Play with Affordances (1:37, 7m)

Here's an exercise that you can try with your favorite webpage. It's a chunk of Javascript that changes all the text on the page to X's, so that all you can see is what the page is telling you nonverbally, using affordances. (It doesn't affect text that's rendered in an image, unfortunately, so this has the interesting side effect of discovering pages with poor accessibility and poor internationalization.)

Do an actual demo: One way to use it is to open your browser's Javascript console and just paste the code in; it will change the current page. 

Another way to use it is to create a new bookmark in your browser, and use as the URL javascript: followed by the code given above. Clicking on this bookmark will run the Javascript on the current page. (This is called a bookmarklet, and it's an one way to modify web pages you don't own.)