####Draft

### Dinosaurs

Scott Hanselman: Alright, now we're recording. OK. David Sokol, tell me about Fortran.

David Sokol: Fortran is an interesting programming language simply because it's one of the
oldest programming languages that's still in use today besides assembly.

Rob Conery: Okay, wait a minute. I have to step in here. What is that music? And Fortran?
Excuse me? What have you done to my podcast? What, I mean, our podcast, sorry.

SH: I was going to say, our podcast. Well, this week I wanted to spend a little time being
a little more creative so it's my editing and my musical selection because you were
sleeping.

RC: You call that music? I think you just used the term 'music'. What is that? It sounds
like a pocket calculator.

SH: Well because this week's episode is called 'Dinosaurs', and because we are talking
about older things, I wanted to bring in some older music. So we've got some interesting
70's remixes, we've got some MIDI, and some SID chip music from commodore 64s. It might
be a little bit jarring, but this is what we were listening to in the 80's when we were
in the computer world.

RC: It's true, It's true. So I heard the guy say something about Fortran. Who is he, and
why is he doing Fortran?

SH: We've got three really interesting stories on This Developer's Life this week.
David Sokol is a young developer who actually went straight out of college into a job
writing Fortran.

RC: You're kidding me.

SH: Exactly. This is a living language with a lot of people using it, and this story is
about his journey as a .NET developer to first a begrudging respect, and then an actual
respect for Fortran.

RC: My goodness.

SH: And then a little later, we have someone also using an old language, Sean Bamforth,
who is using DataFlex. Not a living language, in fact a totally dead language that he has
no business using.

*Unknown* : I've never even heard of it, I don't even know what it is!

SH: Well tragically it's a language he's given 15 years of his life to, and we'll find out
what Sean Bamforth did with that 15 years and how he feels about it. Then finally to
wrap the show up we've got our very own Pete Brown who years and years later insists on
making music with commodore 64 and is now ripping SID chips out of commodore 64s and
hooking them up to actual PCs. So we've sprinkled commodore 64 music throughout.

*Unknown*: Oh boy.

RC: You know this is teaching me not to go on vacation, but I will say one of my
favorite parts of the last episode we did with Pete in it was the part he said he's
working with synthesizers and I got to throw in some craft work. That was exciting.
See craftwork my friend is music. So, I don't know what this stuff is.

SH: This from a man who uses Lady GaGa remixes when I'm not looking. So this is my way of
getting back at you. It's Commodore 64 week on This Developer's Life, Dinosaurs. Let's
hear again what David Sokol is doing with Fortran.

DS: Fortran is an interesting programming language simply because it's one of the
oldest programming languages that's still in use today besides assembly. It's varied
simply because you can definitely tell the difference it and when something is written in
you know, Fortran 66 versus Fortran 77 versus Fortran 90 versus the new Fortran that was
only release about ten years ago. They all have very distinct coding styles and it's
something you just don't see with the .NET Framework where you have a new revision every
couple of years where you can say, "Oh, this person's using these helper classes so it
must be .NET 2.0, or 3.5. The actual syntax and formatting of the language makes up what
version of the language you're using. It's also interesting because of the history
associated with the language, and the way it's documented. I mean, when I work with
Fortran on a day-to-day basis I go and look at pages that look like they were meant to be
formatted for Netscape Navigator, the gray background and the standard font that they all
use. They have a little update at the bottom of the page that was a couple days ago
because these Fortran libraries are still being actively worked on. They're incredible
simply because they are some of the most well debugged libraries I've ever used. You have
something that was written in 1970's and it's been adjusted once every five or six years
by a PhD or a researcher that focuses purely on this sort of function. You realize that
40 years of little tiny adjustments to this function makes it near bulletproof. Which is
something that's just required for some of the usages of Fortran, such as nuclear
industry, numerical computing, and finance.

SH: How old are you?

DS: I am 26.

SH: Tell me about how this started. You couldn't have planned this.

DS: No, when I originally hired for my company they wanted me as a .NET Developer. So I
went in, did my interview, the programming assignment was to do a little web application
that displayed a report. I did it in C#, not really thinking much of it. I accepted the
job, showed up first day, and they said, "Oh, by the way, we're a VB.NET shop." I had
programmed in VB.NET before, so I was taken a little aback because I really like C#, but I
say, "OK, no problem. I can do that." Then the second day, one of our researchers came in
and sat me down and gave me my "welcome to the company". He said, "We do all of our
research code in Fortran. We do that because we all know Fortran, and we use to do it in
assembly." The research department basically decided that we're not going to learn another
programming language. We're just going to use Fortran for anything we have. So I laughed
at it, because I didn't think that, "Oh this is some researcher, he's going to be writing
some research, and give me some formulas" and I'll go ahead and plug them into VB and be
good to go. I didn't realize I would be taking his formulas and implementing them in well
structured Fortran in a 64-bit environment.

I had this one crazy Russian professor at my university who always taught a Fortran class
for the engineering students. None of the Computer Science majors want to take that
Fortran class because no one thought that we were going to be doing Fortran. He's always
put a plug in his own classes of software development, "Oh, by the way guys, I'm teaching
a Fortran course. You guys should take it. It's very useful in the business world if you
ever do any sort of engineering or finance stuff." None of us took it. None. I came back a
year later to talk with him and catch up with the professor, and he's like "Oh yeah, so
you're doing Fortran now?" I said, "Yeah, you were absolutely right." He's like "That's
one of the best languages there is." It works well with multi-core and all the high
performance stuff we're getting out of stuff like F# now. With Fortran you get very nice
performance characteristics because almost all of the functions are written, well at least
the way that we write our functions, are written as just pure functions where you just put
in inputs and get a single output. So you can very easily all the loops as vectors on a
multicore system and get massive performance gains, whereas something like C or C# where
you want to do all kinds of crazy things with multithreads. You don't get that kind of
performance guarantee you get out of the Fortran compiler.

SH: Did you think that you were in trouble when this started, or were you positive? I
could see someone saying, "Oh no! This is a bait and switch, this is not what I signed up
for." 

DS: I originally jumped in going "OK, this is my first job, I have an actual job now with
healthcare and that kind of stuff so I am going to give this my best effort ever." I went
into it and in about two to three days of just staring at old Fortran documentation, I was
pretty lost. I will say I did not go to my boss and go, "Hey, I'm tired of this, I don't
know anything about Fortran." I just complained to my other friends who were programmers
going, "I can't believe they have me working on this crap. It's so terrible, I'm going to
rewrite the entire thing in C#." Just because I can't believe somebody even uses this
stuff. Then as I got more and more into it, as we converted from the old Compaq Fortran
compiler to the - at the time - just released Intel 64-bit Fortran compiler I realized
what a huge undertaking it would be to rewrite all of this well-crafted Fortran code into
something that was even remotely performance equivalent in a managed language or even C.
Getting into it and getting use to all the compiler flags, figuring out what a vector was,
trying to get all of the old libraries we had used, which some of them were taking binaries
that were compiled in the 80's, and still referencing them in our code. Trying to get all
those things on a modern system was just a huge headache. It required me to basically keep
this long changelist of all compiler flags that they used so I could get right combination
of about fourteen to fifteen flags just so that our code would compile properly. It was a
huge pain because there isn't any information available now on trying to get a compiler
setup for Fortran. To resolve libraries references and those kind of things I had to use
a third party utility, Filemon, to figure out exactly where the compiler was looking for
things, then figure out where I should put stuff to get it to compile. It was me
essentially reverse engineering the compiler because we didn't exactly know what it was
and no one wanted to take the time who had experience with Fortran to help me figure it
out.

SH: At what point do you just give up? I mean, maybe this is a young person's game, but
you're describing, not just speedbumps, but huge walls in your way. You just say, "Come
on, forget this dead language."

DS: I was trying to rewrite a function for a Goldberg calculation. Now, I don't even know
what that was. I was just trying to take the code that was written in Fortran and
translate word for word into VB.NET. That in itself is not that hard. You can take and
copy-and-paste a piece of Fortran into Visual Studio and change the weird syntax for the
.GT for greater than into an arrow you're good to go. What the problem was, was the
external library functions.

(11:46)