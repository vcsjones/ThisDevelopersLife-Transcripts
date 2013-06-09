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
.GT for greater than into an arrow and you're good to go. What the problem was, was the
external library functions that I reference. There are functions that just don't exist in
libraries for VB.NET, or they exist and they are not freely available libraries. There's a
library called IMSL that we use pretty extensively in Fortran. It used kind of shipped by
default with Fortran compilers, like the HP Fortran compiler or the Intel compiler has a
single user license for this library. This think cost like $3,000. You think of that and
you compare a single user license for DevExpress or SyncFusion and compare that to this
one tiny numerical library for $3,000, it seems absolutely ridiculous to pay those
licensing costs. On top of that, we got things like the Mathematical libraries aren't
licensed per developer, they're licensed per processor that the code is executing on. They
used a method to figure that if have enough money to buy a lot of processors, you have a
lot of money to buy their software. After struggling with this crap for about three to
four weeks I finally got it to the point where the code would compile and got checked into
TFS and was into a version control system. At that point we designated this one machine
that was in the office that sits under my desk right now as the machine that would compile
our release code on. If anything happened to that machine, we're SOL. We take daily
backups of a snapshot, but that is the one machine that can compile our code properly. It
would probably take two to get it even running again.

SH: Is this because this is a niche? Is it because, you know how you hear about people
selling really old comic books for $3,000 and you say "well, who would ever spend that
much money on such an obscure old thing?" but then you figure, there's a niche - it's a
niche, or are these the real programmers? All these .NET guys and all this Microsoft and
Java and all this $99 grid view type stuff, are we just playing at business, but all the
real work is happening in Fortran and underneath?

DS: I think that part of the issue is Fortran is not meant for programmers. What we call
programmers will write ASP.NET applications, or WinForms or Linux, or that kind of stuff.
Fortran is meant to express numerical functions and formulas. It stands for formula
translation. We recently hired a guy about a month ago, and he came in, he's about 28 or
29 years old, and he came in writing Fortran. He's been cranking our new Fortran code for
the past two or three weeks now. He's not a trained software developer, he's a climate
scientist. He's writing some software to basically try and predict hurricanes when They
make landfall into the eastern United States. Now, I'm not one to be able to go in and
tell him, "Look, don't program in this language because it's dead" because that's what
he's been using and that's what works for him. His specialty as a client scientist far
outweighs the pain of us trying to force him to write in a language he's not familiar
with. When you deal with finance and research, you're basically going to be dealing with
Fortran. Those specialists who aren't programmers are going to be working in whatever they
are most comfortable with. As programmers we're kind of in a weird position where we have
to kind of bow to the whim of the specialist in that area, and still make it work, just
because their research is more valuable than the code that we produce.

SH: Huh. Do you think this language will live forever?

DS: It's definitely got the best track record for staying alive. I think it will. The fact
that we have nuclear reactors running Fortran. We have new Fortran developers every day,
just not in the CS perspective. It's going to be around for quite a long time, and the 
functions they've built into Fortran 2000, I'm not sure if there is a Fortran 2010, but it
would make sense that there would be, actually make it a decent language. They got rid of
all the terrible things in Fortran 66 and Fortran 77 to make it respectable. There's no
reason it shouldn't be moving forward. We just kind of have this stigma as developers to
basically ignore this language we read about in the old archives or usernet usergroups.

SH: Do you think that C# could live this long?

DS: I do not know. I would hope so, but one of the things that makes Fortran incredibly
long lived is it's built on research institutions. It's built by the same people who gave
us the internet. C# is controlled more-or-less by Microsoft. Java is controlled more-or-
less by Sun, and then eventually by Oracle. Whereas Fortran has basically for the past 30
to 40 years been controlled by a group of academics that are all working to make the
language better. Even though they have an incredibly long revision time, roughly ten years
between versions, they always end up making forward progress. I think the fact that mostly
it's rooted in academia rather than in a corporation just makes outlive everything.

SH: So Fortran is 50? More than 50 - and you are 26. So you're using a language that is
twice your age. Do you think Fortran is like the Latin of programming, or is it like the
English?

DS: I would say it's the English. I'm going back to where you initially learn English and
sentence structure, and you learn how to diagram sentences. They got the nouns, and the
adverbs, and figure out the adjectives. One of the incredible things about Fortran is it
makes these very basic concepts to programmers very simple to use. We have for loops and
do loops and those are very accessible within Fortran. Variables are very accessible in
Fortran, and in some cases they are much easier because you don't have to deal with all of
the other things like multithreading, reference pointers, or any of that stuff because
Fortran to me seems like a predecessor to Visual Basic, in a way. It took a lot of the
hard crummy things about programming in an era where machines are being programmed by
punchcard and assembly only, and makes the accessible to someone who just needs to make
some numbers compute. I would say it's one of the more basic programming languages, and it
would be a very good thing to give to a kid. It wouldn't be on a level of Logo, or any of
those other programming languages specifically designed for children, but it's a very
easy language to grasp in concepts. I was trying to convert some Fortran code to Visual
Basic, and I had worked for about two or three days converting roughly 3,000 lines of
Fortran to VB, and I had gotten the code to match all of the way out to the 8th decimal
place. I was very happy with it, and it ran decently the same. I took about a 20%
performance hit. Then I realized when I hooked this couple of library functions to our
main program that all of our numbers were completely off. We ended up predicting a loss of
a couple of extra billion dollars, which definitely put us in the red. I was trying to
track this down because I was confident, young and hardheaded, that the VB would end up
being better in the long run. It turns out that extra 9th decimal place that I hadn't
quite gotten to match yet was causing the issue. Some of the functions we used for
insurance loss prediction were that sensitive. That was the exact moment that I realized I
need to go home early, have a drink, come in the next day and start writing everything
that needs to be written in Fortran in Fortran instead of fighting the system. There's
just too much there for any one person to try and go through and rewrite it all. That's
when I stopped fighting Fortran and started going along with the current.

RC: So Scott, you know what Edsger Dijkstra says about Fortran.

SH: I know he's not a fan.

RC: I have a quote from him that I actually put in a blog post recently, he called Fortran
"The infantile disorder. Now 20 years old, it is hopeless inadequate for whatever computer
application you have in mind today. It's too clumsy, too risky, and too expensive to use."
I don't think he's a fan.

SH: When did he say this? Because what I am hearing is Fortran is a living language,
there's a lot of powerful stuff in it, multithreading, multiprocessor, x64. People are
doing work in Fortran, Dijkstra or not.

RC: True. That was a while ago. He also doesn't like COBOL, he said "The use of COBOL
cripples the mind. Teaching it should therefore be regarded as a criminal offense."

SH: I think we can all agree on that one.

RC: I think so too.

SH: I was impressed that David learned that not every problem is solvable in .NET. I was
most impressed when he stopped writing something in VB.NET and started writing something
in Fortran. I think that is the first act of This Developer's Life this week is trying to
tell us is that sometimes we can learn from the past, specifically dinosaurs that we may
have written off.

RC: And that VB.NET will cause you to learn Fortran, in relief.

SH: Clearly, that is exactly what I wanted you to take away from this segment.

RC: So, serious question though: so what? Are we telling people go learn Fortran? Are we
saying that Fortran .NET is coming? Is it going to be the new web frameworks built on
Fortran? What's the deal?

SH: No, I think what I took from this segment is that there is something to be learned
from the past, and to write off the past is to miss out on some opportunities to do good
work for the future.

RC: Do we have a Fortran geek trading card somewhere?

SH: I'm actually looking forward to getting David Sokol's rookie card, and trading that up
to, maybe I'll get a Rob Conery.

SH: Our next segment is Sean Bamforth who is talking about Dataflex, which is not a
language we should learn anything from. It's an old, old programming system that he has
given 15 years of his life to.

Sean Bamforth: So my name is Sean Bamforth, I'm a Dataflex programmer. Dataflex is a
programming language that's been going since 1980, and to be honest it feels like I've
been programming it since 1980. [laughs] That's my introduction.

SH: That's a beautiful introduction. It was magical. Were you born before 1980, I hope?

SB: I was, yes, actually. I haven't actually been programming it since 1980, I've been
programming it since probably 1990-something, 1995 probably.

SH: You know how we look down on programmers that program in VB?

SB: Yeah.

SH: Is it because it's VB, and I'm talking about VB6, the VB.NET people
don't need to send me a letter, or is it because it's old?

SB: It is because it's VB6. When VB6 came out, we hated VB6. I don't know about from the
people sides, Application Programmer sides, why they hated VB6, but I hated it because
database stuff was just impossible, and I was working with databases. VB6 was out, now
my date times might be a bit wrong here, but VB6 was out, and I think Delphi came out
after it, it was around about the same time. We loved Delphi, and it's database was
rubbish as well. Yeah, I don't know. It's always been hated, and maybe it's just because
it's Microsoft. The language was fine, it was absolutely fine. In a lot of ways, you can
program in Dataflex you can program in VB, there's a lot of similarities there.

SB: So Dataflex is a, well we can talk about new Dataflex or old Dataflex, I'll talk about
new Dataflex. New Dataflex is a compiled to pcode, as we used to call it, managed code
you'd call it now, compiled to pcode, VB-like I suppose. This is really hard, really hard.
It's a simple language, it doesn't do like your C+ things, you know where in C you say,
you're assigning a variable and you say "a equals 27"? You don't do that. You say "27 to
a". So in many ways a little bit like COBOL 2.

SH: Is it all caps? Is it a language that feels like it's shouting at me?

SB: It isn't all caps. It's just a language that likes to do things in its own way. I'll
give you another example, say you've a form, and you pop a button on it, and you want to
put some code in the button click event. Now in pretty much every language out there, that
on click stuff it goes in the form somewhere. So it's like like an event in the form, and
you wire it into button. Dataflex is completely different, you have the button, the on
click event is a method inside the button object. The button is defined as a code object,
and the events are defined inside that object. It's like maybe it's a good way of doing
things, but it's different from every single thing in the world. You might be able to tell
me otherwise. You might say "That's exactly how so-and-so works." I don't know, but it
strikes me as being different. It's got that COBOL syntax move something-to-something, and
weird objects.

SH: Somebody told me once that Finnish, the Finnish language - the language of Finland, is
the one language on the planet that like no other language and from a linguistic
perspective, it is as if they had been dropped through wormhole from another planet, and
it is their own thing. It's maybe a little like Japanese, but it's effectively like
nothing. Is this thing, Dataflex, is it a parallel universe from another world?

SB: It's not a parallel universe. I wouldn't say it was Finnish, I would say it's like, if
we were speaking English, German. It sounds the same.