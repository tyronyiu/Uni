# Mathematical Medicine: Positron Emission Tomography (PET Scans)

[Positron emission
tomography](https://en.wikipedia.org/wiki/Positron_emission_tomography) is a
modern day scanning tool often used to observe the metabolic processes of tissue
in 3D. The scans the physician receives look quite similar to [X-ray computed
tomography](https://medium.com/@sullyfchen/mathematical-medicine-computed-tomography-ct-scans-f2a762f398e7)
(CT scans), but the mechanism behind each are quite different. Take a look at
the PET scan below, showing levels of consciousness based on brain tissue
metabolic activity.

![](https://cdn-images-1.medium.com/max/1600/0*1qSJ-EpcfTRTD2AO.jpg)
<span class="figcaption_hack">[Source](https://sciencebasedmedicine.org/pet-scans-predict-coma-outcome/)</span>

![](https://cdn-images-1.medium.com/max/1200/0*1asNTqE4_iELOl_T.gif)
<span class="figcaption_hack">[Source](http://bocaradiology.com/pet.html)</span>

Again, in the scan to the left, you can see a the 3D reconstruction of tissue
metabolic activity from a PET scan. Notably, we see increased activity along the
chest walls, indicating carcinoma, as well as the supraclavicular fossa.
Information like this cannot be obtained from a regular CT scan, and is thus
invaluable to many specialties, particularly oncology and neurology.

The basic mechanism behind a PET scan is as follows: inject the patient with a
glucose-analog tagged with a radioactive isotope (most often
[fluorodeoxyglucose](https://en.wikipedia.org/wiki/Fludeoxyglucose_(18F))), and
use the radiation emitted to localize tissues with high metabolic activity
(tissues that consume more glucose). There’s *a lot* more to unpack here, so
let’s go a little more in depth, starting with the acronym “PET” itself.

### Positron Emission

You may remember the concept of radiation from your undergraduate chemistry and
physics courses — it’s essential the release of *something *energetic from the
nucleus of an unstable atom to allow that atom to decay into something more
stable. There are many “*somethings*” that an atom can release, from heavy
helium nuclei to energetic gamma radiation. In our case, we are looking at
isotopes that release something called a “positron” during their decay. A
positron is what’s known as an “antiparticle,” a mirror-image of what we define
as “regular” particles. Specifically, a positron is a mirror-image of an
electron. It’s very similar to an electron, except it has a positive charge
rather than a negative charge. During positron emission, a proton is “converted”
**(it’s a lot more complicated and we’ll talk about it later)** into a neutron,
releasing a positron in the process (notice how the charge is conserved!).

What many people don’t realize about PET scans is that it’s *not* the positrons
that are being detected and scanned, but rather a byproduct of the positrons’
interaction with other charged particles. When an antiparticle and a particle
collide, they annihilate spectacularly in a show of lights, producing gamma
rays. So, when a positron emitted by the radioactively tagged glucose molecule
smacks into another electron nearby, they annihilate each other and release high
energy gamma rays in the process, which are then picked up by the PET scan
detector array.

### **Positron Decay and Annihilation**

You may know that atomic nuclei are made of protons and neutrons, but there’s
actually another level of depth to these building blocks: quarks.
[Quarks](https://en.wikipedia.org/wiki/Quark) are the constituents that make up
protons and neutrons, along with many other larger particles. There are many
kinds of quarks, and their interactions alone are extremely fascinating (see
[quantum chromodynamics](https://en.wikipedia.org/wiki/Quantum_chromodynamics)),
but we will be focusing solely on the quarks that make up protons and neutrons:
the “up” and “down” quarks — yes, those are really their names. In the simplest
explanation possible, two up quarks and a down quark “bonded” (via
[gluon](https://en.wikipedia.org/wiki/Gluon) exchange) together form a proton,
while two down quarks and an up quark form a neutron. In this manner, you could
see how “converting” a single up quark in a proton into a down quark could
change the entire thing into a neutron, right? That’s exactly what happens in
positron decay — a random flying particle called a “[W+
boson](https://en.wikipedia.org/wiki/W_and_Z_bosons)” interacts with an up quark
in a proton via the [weak
force](https://en.wikipedia.org/wiki/Weak_interaction), converting it into a
down quark. In the process, a positron and a
[neutrino](https://en.wikipedia.org/wiki/Neutrino) are released. Below is a neat
diagram called a [Feynman
Diagram](https://en.wikipedia.org/wiki/Feynman_diagram) depicting the whole
process.

![](https://cdn-images-1.medium.com/max/1600/0*UvtbJe9V_94GV1nG.png)
<span class="figcaption_hack">[Source](https://www.researchgate.net/figure/Feynman-diagram-of-positron-decay-Protons-and-neutrons-are-not-elemen-tary-particles_fig1_277845076)</span>

![](https://cdn-images-1.medium.com/max/1200/0*h7x3mzq0UfzobkNi.png)
<span class="figcaption_hack">[Source](https://en.wikipedia.org/wiki/Electronâpositron_annihilation)</span>

After the positron is released, it travels for a distance on average about a
millimeter, until it interacts with an electron, annihilating each other
producing the gamma rays detected. Interestingly, the interaction always
produces two gamma rays (for conservation reasons), and these two gamma rays are
released in directions approximately 180 degrees apart. This forms the basis of
the localization part of PET scans: when we detect two gamma rays at around the
same time (within a few nanoseconds), we can trace the paths of those gamma rays
back to the initial spot they came from (inside the patient). In reality,
measurements and uncertainty prevent us from locating the exact area the photons
came from, but at best we localize the line along which the photons traveled.
When many detected lines seem to all be *intersecting* at the same spot in the
body, we can make a good guess that the specific spot is producing the gamma
rays. In practice, it’s much more complicated, of course.

### The Detector and Localization

Positron detectors use
[scintillator](https://en.wikipedia.org/wiki/Scintillator) to detect gamma rays.
The scintillator “converts” a gamma ray into a small burst of visible light
through some complicated interactions. By measuring where and when these light
flashes occur, the gamma ray can be detected and localized.

![](https://cdn-images-1.medium.com/max/1600/0*X_0UHd8GBNG85OYu.png)
<span class="figcaption_hack">[Source](https://www.radiologycafe.com/radiology-trainees/frcr-physics-notes/pet-imaging)</span>

There are many, many difficulties presented with localization however. First of
all, sometimes the gamma rays don’t actually end up at 180 degree separation
when they reach the detector, due to internal scattering and other effects.
Since the detector always assumes the photons are scattered at 180 degrees, this
can lead to false positives. Similarly, by random chance two unrelated gamma
rays can be detected at the same time, leading to another false positive.

![](https://cdn-images-1.medium.com/max/1600/0*mGuRr8yzyvS2-WWS.png)
<span class="figcaption_hack">[Source](https://www.radiologycafe.com/radiology-trainees/frcr-physics-notes/pet-imaging)</span>

As you might be gathering so far, the precision with which the travel time of
the gamma rays can be measured determines the quality of the image. Most PET
scanners have a resolution of a few nanoseconds (very very short time frames!),
while some newer and more expensive ones have time frames of a few hundred pico
seconds. Even this kind of unimaginable precision isn’t enough to remove all the
uncertainty. Additionally, the scintillators themselves have a small “cool down”
period where they are not as sensitive to gamma rays for a bit. All of this
uncertainty leads us to the next process: filtering, error-correction, and
computed tomography.

### Processing the Data

For the most part, a similar process to CT scanning can be used — the Radon
transform and filtered back projection. You can read all about that in [my
article about CT
scans](https://medium.com/@sullyfchen/mathematical-medicine-computed-tomography-ct-scans-f2a762f398e7).
More modern algorithms, however, estimate what the most likely distribution of
metabolic activity is in the tissue that would produce the observed results.
These algorithms use *very complicated* statistical techniques which should
deserve an article of their own. If you are mathematically/statistically
inclined, you can read about [one of those
algorithms](https://www.ncbi.nlm.nih.gov/pubmed/18238264) here.

### Wrap-Up

The gist of this whole process is as follows:

1.  The patient is injected with a radioactively tagged glucose molecule (or glucose
analog) which will later undergo positron emission.
1.  The ejected positrons travel for about a millimeter (depending on the isotope)
until they interact with an electron.
1.  The electron and positron annihilate, creating two gamma rays which travel in
directions separated by about 180 degrees
1.  The gamma rays hit the scintillator, producing a flash of light detected by
another detector
1.  If two gamma rays are detected on two different sides of the detector at about
the same time, a line is computed along which the gamma rays traveled
1.  Using advanced statistical methods, this collected data is used to generate a 3D
model of the metabolic activity in the patient being scanned.

PET scans are pretty cool!

* [Science](https://medium.com/tag/science?source=post)
* [Pet Scan](https://medium.com/tag/pet-scan?source=post)
* [Medicine](https://medium.com/tag/medicine?source=post)
* [Physics](https://medium.com/tag/physics?source=post)
* [Radiology](https://medium.com/tag/radiology?source=post)

### [Sully Chen](https://medium.com/@sullyfchen)

Machine learning, mathematics, medicine. I do research in biotech.

