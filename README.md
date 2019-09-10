STFU: STANDARD TEXT FORMAT, UNIVERSAL


<pre>
<H1>Starting Notes:</H1>

All numbers are inclusive [0i..5i]
such as for(i=0;i<=5;i++) or while(i>=0){i--}

Leading (first) bit is most significant.

<H1>Bit Switch:</H1>

00xxxxxx [0i..5i] "6 bit" Number
01xxxxxx Control Symbol
1* Formal ("UTF8" style) Expander

---
<H1>All Characters are in Expanders</H1>

ALL "letters" or symbols "character" <= 127
are encoded in 2-byte Expanders:

110xxxxx 10xxxxxx

"letter" 'a' is 110 00000 10 1100001

Numbers and some Control Symbols are mapped from "ascii" of the corresponding "character".

---
<H1>Expanders, Extenders & UTF8</H1>

All 8-bit Byte Extenders are available:

len byte[0]  byte[1]  byte[2]  byte[3] ...

"UTF8":

2 [10i]    110xxxxx 10xxxxxx
3 [15i]    1110xxxx 10xxxxxx 10xxxxxx
4 [20i]    11110xxx 10xxxxxx 10xxxxxx 10xxxxxx

<B>The "Books" above 2^23i include the "UTF" in slot 0
and the forms, layout, tooling, phonemes,
and properly sorted "Code Points"; 11111000 is "UTF"</b>

5 [25i] 111110xx 10xxxxxx 10xxxxxx 10xxxxxx 10xxxxxx
6 [30i] 1111110x + 5× 10xxxxxx
7 [35i] 11111110 + 6× 10xxxxxx
8 [41i] 11111111 + 7× 10xxxxxx + Another Expander

---
<H1>Symbol Tables</H1>

For any Symbol Table: A Control Symbol or Chracter $

$(index)

$(number'index'tree)(v)

or

$({Any Extenders})

$({Any Extenders}'iNd3X'{Any Extenders}'TreE)

But not mixed in any Turn.

<H2>Turns & Slots</H2>

The entire system is based on a Control Symbol (sometimes with a initial time slice), a sequence of Turns through a route "tree", a matching composite value, and compositions of sets in Slots. 

$time(turn'turn)({any})

In any of these, both the Turns and Slots, a STFU8 or UTF8 "text", a Context @() or !() or a Reference with Associative, an indexed tree ()() and composition, a *() "type" Declaration or a System ~(bits) can be included. A Number can be used as a Turn, as can a STFU8 or UTF8, even a turned reference Context!

Or a set (') of any of them in Slots with or without the Turn index named. [N] if not ()()


<H2>Adding Time:</H2>

The initial time slice can be included for temporal versioning,
it's associated references per referenced initial time as well.

Numbers are 6-bit, the initial time slice is msb aligned to resolution.

$5i5i() and $5i5i()()

$5i5i56() and $5i5i56()()

The time comes from a chopped 64b time, called "Fone"

The Fone's time is chopped to 2^16 ms, slightly more than one clock second, 65 Fone Seconds, and 6 bit multiples. A short Fone slice is Fone Minutes or Fone Hours, to 64× each.




---
<H1>HTTP Bytes</H1>

There is a compatibility mode for HTTP
using the old "ascii" characters as control symbols and numbers:

<script>
for (
var i = 0;
i <= 255;
i = i + 1
)
{
var s = String.fromCharCode(i);
if (
s == encodeURI(s)
&&
s == encodeURIComponent(s)
)
document.write(s);
}
</script>

Out of:

<script>
for (
var i = 0;
i <= 255;
i = i + 1
)
{
var s = String.fromCharCode(i);
if (
s == encodeURI(s)
)
document.write(s);
}
</script>

Thereby:

$(Index'Tr3E)(v)

---

For @ and !, the Universal Contexts:

@time(Context'tree@host.tld)(😴) is an Associative Reference 
@time(Context'tree@host.tld) is the Context (and "file" name!)
@time(Context'tree@host.tld)() is the References "file"!

Same for !() and !()()

Or without time:

@(Context'tree@host.tld)
@(Context'tree@host.tld)()

These are the URI IRI URL "file name" or reference. at host.tld's interface, as declared in /@(@host.tld) or /@() ”file" via host.tld

<!--
\n
(
~
(index'Tree)(v)
)
\n

!'()*-.0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz~

Out of:

 !#$&'()*+,-./0123456789:;=?@ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz~ 

-->

---

<H1>Transport Syntax</H1>

HTTP and IRI (URI, URL) "% encode" everything except:

POST:

!'()*-.0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz~

GET & HEAD:

 !#$&'()*+,-./0123456789:;=?@ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz~ 

Of the available "ascii characters", 

<H2>63i Numbers:</H2>

0123456789
abcdefghijklmnopqrstuvwxyz
ABCDEFGHIJKLMNOPQRSTUVWXYZ_-

<H2>Control Symbols:</H2>

Per the available Symbols, and with the ~ in 0111111, the ' is , and the Syntax is $()()

# breaks in "IRI"
$ breaks in PHP, etc
* and : break in file systems
/ is IRI Path
punycode has mutilated -
and social media misuses _


POST:

!'()*.~

GET:

 !#$&'()*+,-./:;=?@~

Available for HTTP Transport:

!'(),.;@~

And POST:

!'().~

The containing Symbols ( "left hand" and ) "right hand"
combine with the ' as $((')(')'()())() 
to form (iNd3x'Turns) with (index)(Slots).

These numbers or Expanders (including "UTF8")
provide the tree's Turns and the set's Slots.


---
<H1>Universal Structure:</H1>


<H2>Structure:</H2>

A local, universal, context, and system table are each required:

~ System
! Universal
.() Local
@ Context

The system table is explicitly reserved for host implementations but includes the minimal standards for operation.

The ! Universal Context is well-formed and extensible by any !() or the abbreviated @().

ALL character encodings including those < 128
use Expanders of 2 or more octets with high bit set.

The 64 numbers are 00xxxxxx and mapped to ascii in the initial encodings.

The @(@) Context is a combination of the context tree and the supporting "named" host.

@(@) are typically a "UTF8" Expander or 6-bit number (or null) indicating the primary context,
@(🐩
then the optional context's tree with '
@(🐩'😎'345'A'🦓
The @ Context delimiter
@(🐩'😎'345'A'🦓@
and the UTF8 Expander
@(🐩'😎'345'A'🦓@stfu.site
that can also have an "IRI" (URI, URL) styled path
@(🐩'😎'345'A'🦓@stfu.site/demo.php/
or fully formed "IRI" in "UTF8" 2+ Byte Expander
@(🐩'😎'345'A'🦓@https://stfu.site/demo.pho?x=
Closed with the ) other containing control symbol
@(🐩'😎'345'A'🦓@stfu.site)

Because ALL characters are "UTF8" Expanders, there are no " quotes or other convolutions.

The "named" host assumes TLD, but can be any system type. ~(demo'tel'sms)(1'000'000'0000)

<H2>Where you at?</H2>

For @ and !, the Universal Contexts:

@time(Context'tree@host.tld)(😴) is an Associative Reference

@time(Context'tree@host.tld) is the Context (and "file" name!)

@time(Context'tree@host.tld)() is the References "file"!

Same for !() and !()()

Or without time:

@(Context'tree@host.tld)
@(Context'tree@host.tld)()

These are the URI IRI URL "file name" or reference. at host.tld's interface, as declared in /@(@host.tld) or /@() ”file" via host.tld

<H2>Local Context:</H2>

Within a Context, indicated by the Tree of Turns,
there is content within:

@(🐩'😎'345'A'🦓.(some'thing)@stfu.site)

The ' and . are handled the same as ~ and !
.(local'tree), though ' is exclusively Turns or Slots in sets. ( starts a turn or set of slots. Implied " (' ".

This Turn, .() indicates the next turns are inside the container or box.

!(~(wire)(~(bits)('''))'(in'set)'@(a@b)'🤣.(3'🤗))

Because @(@) is a courtesy wrapper for !()(),
Both @(@) Context and all of the structures anywhere have the Turn Tree and the value.

In .(local'data)(this pair is a value, here it's an Expander)

The ' of Turns also functions the same way, allowing an in'set turn.

In any level, the ()((local'data)(value))

Or as a set of Slots:

()((local'data)(value)'RAW '(STFU8'UTF8)' in 2 octets or 10xxxxxxs '(local'STFU8'data'4)(value)'etc8s)

The @(@) Context and !() are the same way:

@(@)((local'data)(value))

Or more importantly

@(demo's0me'TrEe@stfu.site)(@(jack@twitter.com)(🤐))

Associative Reference!

This can map an @(@) or !() with the Associative Reference, typically a formally structured Syntax or an Expander suitable for the concept of inter-contextual association.

Internally at any level, any element in the tree can be associated to anything else:

.(local'data)(@(demo@stfu.site)(🤬))

Or

@(demo@stfu.site)(@(demo's0me'TrEe@stfu.site)(🤪))

Or between specific data points inside the box:

@(🐩'😎'345'A'🦓.(some'thing)@stfu.site)(@(demo's0me'TrEe.(local'data)@stfu.site)(🤯))

Simple!

@(demo's0me'TrEe.(local'data)@stfu.site)(@(🐩'😎'345'A'🦓.(some'thing)@stfu.site)(😜))


---
<H1>Associative Reference</H1>

Like the pair of @(@)(🤗) associations, any point in any context can have inter-related associations with any other, anywhere.

In !()() this is called "Cube" and "Ball" held left-hand and right-hand.

The "cube" has a box that holds stuff.

The "ball" is the Universal Context.

Your stuff is in the box, including your concepts of how other stuff is related (or not) anywhere, in the box or far beyond!

Your "cube" has its own "ball" where references from anywhere else are posted for reference. Every "cube" Context does!

Any Associative Reference can have a diversity of attributes. This includes the standard set and any others that you can come up with, including association by another concept in any context.

<H2>Associative Syntax Structure</H2>


---

<H1>Additional Standard Control Symbols:</H1>

@ Context @(@)
! Universal !()()
~ System Tables ~(bits)
.()() And ()() Local data

<H2>Declaration "type" Anywhere!</H2>

*() Declaration "type" anywhere

Any (named'index'🦓)(@(🐩'1am'😴@stfu.site)(😜🤯🤪)) can include an Associative Reference with it's own type!

.(named'index'🦓)(@(🐩'1am'😴@stfu.site)(*(@(😋'types'associative'😍@stfu.site)'
(😍'value)(3)'(😍'type)(🤯)
))


Is an easy example of a Declared *() "type" using named index values for Accurate Representation!

Any structure of knowledge or concepts can be represented and presented this way using the Declaration's referenced "show" "cube" "ball" "flow" and related definitions.

<H2>,() "Alternate Text" ~(hint)</H2>

At any level of Slots (except Turns), 
" ,() " can be included as an alternate "hint" (typically a short text name or description), and "overload" values set in YOUR reference to another context, such as changing the color of a tooling in the "cube" when using their layout process.

<H2>IRI Reference from ~(bits)</H2>

/() is included for IRI URI URL reference from a definition in the #Declaration *() on how to use those ~(bits). Typically the description exhaustively describes the structure (image).

---
<H1>Declaration Conditions</H1>

The entire system uses one standard format and one *() Declaration that includes the "host" Implementation getting and setting bits. 

Containers of bits referenced in the host have their Declared structure and describe their processes or configuration therein.

Valid "host" Implementations might extend a more direct physical process, like an ADD function of a Declared fixed bit width or "glsl" triangles into "show" or "flow". (Pixels)

<H2>Merging Structures</H2>

Multiples shall be handled as parallel records such as [a,b] of the same but different; many Associative References exist between the same Concepts, and similar Contexts may merge in presentation!

---

<H1>Declaration + "type"</H1>

The Control Symbol *() is the Declaration.

The Declaration either contains the definition of the structure or contains a reference to a Context that Declares the type's structure.

The Declaration *() can contain the entire definition and how to correctly present your concepts or context anywhere!

All structure, and all operation (such as the representation of your "cube" and "ball" and how to "show" them) are defined in the Declaration *()

The host Implementation need only a minimally simple and formally valid ability to copy bits to various "wire" or "line" interfaces including screen pixels, phone or Internet connectivity, or the host's memory.

The system in whole uses a "Table Basher" that is formally valid everywhere and collections of ~(bits) and *(structures) that you define.

There is a minimal or host implementation augmented set of "Truth Tables". ~(true) And logic "flow".

The *() includes everything necessary to calculate the Accurate Representation of your Context, Concepts, and Associated References and "show" them any way you want!

There is a Declaration of how to "show" your Context, including how to Accurately Represent your "cube" and "ball", and inter-associated concepts beyond your "ball" in the "show"!

Every Context has a cube and a ball, at every level.

The cube has stuff in a box, the ball has the Universe.

The cube has its own ball! Infinitely many cubes and balls inside each little Context (but preferably each general concept in it's own context) STFU!

The type Declaration * takes care of everything else!

<H2>Truth, Logic, FLOW</H2>

The elementary logic, presentation, data representation, ... and flow control are all contained in the System Table.

All you really need is the ability to copy bits between some place to another, at any scale.

By using bits and containers of bits with only a minimal get&set function, every Context controls the entire process of Accurately representing it's data and presentation!

<H2>SHOW CUBE BALL</H2>

Every context, at any level, is provided a "cube" to Accurately represent it's stuff.

Within the 4D cube, a 3D volume and time, you can represent your STFU any way you could possibly want!

Animation, 3d objects and tooling, human interaction, layout graphemes or audible phonemes, etc. You have explicit control of how your context is represented!

The "show" and it's "flow" in the *() Declaration describes how your concepts are presented in your "cube", how data from your STFU boxes are represented, and how Associative References in your cube or from it's ball are presented.

Beyond your "cube" at any level is a "ball" that includes the Contexts and Associative References for the entire universe.

Your *() Declaration's "show" handles ALL of the layout and presentation for your Concepts and Contexts anywhere they go, and do exactly the same for every STFU Context that gets to you!

<H2>Declaration Efficiency, Burdon</H2>

The Declaration *() includes an overview of the technical processes of presentation including controls for efficiency, complexity, detail, and the description of how to Accurately Represent the Concepts in the best way for anyone.

Everything goes in a "cube" or controlled by a "ball"!


<H2>Declaration's in Contexts</H2>

Every Context has a Declaration of it's structure and how to Accurately present it.

Any specific data can include it's own unique "show" or "type" or it can reference a Context *(*(@(@))) somewhere that describes a way you prefer.

Multiple ways are merged for the most correct representation possible!


<H2>FLOW & control</H2>

Every process related to your Context is controlled entirely by your description in the *() Declaration.

The entire system does nothing other than move bits around and tell the host Implementation to put bits as pixels on a screen or put bits to wire and get some more! (Any wire, audio, video, interfaces, camera, phone or Internet, or as a host for the data!)

Extensions of the bit operations in formally valid implementations make Accurate Representation and presentation very fast and efficient!

Entire complexities of process can be implemented in your Context with the "show" "cube" "ball" "flow" in the *() Declaration.

The template that shows this structure and Accurately Represents these Concepts is simply a set of descriptions in the Declaration that request the valid implementations "host" to move bits around to various places ALSO described by a Declaration in a Context.

Anywhere!


---

<H1>Initial Time + Re-Visioning</H1>

Accuracy of Representation is important. When you reference something you expect it to be accurate, not randomly changed into something else.

Control codes for previous & next allow the sequence in time to be loaded together.

A context could change to someone else, or become outdated.

@5i5i5i(@) or @5i5i(@)
!abCdEf(...)

allows for a n×6 bit initial time slice to be indicated, providing versioning and history and the References to it can be stored on the local time slice as well. msb aligned

@5i5i(@)() ALL THE REFERENCES!

It's better to create a new timeslice or tree'd Context when things change, keeping the other ones because someone somewhere else might reference them!





---

<H1>Tools of Implementation</H1>

In order for your Concepts and References to be Accurately Represented, you need to use 


This can be loaded and referenced accurately in parallel starting at any point using an expanding tree or linked-list that has offsets.

Because the Control Symbols and Numbers are never STFU8 nor UTF8, they will always be accurate.

A \n newline is processed similar to the ' but only between 

The Context "file" @(@) has everything in this simple box.

Your Accurate Representation is shown in a "cube" with all your local references and any local references to anything else!

The Associated References "Ball" @(@)() "file" has ALL of the references to it from anywhere else and is open-ended so it can be appended.

Same for !() and !()() 

---

<H1>Formal Syntax</H1>

Bit-Sequential processing tree with parallel offsets and optional alignments

.()(@(.()@)) expands inline.
()()' vs .()() locals

---

<H1></H1>

---

<H1></H1>

---

<H1></H1>

---


<H1></H1>

---


