---
layout: post
date: 2019-08-10
author: Ty Yiu
title: 'The Founder`s Diary'
subtitle: 'Entrepreneurial contribution to the \textit{"Resonance"} project' 
documentclass: article
toc: true
header-includes: |
    \usepackage{caption}
    \usepackage{subcaption}
---

\maketitle

\begin{abstract}
Each team received £100 and a new raspberry pi 3. The objective was set to be a
project involving the raspberry pi as a essential functioning part. This project
had to be revolving around the subject of \textit{sound}. In this project, the
teams were asked to build a prototype for an entrepreneurial undertaking. The
exact nature of the project could vary, though the team composition would
require constituent individuals with personalities corresponding to the three
founder's personalities, \textit{hacker, hustler and hipster}. The three
personalities create a balanced team, equipping each team with the skills
required for the \textit{start up journey} ahead.
\end{abstract}

\pagebreak

## Founding \textit{Resonance}
The team ended up being consisting of Linus, Gaby and myself, where Linus
represented the personality of the hustler and Gaby the one of the hipster.
Linus and me knew each other quite well already and we could be confident in
each other's abilities.

The idea presented itself from my thought of *"what is sound?"*, given that it's
the project's topic of question.
While wondering whether air, our atmosphere itself has a *vibrational
frequency* or how that would look like, given its fluid dynamics and composition
of multiple gases, I started doing some thinking about what the value of the
knowledge of vibrational frequencies of atmospheres could hold. As I was
thinking how to best find said frequency of air, the ISS and its isolated
atmosphere sprung in to my mind (for some reason quicker than a big, sealed tank
on earth). Then, I remembered having done research into fires in space and about
the properties of fire in an isolated atmosphere, which then led to the thought
of being able to manipulate the atmosphere in such way, that the fire would not
be in contact with oxygen, but rather nitrogen, which would cause the fire to
extinguish. 

So the idea was born, the build of a prototype that can extinguish
fire using vibrational frequencies. Alternatively to current fire fighting
methods, it does not require any fuel and as the project involved a raspberry
pi, it could probably be automated as well. 

## Week 2
Having had clear instructions and lots of creative freedom, it was time to
design a protoype that would be hacked together for our mvp/proof of concept.

I immediately went on to setting up the raspberry pi, of course headless,
because who needs a monitor and input-devices when you have ssh. The challenge
of the day was to set the pi up, including getting a keyboard and mouse, which I
really wanted not to buy with the budget we were given. 

The biggest pain the whole week originated from the pi not being able to be
accessible via ssh. Small problems like "correctly writing the wifi's name" or
"putting the setup files in the correct places on the pi's boot drive" arose a
couple of times and kept nagging me. 

Once set up, we started making thoughts about the parts we'd need for the
prototype build. I did set up an audio system before and had knowledge about
what we'd need and my hobby background of engineering and physics came in quite
handy for knowing how a speaker works. That was an advantage, because we could
save a lot of costs building our own special purpose speaker, as it, unlike
commercial product speakers it would not require to be varied in pitch much, nor
that it would need different speakers for different pitches. The goal was to
find a frequency that is working and build a speaker to solely produce one
frequency. Besides the speaker, there would need to be a connection between the
speaker and the raspberry pi that crates the frequency, electronic parts, like
cables and the sensor, for mentioned automation, detecting a flame. I gave the
list of parts with vague specifics to Linus to find possible choices of specific
products we could buy. Gaby and Linus were also making thoughts about the
commerial application of the idea in the meanwhile.

While filtering the possible choice of parts, I started digging more into the
theory of the project. I downloaded a frequency tone generator app for my phone
for initial tests, maybe my phone speaker could already make enough of an impact
to turn off the flame of a lighter. Somehow, from having read a lot about sound,
waves and frequencies for my high school specialisation subject, physics, I had
the thought of starting out at 60hz, one tick per second and vary pitch to see
if there were and noticeable changes in the flame when directing the sound wave
front closely to the flame. And very well, even at 60hz, my initial starting
point, the flame did react. The first solution was found, from now on there was
proof of being able to affect fire using sound.

## Week 3
Because of the previous problems with the pi's connectivity, I formatted the
pi's SD card and installed the lite version of buster, which has no GUI, for the
*obvious* need of performance considerations. Also, I set up the ssh key-pairs
to not having to log-in every time manually. Having ordered the parts I began
writing a simply python script that reads from the GPIO pins and another script
that generates a steady frequency and a third one. The first script would be
used for detecting a flame via the infrared sensor, which's detection would then
run the frequency script for so long, until the sensor doesn't read any further
flame present.
Unfortunately, I forgot to order connector cables for the sensor
to the raspberry, because they were both male and didn't think soldering the
contacts would be big of a problem. I was so wrong, my soldering iron isn't
meant for delicate work and I made a huge mess, while using tons of solder and
wasting loads of time. After more than an hour I had three wires connected,
though the connections did break afterwards a couple of times, after which I
decided to order the jumper wires.

Having found out that the idea would actually work, it was time to optimise and
scale the effect. To do so, I used my own home-speaker and connected it to a
frequency generator program. The effect seemed to be maximised when using the
low-frequency woofers of the speaker, instead of the tweeters, which indicated
to me that the volume of air movement would probably be a factor. The diameter
of the speaker cone would move more "energetic" waves, though also more "wind",
which I wanted to make clear is not the reason for the effect to work. The
subwoofer seemed to create an actual air current, which I thought could be
reliable for the flame extinguishing. Of course, whether the atmosphere itself
is moved or individual molecules is of no interest to the flame, but have the
same effect, the separation of flame and source. The proposed method achieves
the separation by vibrating *all* oxygen molecules only, so that other gases
fill its position, such as nitrogen, rendering the flame unable to burn. 

Knowing this could work and having seen it in action, I decided to see what
works behind this mechanism and also whether "60hz" would be the best frequency.

My research into *"Atmospheric accoustics"*, how I call it, started with
*resonance*, which is also where the name of the team originates. Natural
resonances or vibrational resonances must exist on smaller, molecular scale and
so that led me to *molecular vibration*. While learning about that, I found out,
that di-atomic molecules, like oxygen have different vibrational frequencies and
can also vibrate in different planes/dimensions, thus are easier to vibrate. 

### Theory
The effect we are making use of can simply be attributed by the following
effect:

> If the relaxation time is just the right value, then when a pressure wave
> passes by, the increased translational energy is converted into vibration and
> then back into translation coincident with the arrival of the low-pressure
> region. The wave amplitude is attenuated since the acoustic energy is
> converted either to random molecular motion (heat) or to pressure that is out
> of phase. When the acoustic frequency is of the same order of magnitude as the
> relaxation frequency (1/2 pi tau) of a particular vibrational mode, air can
> induce significant sound attenuation. The relaxation frequencies and maximum
> attenuation amplitudes vary with the type of molecule, the mode of vibration,
> and the presence of other types of molecules such as water vapor. (Vibrational
> Relaxation | ScienceDirect Topics. (2019))

Knowing we are working with oxygen and nitrogen, as they mostly make up the
atmosphere, it makes sense to calculate their molecular vibrational relaxation
state. We will need them to calculate the *"Attenuation coefficient"*, which
describes how permeable a medium is for a sound "beam" / directed sound
wave-front. That coefficient then gives indication about how easily a specific
frequency moves through a given medium. That in turn also means how well the
vibrations are transferred from molecule to molecule or better said, how much
energy, in the form of vibrational energy is lost over distance. 

Assuming a temperature of 20 degrees C, 70% relative humidity and that the
atmosphere is only Nitrogen/Oxygen: (Engineering Acoustics/Outdoor Sound
Propagation. (2019))

For oxygen molecules, 
$$
f_{r,O} = \frac{1}{P_{s0}} {24 * 4.04 * 10^4h * \frac{0.02+h}{0.391+h}}
$$

$$
f_{r,O} = \frac{1}{1} {24 * 4.04 * 10^4*0.7 * \frac{0.02+0.7}{0.391+0.7}}
$$

Convert from wavenumber to hertz-frequency:

$$
f_{r,O} = 18687 * 2.998*10^{10} = 56Hz
$$

While for nitrogen molecules,
$$
f_{r,N} = \frac{1}{P_{s0}} (\frac{T_0}{T})^\frac{1}{2} {9 *
280he^{-4.17[(\frac{T_0}{T})^\frac{1}{3}-1]}}
$$

$$
f_{r,N} = \frac{1}{1} (\frac{293}{273})^\frac{1}{2} {9 *
280*0.7*e^{-4.17[(\frac{293}{273})^\frac{1}{3}-1]}}
$$

$$
f_{r,N} = 193.17Hz
$$

,Where $T_0$ = reference temperature (K), T = atmospheric temperature, $h$ =
(absolute humidity) (%), $P_{s0}$ = reference pressure

So in fact, the 60hz that I had in my mind from the beginning on were pretty
close to the actual vibrational relaxation frequency of Oxygen.

If we were to try to optimise the effect for longer distances, the acoustic
attenuation due to atmospheric absorption could give indication about what
frequencies propagate best in a given medium with circumstances, like
temperature, atmospheric composition, pressure and humidity. 

## Week 4
After having done the calculations and having thought of knowing the theory, the
assembly of the prototype started. Linus and me met up at my place and he gave
me a helping hand in building the prototype. The speaker cone we bought was
hooked up with speaker wires to an amplifier, which was connected via aux to the
raspberry pi. The software already coded and installed, was running constantly
in the background as a service within systemd. It continuously checks the GPIO
input to which the IR sensor was connected, if there was a flame detected. At
first there was little effect to even the smallest flame, which was really
throwing me/us off for quite some time. The problem was the above mentioned
acoustic attenuation due to atmospheric absorption, or better said the problem
was, that the effect was minimised. I forgot two physical effects that were
overriding the wished effect.

The first one was the *Inverse-square law*, which supported the attenuation
effect, so we installed boundaries. These boundaries were cylindrical and in
length as defined by the standing wave harmonic, for tubes which are closed at
one end, of the used frequency, which was varied. So the boundaries were made
out of flexible cardboard, to allow the variation of length of the cylinder. 
The other effect I had forgotten to realise acted, was bernoulli's law. We
closed the open end of the cylinder boundaries off with more cardboard, and cut
a hole in it, so that there would be a pressure difference within and outside
the chamber. The closing off of the tube's length at the harmonic also allowed
resonance to further increase the pressure, due to internal reflections. We did
some testing with these changes to the design of the prototype minding these
effects.

The result was a much more focused *"beam"* of sound waves, accelerated through
a pressurized chamber, which was able to extinguish a candle of further than
1.2m away (indoors, no interference or wind).
Linus and me were so glad after these improvements, we literally started jumping
around in laughter.

## Week 5
Having finished our prototype, there were still some problems that kept occurring
with the raspberry pi, specifically that it wouldn't connect to the network I
set up it should connect to. It turned out, that the lite version of the buster
OS doesn't come with a package, that copies the network configuration files from
the boot partition into the linux networking directory. A quick install of that
package fixed the problem, seemingly for good. 

Another thing that finally arrived were the female-to-female jumper wires, to
easier connect the sensor to the pi and in a much cleaner way, than the prior
soldering mess I created. The setup was much easier now, not having to worry
about the delicate soldering connections.

As our prototype was finished and working and with little easy to achieve
optimisation in reach, there was time to think about where this idea could be
taken next, given an investors pitch were to be successful.

### Further steps...

The next step that I would take, as a hacker, with relative financial freedom
for the project, is optimisation and testing. The optimisation refers to the
materials and shapes used in the prototype. Metallic cylinders may work better,
if relatively flexible, than the current *cardboard*. There are also other
shapes that could be tried out, a cone shaped or pyramidal shaped housing would
probably increase bernoulli's effect. Then there are other forms in complete, a
revamped design idea I had, came from a Sony television, which vibrated the
display instead of having speakers. That concept could be used for a flat
version of the system. The testing refers to the capabilities of each setup.
Now, we know little about the capabilities, the speaker can output more than a
hundred watts, though only receives fourty-eight, room for optimisation as well. 

The other step I would take, is a workaround to the current patent, that holds
many frequencies of the sound spectrum for fire extinguishing purposes. That can
be done with for example trying ultra-sound or infrasonics.

In terms of business, I would target the system to either insurance companies as
an automated system to lower potential risk of house-fires originating in
kitchens or to server farms and computing centers. The server farms have ideal
conditions for the system to operate and alternatives are destructive or toxic
and non-environmentally friendly. Another target would be the space station and
future rocket systems. Due to the atmosphere being precious during flight and
alternative methods of extinguishing fire known from earth don't work, the
system would be an unseen solution to a very dangerous and costly problem.


\pagebreak

> I did not include all my calculation, nor any code, nor any images from the
> build or videos. This report solely highlights my personal contributions and
> problems faced and how they were overcome.

## References

Molecular Vibration | ScienceDirect Topics. (2019). Sciencedirect.com. Retrieved
9 August 2019, from [here](http://bit.ly/2OKP1wT)

Vibrational Relaxation | ScienceDirect Topics. (2019).
Sciencedirect.com. Retrieved 9 August 2019, from [here](http://bit.ly/2GWt5Zl)

Engineering Acoustics/Outdoor Sound Propagation - Wikibooks, open books for an
open world. (2019). En.wikibooks.org. [here](Retrieved 9 August 2019, from
https://en.wikibooks.org/wiki/Engineering_Acoustics/Outdoor_Sound_Propagation#Attenuation_by_atmospheric_absorption[5]_[6]_[7])

CN204932657U - Low frequency sound wave fire extinguisher - Google Patents.
(2015). Patents.google.com. Retrieved 9 August 2019, from
[here](https://patents.google.com/patent/CN204932657U/en)
