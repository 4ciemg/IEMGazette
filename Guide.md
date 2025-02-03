#EQ Guide for IEMs
***

!!! danger 
	!!! warning  Do you need this guide?
		Another guide is available through squig.link databases in the Equalizer tab. The yellow question mark button has a short and useful guide that presents a decent chunk of this guide's content in a condensed manner, and is suitable for most people looking for a quick introduction to EQ.


!!! info Guide Overview
	The goal of this guide is to provide the necessary, stripped down practical information for equalizers (EQ) when it comes to audio reproduction, and is aimed at most people, from beginners to experienced users. Some basic theory will be summarized, but a general understanding of the hearing system, audio, and waves is useful.
	This guide will be mainly focused on EQ concerning **IEMs**, and will be updated frequently. Skip the sections you feel comfortable with, or just do whatever you want.
 
	There are 3 main sections in this guide: 
	1. Audio and EQ basics, where necessary foundational knowledge is summarized
	2. How to EQ, where detailed instructions and/or information pertaining to EQ are given 
	3. Case study, where demonstrations of the EQ process are shown 
	4. Measurement rigs, curves, and preference targets, where information about metrology is given


*Table of Contents*
[TOC2]

***
***
##Audio and EQ basics
***
###Recommended articles and videos

While not necessary to the guide, the readings from [Dale's Music Stuff](https://daystarvisions.com/Music/index.html) from HE1 up to HE7 are good, easy-to-digest yet in-depth articles that explain a lot of concepts and ideas that are immediately relevant to the task. It is focused on headphones, but the same general rules and suggestions also apply to IEMs. Reading them will provide much more information than what is given here in terms of audio and the hobby as a whole, while this guide is for the most part solely dedicated to EQ. Crinacle's [Graphs 101: How to Read Headphone Measurements](https://crinacle.com/2020/04/08/graphs-101-how-to-read-headphone-measurements/) is also an interesting read that dives into measurements and how to read them.


The following videos are also fun and intuitive ways of understanding audio and EQ.
[How Audio Illusions Trick Our Brains](https://www.youtube.com/watch?v=Sn07AMCfaAI)
[Every sound is SINE](https://www.youtube.com/watch?v=UrBZsUBibtk) 
[How to TUNE your headphones (the easy way!)](https://www.youtube.com/watch?v=PsijHAVLbuY)
[EQ Basics - Watch BEFORE you get started!](https://www.youtube.com/watch?v=FRm9qTmQHKo)
[The Limits of EQ - A case against using EQ profiles for headphones](https://www.youtube.com/watch?v=FD_s2s8Mw9k)



!!! warning 
	->**Before continuing, knowing how to read graphs is a crucial skill, and it is essential in using EQ. Knowing how to properly wear IEMs is just as important; getting a proper seal and consistent insertion depth will yield the best results.
	The FAQ and terminology sections are also worth taking a quick look at.** <-

***
###Measurements and warnings
Measurements in the headphone and IEM community often refer to frequency (magnitude) response (FR) plots where the x-axis represents frequency, in this case the audible spectrum band (20 Hz to 20 000 Hz or 20 kHz) in logarithmic scale to match how human hearing work. The y-axis represents amplitude/loudness/SPL, usually in dB, in linear scale. Together, they form a graph that shows **how loud something is at specific frequencies**. An important thing to always check is the scale of each axis; these are commonly modified to skew perception. These measurements are important for two reasons.

!!! info Importance of measurements
	1. FR is by far the most important factor when it comes to sound quality (ignoring factors like comfort, price bias, aesthetics, etc.) and is the main metric that is used both in the audiophile hobby and the acoustic preference research sphere
	2. Human hearing is **not reliable**. There are many pitfalls and flaws in our hearing, so it is usually recommended to use graphs and measurements as a foundation. It allows for efficient detection of flaws, and it also gives a visual aspect to latch on to

Do note that music can also be represented in such plots, where different frequencies will have different amplitudes. For example, imagine a song where there is only bass music playing, and another that only has a flute: the bass song will have higher amplitudes at lower frequencies, while the flute song will have higher amplitudes at higher frequencies. Of course, music has a time component, meaning that a singular FR graph of music only represents a snapshot of the music at a specific time. Intuitively, one might assume that IEMs also have a time component; this is covered in the [FAQ](https://rentry.co/IEM-EQ-Guide#faq). **All that is important for now is that an IEM's FR is all that really matters when it comes to objective metrics.**

->![Example of a frequency response graph. ](https://i.postimg.cc/ZKjcq1bh/mic-basics-frequency-response-content-1.png){49%:49%} ![Example of a frequency response graph. ](https://i.postimg.cc/fydyGycD/KZ.png){49%:49%}<-



IEM measurements are significantly more prominent than others because they are devices that are easy to measure compared to headphones and loudspeakers. Further more, the prevalence of affordable clone couplers - coupler in this case referring to the measurement device - made it so that IEM measurements have become widespread in a very short amount of time while still *somewhat* adhering to the established standard for measuring such devices. This widespread prevalence of high quality measurements is very useful for EQ purposes as well as for getting a rough idea of how an IEM will sound like.

This does not mean that measurements are infallible. Clone couplers are manufactured by unknown companies/groups in dubious conditions, and while they **might** comply with the relevant standards, they are not nearly as precise and/or as consistent as official gear. Not only that, **measurements might not match what the user/listener is hearing**. This topic is addressed later; for now, note that having a **proper seal is important for bass frequencies**. It is therefore important to understand the following rules in order to avoid problems with regards to FR graphs and measurements.

!!! warning Rules to consider
	- Measurements between different databases/couplers/standards cannot be mixed
	- Most couplers are only rated to 10kHz, therefore measurements should not be scrutinized >10kHz. High amplitude and narrow peaks/dips above 5kHz should also be ignored
	- Unit variation is a considerable factor, and should be accounted for 
	- Most couplers have a better seal with IEMs than IEMs with human ears, so proper fit/seal should be accounted for
	- Normalization should be accounted for, and should be modified to fit actual perception
	

Another aspect that should considered is compensation, which is used in two ways in the community. The first one uses compensation as a way to more easily see the error/deviation of an FR curve to another. Compensation in this manner improves "readability", and makes the EQ process easier.

->![Compensation of the Truthear Zero to the HarmanIE 2019 target, normalized at 1kHz](https://i.postimg.cc/FKBZ5DL4/Compensation-target.png){75%:75%}<-


The second way aims to correct/remove the errors introduced by the coupler. It can also be used to correct the coupler to a reference coupler, which can theoretically mean that measurements done on different couplers can be exchanged, provided they have been compensated properly. A full explanation of proper coupler compensation is beyond the scope of this guide; just know that it is complicated and requires a lot of data to work properly.

The 5128∆ project aims to create such compensations for various different databases on squig.link; more precisely, the compensations use Crinacle's coupler as a reference (more information about databases in the [Measurement databases and tools](https://rentry.co/IEM-EQ-Guide#measurement-databases-and-tools) section). Therefore, compensated measurements in databases that are a part of the 5128∆ project can be compared to those in Crinacle's database, and by extension to other 5128∆-compliant squig databases as well.


***
###Targets and preferences
While a lot of research in terms of sound preference has been done on loudspeakers and headphones, what has been done with IEMs has been less thorough. To better understand measurements, it is important to understand the intersectionality between preference, perceived accuracy, and anatomy. 

!!! info Oversimplified summary on the role of anatomy in terms of hearing and graphs
	1. Parts of the ear/body act like filters on the incoming audio signal for localization purposes. The biggest change is a total rise from 1.5kHz - 8kHz peaking at 3kHz
	2. The eardrum acts like a pressure detector measuring amplitude vs frequency. Therefore, the eardrum **does** perceive more 3kHz energy
	3. The brain expects these changes, and "cancels" out these filters. The resulting perceived sound is therefore the same as the original sound
	4. IEMs bypass many of those parts. They should therefore aim to have a resulting sound at the eardrum that includes every single expected changes

Grasping the above is important because it explains why IEM measurements and preference targets are **not** flat, and why they have a large rise after 1kHz (commonly referred to as **ear gain**). The couplers used for measurements aim to simulate the eardrum where resulting measurement will reflect the FR at the eardrum after having been influenced by parts of the body. These changes that the brain expects are called Head-Related Transfer Functions (HRTF), and it is this HRTF that is responsible for **sound localization**. Of course, different people will have different HRTFs due to differences in anatomy, and these differences become significant in certain frequency ranges. **While HRTF variation is quite high, there is still value in trying to find a preference target that sounds pleasing to the majority of people, which is why preference research is still ongoing**. The image below is commonly used to explain HRTF; only the concept of the rise and fall of the FR should be noted, as all the other minutiae is **not applicable to IEMs/headphones**.

->![Different changes caused by anatomy on incoming sound and FR. Ignore the angle of incidence part](https://i.postimg.cc/MpJRmYdG/HRTF.png){75%:75%}<-


!!! info Oversimplified summary on preference research
	- There is a significant correlation between preference and "neutrality"/accuracy in terms of sound reproduction
	- For loudspeakers, this means that a flat FR in anechoic conditions is preferable
	- Anechoic conditions are rarely found in everyday life, much less in studios. Most environments are semi-reflective, which introduces a downwards slope (or clockwise tilt) to the loudspeaker FR
	- IEM (and headphone) preference research usually aims to recreate similar timbre to that of optimal loudspeakers
	- Significant deviations in bass and treble is normal, and attributable to preference, hearing loss, and other factors
	- Small changes in FR (<3dB) over relatively small frequency ranges are hard to notice at best, and imperceivable at worst

The most "researched" target comes from Harman, and the latest iteration of their IEM target  is their Harman In-ear (HarmanIE) 2019v2 target. Despite being the most thoroughly researched target, there has been a lot of pushback against this target. Furthermore, many prominent reviewers have also included their own personal preference targets in their databases. Oftentimes these targets are either existing preference targets with tweaks (eg some variation on HarmanIE) or a mix of different FR parts of different IEMs they like (eg combining the bass of X IEM, mid range of Y IEM, and treble of Z IEM).

 The following is a brief summary of important preference target curves, as well as other curves that are **not based on preference**. There are also more informative and in-depth explanations of each of them in the [Measurement rigs, curves, and preference targets](https://rentry.co/IEM-EQ-Guide#measurement-rigs-curves-and-preference-targets) section.

!!! info Summary on various preference targets and other curves
	- Harman In-Ear (HarmanIE): Preference target by Harman for IEMs, based on past headphone and loudspeaker preference studies. The most validated target when it comes to targets with proper listening testing
	- Diffuse Field (DF): FR curve based on a completely "reverberant" listening condition (ie no energy emphasis on any direction). Used mainly as a reference curve, not a preference one
	- Etymotic Target: DF with an introduced "room tilt" based on outdated preference research (Consumer reports accuracy score) and the X-curve.
	- IEF 2020: Rudimentary target, mostly used to showcase "proper" HRTF features / ear gain. Bass is completely variable and up to taste, but is shown as flat for ease of use
	- IEF 2023: Target based on DF + tilt for IEC 60318-4 compliant rigs. Bass is also completely variable and up t taste
	- DF + tilt (Δ and JM-1): Popularized by the Headphone show and Crinacle. Essentially a DF curve with varying levels of tilt across the whole response. Used with preference bounds from Harman research, so there's not a singular target. Mostly used in the context of the B&K 5128 rig
	

***
###Human hearing
The human hearing mechanism is complex, and can only be summarized in an almost-vulgar, oversimplified manner. A few more of the relevant concepts to this guide are discussed.

!!! info Auditory masking
	->Auditory masking is a phenomena where a signal can affect the perception of another signal, usually one in proximity in terms of frequency. The following image illustrate the concept: a simple tone at one frequency (masker) can create a masking threshold on the surrounding frequency range whose shape and amplitude depends on the masker's own loudness. Any other signal that falls "under" the threshold is masked and inaudible.<-
->![Auditory masking](https://i.postimg.cc/rFPm0wjt/1706913375313.png){75%:75%}<-

!!! info Auditory memory
	->Auditory memory is **especially fragile and short** for humans. Relying entirely on memory when it comes to sound is not possible. It is therefore recommended to take notes of sound impressions, do ABX tests, and use measurements when it comes to describing and/or modifying IEMs and audio. **It doesn't mean that our hearing is useless**, but rather that it is **very fickle** and should be used as a "measuring tool" conservatively.<-

!!! info Equal-Loudness Contours
	->Equal-loudness contours show the required loudness level (in this case phons) for perceived equal loudness at various frequencies. The image below shows a rise in lower and higher frequencies in the curve, indicating that those regions need more phons in order to be perceived the same as the middle frequencies (ie human hearing is more sensitive to the middle frequency range). Another important aspect is how this rise in low/high frequencies **reduces** as SPL goes up, indicating that those regions require less phons in order to be perceived in equal loudness (ie human hearing becomes more sensitive to low/high frequency range with increases in listening volume). The effect over normal listening volumes is somewhat negligible, but it should still be considered throughout the guide.<-
->![Equal-Loudness Contours](https://i.postimg.cc/QMczSpWq/ELC.jpg){50%:50%}<-

!!! info Distortion and audibility
	->Distortion at a frequency increases/decreases when the amplitude at said frequency increases/decreases. Therefore, using EQ to boost the level of certain frequencies will also increase distortion. For IEMs, distortion is **negligible**, and even more so when considering distortion audibility with music. Only severe flaws with the IEM will lead to distortion being a relevant metric to consider.<-

!!! info Brain Burn-in
	->Brain burn-in refers to how our perception of sound can change with time as we get acclimated to a particular sound, and often occurs (in the context of IEMs) when the FR of a new IEM is significantly different than another one that was used before it. Preference for the new one is then taken to the extreme (positively or negatively), and this disparity in preference averages out and lessens with time as the user gets used to the sound presentation. For this guide where comparisons and constant subjective evaluation are needed, brain burn-in should be isolated and/or removed from the process.<-


***
###Equalizer basics
An equalizer (EQ) is a tool used to modify a signal, in this case an audio signal. In most cases, it is used as a way to change the amplitude for a specific frequency range/band. 

!!! info Four relevant filter parameters
	- Filter frequency, which dictates where the center of the filter is 
	- Filter quality/slope Q, which dictates what frequency range will be affected by the filter
	- Filter gain, which dictates the amplitude change, usually in dB
	- Filter type, which dictates how a filter behaves

There are different types of EQs, ranging from analog/digital EQs to parametric and graphic ones. Parametric EQs (PEQ) allow the user to change all three parameters, and provide a nice balance between being flexible, and being easy to modify and use. Unless stated otherwise, EQ will refer to PEQ for the rest of the guide. 

!!! warning EQ minimalism
	->The guide adheres to what I call **EQ minimalism**, which can be thought of as an approach to how EQ is used and developed. In this context, it means that ideally, an EQ preset should have **as few filters as possible**, for which each filter should have **low gain and Q values**. Aiming for few but broad changes is a good rule of thumb to follow; for more complex sections, deviation from this rule will be normal, even necessary.<-

	

The following image shows three FRs in three different colors. The red one is the base one with no filters, while the green and blue ones have different filters in order to showcase what each parameter does. The table includes the filters used in increasing order of frequency; the three left columns are for the blue FR, the three right columns for the green one.

->![Peak filters](https://i.postimg.cc/zfY5VpYw/EQ.png){75%:75%}<-
Frequency (Hz) | Gain (dB) | Q | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|:-:|:-:|
50 | 5 | 3 | 50 | 8 | 3 | 
1000 | 10 | 3 | 1000 | 10 | 1 |
9000 | 5 | 3 | 10000 | -10 | 4 | 
12000 | 5 | 3 |  |  | |


!!! info A few things to note
	- Increasing gain also widens the filter
	- Overlapping filters are summed. For the last two filters for the blue FR, the gain is 5 dB, but the overlap make the peaks land at around 7 dB
	- Negative gain is also possible. If two filters with the same frequency and Q values have "opposite" gain (eg 4 and -4 dB), they will be canceled
		

The only parameter that was not discussed is the filter type. In this guide, three types are used the most often.

!!! info Filter types
	1. Peak filters, which are the ones shown above
	2. Low-shelf filters, which boosts every frequency **below** the specified one (first row). The Q changes the shape of the filter 
	3. High-shelf filters, which boosts every frequency **above** the specified one (second row). The Q changes the shape of the filter 

->![Shelf filters](https://i.postimg.cc/bJmwQSQw/Shelves.png){75%:75%}<-
Frequency (Hz) | Gain (dB) | Q | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|:-:|:-:|
100 | 8 |  0.4| 100 | 8 | 0.707 | 
9000 | 5 | 1 | 9000 | -3 | 3 |

Shelf filters are useful for large changes for which precision is not needed, and are often used for customizing preference targets. For example, if the HarmanIE 2019 target sounded too bassy, simply adding a bass shelf filter with negative gain can be a simple yet effective fix. Same thing for treble: if there is too much or too little of it, use a high shelf filter to change the whole range. Shelf filters are generally used only for the two ends of the frequency range because of their nature, with **Q values of 0.5, 0.71, or 1**. More will be covered in relevant sections.

When using EQ, there is also preamplification that has to be taken into account. In the digital domain - computer, phone, etc - volume has an upper limit. Exceeding this limit results in [digital clipping](https://www.youtube.com/watch?v=W34SG5QO3Q0), which can happen when an EQ preset has large boosts. To avoid this, a preamp is used which reduces the digital volume. Preamp values should always be negative dB values, and should correspond to the highest amplitude change of the EQ preset. For example, taking the blue FR in the first image with peak filters, the preamp would have to be -10 dB. If only the last two filters are considered, then the preamp would have to be -7 dB; the preamp does not necessarily correspond to the highest gain value of a filter, **but rather the highest gain value overall, since summed filters can result in larger amplitudes/gain.**

***
###Tools and software

Now that the basics are done with, here is what's needed for using EQ.

####EQ App
The following link is useful for finding what EQ software is best for a specific OS or device. Do note that these are options that are compatible with AutoEQ; there are other software/hardware that also do EQ, such as VST plugins and more, but they might have different ways of calculating filter slopes. 
[Choosing an Equalizer app](https://github.com/jaakkopasanen/AutoEq/wiki/Choosing-an-Equalizer-App)
Do note that because of how the Android audio stack works, there are slight differences in how different apps implement their EQ. 
[Measurements of Wavelet and Poweramp EQ system-wide PEQ on Android](https://www.reddit.com/r/oratory1990/comments/10abm9k/measurements_of_wavelet_and_poweramp_eq/?rdt=48624)
For the rest of the guide, EqualizerAPO with the PeaceGUI will be used; differences between different apps that have PEQ are very minor. Depending on the complexity of how EQ is being used, additional software and tools might be required.

!!! note EqualizerAPO/PeaceGUI filter types
	->It is important to choose the appropriate filter types when using EQ. The image below contains the main ones; the difference between the shelf filters is that the one with "Q as slope" has adjustable Q values, while the one without has a default Q value of 0.707. Any other app not in the link above might have different filter types with different filter slope derivations that will not match what this guide uses (Robert Bristow-Johnson cookbook).<-
	
	->![Filter types in EqualizerAPO/PeaceGUI](https://i.postimg.cc/bJS532dZ/EQ-Sliders.png){40%:40%}<-
	
	

####Measurement databases and tools
For IEMs specifically, the most comprehensive database is a collection of individual databases (commonly referred to as squigs) all under the squiglink group. While it does contain the most measurements out of any other database, measurement quality can vary between different individual databases, and each individual might not have the same measurements as others. It also has many features such as an in-built Equalizer that provides immediate visual feedback, measurement importing, and more. There are instructions and explanations when clicking on the yellow question marks, one for navigation and the other for the 5128∆ project.
squig.link
Another notable database is from Crinacle, who has the **most extensive individual database**. The size of his database, as well as his B&K 5128 database have led to him being at the center of the 5128∆ project. 
crinacle.com
There are a few other individual databases that are also noteworthy:
[HypeTheSonics](https://www.hypethesonics.com/) (FR, distortion, noise attenuation, and more. Also has a B&K 5128 database)
[WoodenEars](https://www.woodenears.com/) (FR, distortion, and more. Also has a few B&K 5128 measurements)
[Rtings](rtings.com) (FR, distortion, and more)


***
***
##How to EQ
***
###Before getting started
The following sections are ordered in increasing levels of "difficulty", where later sections demand more theoretical and practical background knowledge, some of which **will either not be covered, or only very briefly**. As sections become more "difficult", less and less detailed instructions will be provided: the exercise will be left to the reader to try. A ranking system using five stars will be used to represent difficulty. Later sections usually provide better results, and include other novel ways of using EQ, but are far from being necessary to have a more enjoyable and pleasing sounding IEM; they also require much more time and effort.

Looking at the [Measurement rigs, curves, and preference targets](https://rentry.co/IEM-EQ-Guide#measurement-rigs-curves-and-preference-targets) section is also useful where using EQ to match FR to a target is necessary.

!!! info 
	- ( ): Very straight forward, no tweaking necessary
	- (\*): Small tweaks and changes necessary
	- (\*\*): Requires understanding and experience with EQ and one's preferences
	- (\*\*\*): Complex, requires all the above, and additional tools/software
	- (\*\*\*\*): Complex, requires all the above, listening training, and a good loudspeaker setup. Anything from here on out should be taken with a huge grain of salt
	- (\*\*\*\*\*): Too complex for the end user

***
###AutoEQ to targets ( )

!!! info
	->The simplest way to use EQ is by using AutoEQ, a project that aims to create automatic EQ presets using measurements and a specific target. There are various implementations of AutoEQ: in most cases, AutoEQ aims for the HarmanIE 2019 target. The following sections cover most cases, and also have pros/cons added.
	AutoEQ has a wiki that explains how it functions, but in short, it aims to match the FR of a model to a chosen target in the range of 20Hz to 10kHz. For the guide, both the lower and upper limits will be used.<-


####AutoEQ website
AutoEQ.app is a web application for the AutoEQ project, and has additional features for further tweaking and customization. 

1. Find your IEM model
2. Select the EQ app you plan on using
	2*. Under the Advanced option in the Profiles tab, select your target of choice
3. Download the file
4. Import/use the file in your EQ app of choice.


Pros | Cons | 
:-:|:-:|
Live demo'ing | Somewhat overwhelming/convoluted at first |
Customization available | Customization can lead to bad results |
Wide EQ app support | Somewhat limited model selection |



***
####EQ app 
Several EQ apps have also implemented the AutoEQ project, such as Poweramp on Android and PeaceGUI on Windows. In this case, simply pick the IEM model you have and the preset should apply automatically.

1. Find your IEM model and apply the preset

Pros | Cons | 
:-:|:-:|
Easy to use  | Somewhat limited model selection |
No additional installation |  |


***
####Squigs
Squig databases also have an Equalizer tab that implements AutoEQ. To use it, select the target that you want (under the FR graph), then select your IEM model in the Models tab, ensuring that only the chosen target and IEM are on the FR graph. In the Equalizer tab, find the AutoEQ option, adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project), generate the preset, then export it accordingly.

1. Select the wanted target under the FR graph
2. Select the IEM model in the Models tab, ensuring that only the chosen target and IEM are on the FR graph
3. Find the AutoEQ option in the Equalizer tab
4. Adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project)
5. Generate the preset
6. Export the preset accordingly

Pros | Cons | 
:-:|:-:|
Extensive selection of models and targets | Export only exports the filter values which need to be manually re-input in whatever EQ app is being used |
Customization available | Default range extends to 15kHz, far above what is recommended |
| | Can be inefficient since it only uses peak filters

***
####Wavelet
Wavelet is an Android app that has AutoEQ implementation and allows for system-wide equalization. 

1. Enable Wavelet
2. Choose your IEM model in the AutoEQ section
	2*. If needed, import presets made in squig.link or AutoEQ.app


Pros | Cons | 
:-:|:-:|
Easy to install and use  | No customization possible |
Presets available from other sources | Hassle when making a new preset |


***
***
###Custom EQ presets to targets with small tweaks (\*)
While AutoEQ is excellent at what it sets out to do, it is also possible to EQ to a target manually. Results will probably be very similar to AutoEQ, but creating the preset allows for possible customization filters, and in cases where concise EQ presets are needed (eg when wanting to input presets on other apps/devices), AutoEQ can be non-ideal.

The best way to go about this is through squig in the Equalizer tab. Unfortunately, there aren't any direct steps to making a custom preset. Choose an IEM model, a target, and try to match the IEM FR as close as possible. Also try to include filters that can be customized easily to fit your preferences. For example, adding a bass/low-shelf is useful for adjusting bass levels on the fly by simply changing the gain and/or frequency. The same can be done with a treble/high-shelf, or even peak filters.

!!! warning
	->This is **a learning phase** and will not necessarily produce better results than AutoEQ. What it does produce is a better understanding of EQ, which will be useful later. <-

Here is an example of the difference between AutoEQ and manual EQ when it comes to using EQ on a model (in this case the Salnotes Zero 2) to a target (HarmanIE 2019, ignore the "adjusted"). At this stage, normalization has to be factored in, which can be done through a specific frequency (eg normalizing at 1kHz will shift every FR up/down such that the loudness) or with loudness based on equal-loudness contours. For the image below, AutoEQ filter values are on the left, manual EQ on the right. 
 
->![AutoEQ vs manual EQ](https://i.postimg.cc/NMp0VHHW/Zero2.png){75%:75%}<-

Filter type | Frequency (Hz) | Gain (dB) | Q | Filter type | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
 PK | 23 | -2.4 | 1 | PK | 150 | -3 | 0.5 | 
 PK | 120 | 0.6 | 1.3 | PK | 1800 | -1.5 | 1.5 | 
 PK | 130 | -3.1 | 0.5 | PK | 5800 | 5.5 | 1.5 |
 PK | 300 | -0.5 | 1.4 |  | |  | |
 PK | 890 | 0.7 | 2 |  |  |  |  | 
 PK | 1700 | -1.6 | 1.2 |  |  |  |  |
 PK | 6300 | 4.3 | 0.9 |  |  |  |  | 
 PK | 6500 |  3.5 | 2 |  |  |  | |
 PK | 7700 | -5.7 | 2 |  |  |  | |

AutoEQ uses every filter that is provided to it; if there are 9 filters available in the Equalizer tab in a squig.link database, AutoEQ will use those 9 filters to make the IEM FR as close as possible to the target. This also means that there are usually a lot of "useless" filters, like the one at 300Hz that has a very low gain with a relatively high Q value. In squig databases, it is possible to reduce the number of filters, but it is not something that other AutoEQ implementation can necessarily do; when comparing to the manual EQ preset, there is a significant reduction in the number of filters. Even if two customization filters were added (a bass shelf and a treble shelf), it would still be much less than the AutoEQ preset.



Pros | Cons | 
:-:|:-:|
Customization available | Not straightforward |
Better understanding of EQ | More time consuming than just using AutoEQ |
| | Not necessarily better sounding or more efficient than AutoEQ |


***
***
###EQ for rough IEM emulation (\*)
So far, EQ was used to match an IEM's FR to a preference target (in most cases, HarmanIE 2019). It is also possible to roughly emulate another IEM through EQ. There are two methods to do so, both of which have already been covered previously: Squig AutoEQ and custom manual EQ. These will only yield rough approximations of another IEM.

Squig's AutoEQ implementation also allows for quick FR matching of one IEM's FR to another's. The steps are similar to using AutoEQ with targets.
select your IEM model and the one you want to emulate in the Models tab, ensuring that only their FRs are on the graphs (with **no targets**). In the Equalizer tab, find the AutoEQ option, adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project), generate the preset, then export it accordingly.

1. Select the IEM to emulate in the Models tab
2. Select the IEM model in the Models tab, ensuring that only the two chosen IEM FRs are in the graph
3. Find the AutoEQ option in the Equalizer tab and select the model to EQ
4. Adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project)
5. Generate the preset
6. Export the preset accordingly


The same can be achieved with creating a custom manual EQ preset as per the methodology outlined previously, and the same pros and cons apply. In both cases, the IEM FR that will emulated can simply be thought of as another target for which we're aiming for. 


***
***
###EQ to preference and context (\*\*)
Assuming that you're now familiar with EQ, it's time to dive into personal preference targets. While preference targets with small tweaks (eg an added bass or treble shelf) are a good way to start, they might not be the optimal sound that each person is looking for, which is why having an understanding of one's preferences is crucial. At this stage, the possibilities are endless which also means that everything can become overwhelming. What should be modified first? What if it doesn't sound good? What if X or Y is a mistake? 

Now that you are hopefully more familiar with your preferences as well as EQ, let's add a few rules and important notes.

!!! warning More rules 
	- FR should be interpreted holistically where changes in one range can impart perceptual changes in another.
	- Changes in on frequency range (eg bass) can be perceived as either a direct change in the targeted region, or a change everywhere else
		- Eg. a reduction in bass can be thought of as just that, or as a boost everywhere else except the bass region
	- Human hearing is more sensitive to peaks than dips in FR
	- The debate between accuracy and enjoyment should be ignored in favor of what sounds good to you
	- Listening tests are **necessary**. Overreliance on graphs can lead to bad results
	- Experiment with the filter types and parameters while still adhering to EQ minimalism to achieve different results
	

There are two aspects to consider: preference and context. Preference as described above might not match a specific target, and should therefore be **explored through experimentation**. Context refers to everything from the audio to the listening environment and how the IEM is being used. Factors to consider for both are numerous, such music library which can have inconsistent mixing and mastering between different genres, releases, discographies, and even within the same project, and environmental noise, which might necessitate more volume for certain frequency ranges. 

!!! info Let's divide the frequency range into three distinct regions
	1. Bass 
		- Sub bass (20Hz - 80Hz)
		- Mid bass (80Hz - 300Hz)
	2. Mid range
		- Lower mids (300Hz - 1kHz)
		- Upper mids (1kHz - 4kHz)
	3. Treble 
		- Treble (4kHz - 10kHz)
		- Upper treble (10kHz - 20kHz)


***
####Bass
Fortunately for IEMs, bass output is usually not a problem provided there's a good seal between the canal and IEM. The differences in bass between different IEMs can be simplified to two aspects that can be tweaked to preference. 

!!! info Bass 
	- Bass level, which refers to the overall average bass response loudness relative to the rest of the response. It can be high, low, or anything in between
	- Bass shape, which refers to the relative balance between sub and mid bass. Useful for different bass "presentations"
		1. Bass glide: Generally refers to bass that has a "good balance" between sub and mid bass. Can be a a straight line as shown, or more contoured
		2. Flat bass: Equal levels of sub and mid bass
		3. "Subwoofer" / Tucked bass: Heavy emphasis on sub bass, with much lower relative mid bass level
		4. Rolled off: Emphasis on mid bass, with sub bass levels that are decreasing and lower than mid bass

The following pic shows the different bass shapes in order. Note that this is just a very small sample of what bass can look like on IEMs. The number of variations and small tweaks that are possible can also muddy the waters and create differently perceived bass presentations despite looking mostly similar on graphs.

->![Different bass shapes (in order and normalized at 1kHz)](https://i.postimg.cc/Pq9fBdpX/Bass.png){75%:75%}<-

Bass is the most variable range in terms of preference, so experimenting with not only different shapes but also levels is really important. Bass is also highly variable depending on the audio signal / music you're listening to. For example, acoustic-oriented music will not have as much bass as hip hop, or electronic music. The goal is to find the right balance between your preference and what you're listening to. 

!!! warning EQ based on genres
	->Whether EQ should be suited to match one's library or simply used to correct the IEM's FR has been debated ad nauseam. For this guide, do whatever suits you in terms of accessibility, ease of use, and sound preference.<-

***
####Mid range
Mid range is a tough region to tweak because it is wide in range and also contains a lot of the audio content. Most if not all instruments and components in music have some part of their frequency content in the mid range: everything from bass instruments to high pitched percussions are therefore affected by changes in the mid range. As with bass, mid range can be simplified into three aspects.


!!! info Mid range
	- Ear gain elevation, which refers to how high/low the ear gain is **relative to the rest of the response**
	- Ear gain location, which refers to where the maximum peak of the ear gain is situated at. Common location is at 3kHz
	- Mid range shape, which refers to the relative balance between lower and upper mids. Useful for changing note weight / brightness / warmth / etc.
		1. Recessed mids: Low levels of lower mids, leading to the mid range sounding "thin" and "hollow"
		2. Forward mids: **Usually** refers to high levels of upper mids and/or ear gain.
		3. Low ear gain: Low levels of mids, usually above 1kHz, relative to the rest of the response
		4. Warm/thick mids: High levels of lower mids, leading to a more "full-bodied" mid range and more "warmth".

Mid range has a lot of variation between different IEMs, so much so that it becomes rather hard to demonstrate these different aspects independently. Aiming for a similar mid range as ones found in preference targets should be the goal, but don't be afraid to make big changes if it sounds better to you. The following pics shows different mid range responses and how variable they can also be. Also notice how different normalization can skew visual perception of mid range, which is why listening to the EQ changes is recommended.

->![Different mid range responses (normalized at 1kHz)](https://i.postimg.cc/VvV30YxS/mids-1khz.png){49%:49%} ![Different mid range responses (normalized at 300Hz)](https://i.postimg.cc/WpYRHnd2/mids-300hz.png){49%:49%}<-


***
####Treble
Treble is the trickiest and most difficult region to tweak because of measurement variance, insertion depth, HRTF differences, and more. At this stage, only two aspects are considered.

!!! info Treble
	- Treble level, which refers to the level of treble relative to the rest of the response
	- Treble peaky-ness, which refers to the presence and/or absence of large, noticeable peaks

Doing any changes in treble should, in most cases, only rely on listening tests and not graphs. If there is a treble flaw attributable to the IEM, only then should EQ be considered. For now, treble modifications should optimally only involve shelf filters and/or low-Q/wide peak filters to change treble and upper treble levels. Depending on taste and the IEM's FR, boosting or reducing with these filters should improve overall tonal balance without much effort. 

In the case where there is an obvious peak that is sibilant and/or annoying, there are a few steps to take.

!!! info Fixing treble peaks
	1. Confirm that a peak is actually present in the IEM's FR and that it is not a peak that is present in the audio content
	2. Determine whether or not this peak has a noticeable, negative impact; continue if it does
	3. Locate the peak using music, pink noise, or a tone generator / sine sweep. A tone generator/sweep can also work, but should be done even **more critically as human hearing is not good at detecting perceived loudness** with sine signals. **Only use it for very high amplitude peaks**
	4. Use a relatively sharp filter (Q > 4) and varying levels of negative gain, ensuring that the peak is minimized without encroaching on the surrounding frequency range (ie reduced until no longer bothersome) by using music and/or pink noise

***
####Adding everything together
As mentioned previously, FR should be interpreted holistically. It is therefore wrong to think that because two IEMs have the same bass response, they will sound the same in terms of bass. Every single region affects one another, and it is hard to completely separate each region, especially when it comes music. It is therefore important to test in various ways. Keeping two regions locked and modifying one is a logical approach, but locking one and modifying the other two regions can also lead to interesting and unexpected results. Mix and match and try to experience many different FRs.

!!! warning
	->Listening to each frequency region independently does not reflect how music is heard. Changes in FR should be done with the knowledge that any change in any of the regions will also affect the perception of the rest of the response. At this stage, **experiment and try everything you can**.<-

In the end, the final obtained FR should be ideal to your preferences, and while large deviations in bass and treble regions are normal, the mid range should still have a generally "normal" profile (ie have some semblance of ear gain). The following collection of images are some commonly seen and liked "types" of FR with small descriptions of their tuning; use them as a template and/or mix and match different parts. 

->![Normal ear gain with a bass boost (glide)](https://i.postimg.cc/NFhCkjQZ/zero2.png){33%:33%} ![Normal ear gain with flat bass](https://i.postimg.cc/NjbVvtxr/Proxima.png){33%:33%} ![Sub bass boost with very little to no ear gain](https://i.postimg.cc/15hbpJt4/MEST2.png){33%:33%}<-

->![Forward mids and ear gain with bass boost; emphasis on mid bass by rolling off the sub bass](https://i.postimg.cc/8zT3YcLS/Origin.png){33%:33%} ![Sub bass boost followed by a mid bass dip with forward ear gain](https://i.postimg.cc/bJSFntfQ/Variations.png){33%:33%} ![Bass boost (glide) with low ear gain except for a 4.5kHz peak](https://i.postimg.cc/FFJ2d2h2/CRA.png){33%:33%}<-

->![Somewhat flat or rolled off bass with a lot of lower mids (warmth), with low plateau ear gain](https://i.postimg.cc/KYHH45wG/Andro.png){33%:33%} ![Bass boost (glide) with moderate plateau ear gain](https://i.postimg.cc/5NBTpLYg/P5.png){33%:33%} ![Mostly sub bass boost with moderate ear gain](https://i.postimg.cc/Bv6zqzh7/5EST.png){33%:33%}<-


***
####Noise and environment
Depending on the listening environment, more changes might be useful. There are a lot of factors at play here, such as whether or not the IEM being used has ANC, what the listening volume is currently, what the noise attenuation profile of the IEM is, how loud the surroundings are, if there's a need to be aware of voices or signals, etc. Ultimately, correcting for these factors requires experimentation just like what was discussed previously. A few rules can be used.

!!! info Tips and common scenarios
	- Research suggests that in loud environments, a boost in bass is preferred. Most probably depends on the its noise attenuation profile
	- Based on equal-loudness contours, EQ might need to be adjusted to suit a specific listening volume
	- Good ANC will cancel out bass more effectively than passive isolation, but will also struggle with frequencies above 1kHz


***
***
###Personal measurements (\*\*\*)
Up to this point, EQ was used with measurements provided in different databases, and while some of them are available with the 5128∆ project that allows for cross database comparisons, unit variation is still a very big factor that should be addressed, especially if an IEM and/or brand are known for having mediocre quality control. To remedy this problem as well as a few others, personal measurements should be used. There are three ways in which measuring your own set can help when using EQ.

For the rest of this section, it is assumed that the measurement rig is an IEC-60318-4 compliant occluded ear simulator, aka a 711 coupler, and that all measurements of an IEM are done with the same ear tips unless stated otherwise. 

!!! warning Before measuring
	->If possible, listen to the IEMs before doing any measurements as they can introduce biases and placebo. The measurement rig is **much more sensitive** than human hearing, and so not all "errors" will be audible, unless of course you do measurements first and fool yourself into hearing a problem where there aren't any.<-

***
####Unit variation
Personal measurements are useful for determining whether or not a particular unit of an IEM is faulty or not. Not only that, it also serves as a useful indicator that some part of the IEM might require cleaning or fixing. For example, clogged filters, or debris in vents can drastically change the sound of an IEM, even if it measured fine out of the box.

!!! info Unit variation issues
	- While measurements between different measurement rigs shouldn't be compared, it is useful in this case for identifying large deviations indicative of quality control issues or flaws in the IEM
	- IEMs with large unit variation should also be checked quickly for potential distortion issues
	- For brands with a history of silent revisions, measurements are necessary
	- Any failure due to use and fatigue, like filters getting clogged, can change the FR

Unit variation is **usually not a major issue**, but when it is, it can be confusing when trying to EQ. If a unit has significant variation that is **not easily fixable** through EQ (eg having a substantial drop/boost in the bass region), then it is better to simply return it rather than salvage it. These differences will be perceived by the listener, but even with seemingly large deviations in measurements, human hearing is not as sensitive and can be **easily fooled** by different biases.

The following image shows three different samples of the same IEM. Unit variation can manifest itself as either poor QC, revisions, or pre-production units. The differences shown are relatively significant, and are located in a region that seems to be polarizing considering how the correct final version has the least energy there. 

->![Unit variation across three units of an IEM](https://i.postimg.cc/8CYjcH9H/Variationsunit.png){75%:75%}<-

The next one shows an example of an IEM that has somehow passed the manufacturers quality control stage. Notice how low in amplitude the whole range below 1 kHz is on the defective model; this large discrepancy would require filters with very high gain, and subsequently high preamp negative gain. Not ideal, and not worth using EQ to fix it.

->![Defective unit](https://i.postimg.cc/V6cMz7FF/graph.png){75%:75%}<-

For your own measurements, check to see if there are significant deviations, and if there are, simply EQ the unit to the desired FR following the guide. Re-measure your unit with EQ applied to see if the deviations have actually been removed and listen for any possible (albeit very rare) signs of distortion or other artefacts.

***
####Channel Matching
Depending on quality control...quality, some IEMs and individual units can have significant channel imbalances. Depending on the frequency range being affected and the volume difference, the imbalance can be audible: for most manufacturers, a deviation of 1dB is generally considered as acceptable. Fixing these imbalances relies on the same steps and ideas as previous sections, but requires separate and independent channel EQ.

!!! info Measuring channel matching
	1. Calibrate the coupler and ensure that there are no audio modifications (eg EQ)
	2. Measure one side of the IEM, taking note of how deep it was inserted and of the volume at which it was measured at
	3. Measure the other side, making sure that the volume and the insertion depth is **the same** (ie have the same resonance peak frequency)
	4. If needed, re-measure any side if there is a leak, a mismatched resonance peak, or error in volume

If both sides have been measured to have the same resonance peak location and the same loudness, then comparisons and conclusions can be made between the two sides. The same rules as before apply here.

!!! info Fixing channel imbalances
	- Before even attempting to EQ, **listen** to the IEMs and determine if there is any discernible differences between channels. This step should optimally be done **before measuring** the IEMs as this can introduce bias and placebo
	- If there are differences, **listen** and try to identify the regions where they are situated. Music should be avoided in favor of pink noise and/or sine sweeps
	- The measurement should then be used with relation to what was heard
	- Any deviation below 1dB and/or around the resonance frequency should be ignored
	- Use necessary filters to fix the imbalances while constantly comparing with pink noise and/or sine sweeps
	- If there is a consistent difference throughout the whole frequency range, use a channel specific preamp or limiter to adjust volume on one side

The image shows two IEM units, for which both their channels have been measured. For the Hola, this particular unit displays a consistent difference of around 1dB between channels; whether this is audible or not has to be determined through listening tests. If there's a need for correction, a simple preamp (or peak/shelf filter for focusing on a frequency range) can be used. The G10 also has slight differences, but because they are so narrow, they will most likely not be noticeable.

->![Two IEMs with acceptable channel matching](https://i.postimg.cc/pTncQMz9/Imbalance.png){75%:75%}<-

The following images shows an IEM for which there is a channel imbalance in the ear gain region. At first glance, the small peaks are not only different in level,  but also not aligned between the two sides. Fixing this with the left image isn't so straightforward; the second image, with side 1 being compensated to side 2 offers a better look at what the differences are, and how to fix them.

->![Uncompensated graph](https://i.postimg.cc/nzDrWpDv/channel.png){49%:49%} ![Compensated graph](https://i.postimg.cc/vTyYS9Ms/Compens.png){49%:49%}<-

!!! warning IEM or hearing?
	->It is important to note that while channel imbalances covered so far only refer to those caused by the IEMs themselves, **your hearing can also be responsible**. High frequency roll-off is particularly frequent as age progresses, and slight sealing issues can also cause differences in bass. It's why **listening tests are always recommended** and why measurements might not be enough to cover all bases. If imbalances occurs consistently in the same regions, it is safe to assume they are hearing related. For hearing-related imbalances, use a tone generator and sine sweeps, and use EQ until perceived sound is centered (ie sounds like mono).<-


***
####Insertion depth and ear tips
Insertion depth changes not only the frequency of the canal resonance peak, but also affects the surrounding frequency ranges, and oftentimes significantly. While previously established rules state that measurements shouldn't be scrutinized above 10kHz, there is still some use in looking at insertion depth profiles of an IEM in order to not only see how it reacts to different coupling scenarios, but also to find a match for your own personal experience.

!!! warning
	->A tube resonance is created when IEMs seal the canal/coupler, and changes in frequency (6kHz - 12kHz) depending on insertion depth. Commonly referred to as canal resonance, or length mode, they should **only be modified based on listening tests, and not through graphs**.<-

The following image is an extreme example of how insertion depth can affect FR. As the insertion depth changes, so do the surrounding frequencies' levels. Depending on the IEM's shape, intended insertion depth, and the ear tips being used, insertion depth location can shift drastically; not only that, there can also be damping, from the ear canal and/or IEM in that region, which can affect both the amplitude and Q of the resonance peak. It is therefore useful to have insertion depth profile done through your own measurement rig.
->![Etymotic ER2XR insertion depth profile](https://i.postimg.cc/pX7xRRC7/Insertion-depth.png){75%:75%}<-


The following images shows possible FR changes attributable to ear tips. Ear tips usually influence the bass region because of seal, and treble because of insertion depth as well as other reasons outside the scope of this guide. Assuming proper seal, the bass factor can be ignored, leaving only the treble as being an affected factor. Depending on the shape and size of the ear tip, the resonance peak frequency can shift considerably. The image however does show changes despite them having the same resonance peak frequency; while it is usually recommended not to scrutinize measurements past 10kHz, it is an interesting thing to note that ear tips can change upper treble response, usually in the form of damping.

->![FR changes caused by different ear tips](https://i.postimg.cc/rw0GsmwX/Tips.png){75%:75%}<-

!!! info Rules based on insertion depth changes and ear tips
	- Assuming the location of the canal resonance peak has already been found, measurement at said location should be obtained for the IEM that will be recipient to the EQ
	- Measurements should be done with the same ear tips that will be used for actual listening
	- Check if the resonance peak is audible: if so, follow previous steps for fixing treble peaks
	- Experiment with different insertion depth in case treble is not up to preference

***
***
###EQ refinement (\*\*\*\*)
At this stage, EQ is a tool that with which you are intimately familiar with, FR graphs are readable, decipherable, and hopefully enough to explain your perception of sound, and preferences have been found and more-or-less perfected. While measurements will still be useful, **listening critically** will be the main way of knowing what to change. 

EQ refinement in this context refers to large and complex changes in the treble response for **optimal timbre accuracy**, and also intentional deviations colorations to improve "intangibles/technicalities". It is assumed that you have access to a good "reference" loudspeaker setup. This phase is inherently very personalized, and will require considerably more experimentation, trial and error, and time. Note that the tips provided from here on out will be based on what has worked okay-ish for **me**. Feel free to ignore, or even go against what is written.


***
####Measurements and misinterpretation
At this stage, it is important to be more nuanced when it comes to reading measurements. While certain factors such as insertion depth and unit variation were discussed, there are other somewhat more complex issues that make measurements not as ideal as they seem to be when it comes to representing individual sound perception.


#####HRTF and individual variation

The first main issue arises from **HRTF differences** between individuals. Starting from around 2kHz, the variation in HRTF becomes quite significant, and increases in magnitude proportionally with frequency. For example, looking at the SADIE II database of DFHRTF measurements done at the blocked ear  canal, the patterns described previously can be seen clearly, where amplitude differences of up to 20 dB can be observed above 10 kHz (image on the left). Note that since the HRTF database was measured at the blocked ear canal, it does not include the canal transfer function and potential variations in the frequency range it affects; the variations are therefore even more pronounced and can go down as low ass 1 kHz. What this means is that even if IEMs produced the same FR at the eardrum of two separate people, their perception of the produced sound **will be different** (assuming said perception can be measured, quantified, and compared), despite having the same response at the eardrum. The image on the right shows open and blocked canal measurements of 40 HRTFs for a frontal source: while not directly comparable to the DFHRTF image from the SADIE II database, it does still show the very large deviations in HRTF above 1 kHz depending on the individual. 


->![SADIE II DFHRTF at the blocked ear canal for 40 people](https://i.postimg.cc/KjC6yPq3/SADIE-DFHRTF.png){49%:49%} ![HRTF at the open and blocked ear canal for a frontal source ](https://i.postimg.cc/D0S9DjgK/Moller-HRTf.png){49%:49%}<-


#####Measurement system accuracy

The second issue comes from the inherent **differences in acoustic impedance** between not only the **measurement system and the listener**, but also between **different measurement system standards**. While more details can be found in the [Measurement rigs, curves, and preference targets](https://rentry.co/IEM-EQ-Guide#measurement-rigs-curves-and-preference-targets) section, it is worth summarizing the differences between the "711" (IEC 60318-4) and "5128" (ITU-T P.57/58 Type 4.3) measurement databases as they are the most prevalent right now. The "old" standard is the most commonly used standard, and has extensive data, while the new standard has a much lesser amount of data, but is more "accurate" then the former.

The differences between the both of them can be boiled down to a difference in acoustic impedance, with the newer standard being more accurate to the human population (ie matching the mean better). For expected changes when it comes to graphs, there are a three main places to look at: the bass region below ~150 Hz and above to 1 kHz, the frequency range between 1 kHz and 5 kHz, and the rest above 5 kHz. The former is very important, with 5128 measurements showing clear differences in bass. There are two main changes; the first one relates to overall bass level, where 711 measurements tend to overexaggerate amplitude below 150 Hz, and the second one relates to the relative difference between IEM models with different driver configuration, which explains the commonly talked about "BA bass" (see image below). These differences make the 5128 measurements generally more reliable when it comes to representing what a listener is hearing. As for the latter place, the increased accuracy is somewhat useful, although precautions have to be put in place. From 1 kHz to 5 kHz, the new standard adheres to the mean acoustic impedance better than the old one, although the differences don't seem to be noticeable and/or consistent. For the last region above 5 kHz, the newer standard is much better than the old one, but is not nearly as useful, since HRTF, insertion depth, and other factors result in wildly different responses away from the mean.

->![711 and 5128 measurements of the Etymotic ER2XR](https://i.postimg.cc/nzLgzyJz/5128vs711.png)<-

The image above includes a 711 and 5128 measurement of the Etymotic ER2XR with somewhat similar coupler resonances at around 13.5 kHz. All the differences mentioned previously are visible: the 5128 measurement has noticeably less bass and mid range compared to the 711 and relative to the rest of the FR, the more accurate acoustic impedance from 1-5 kHz doesn't seem to result in as substantial of changes, and the treble above 5 kHz looks drastically different despite the very close coupler resonance. It is important to note that direct comparisons are **not valid**, and that notions conceived for 711 measurements (eg bass to ear gain balance, bass levels relative to FR, etc) **cannot be applied for 5128 measurements**. 

->![Measurements of the Tanchjim Oxygen and Kiwi Ears Orchestra on a 5128 measurement system](https://i.postimg.cc/NfNbDqLL/5128bass.png){49%:49%} ![Measurements of the Tanchjim Oxygen and Kiwi Ears Orchestra on a IEC 60318-4 compliant (711) measurement system](https://i.postimg.cc/DyfB1yvt/711Bass.png){49%:49%}<-

The two images above highlight the noticeable difference in leakage tolerance, the right being measurements done on the 5128, and the left the 711 (both normalized at 1 kHz). For high output acoustic impedance drivers (in this case the balanced armatures in the Orchestra), leakage plays a bigger role, and so the difference in bass compared to an IEM with a relatively low output acoustic impedance (in this case the dynamic driver in the Oxygen) will be more pronounced on 5128 measurements compared to 711 ones. All of this is important to consider because 5128 measurements are done with an attached pinna which is much harder to have a proper seal with compared to 711 measurements which are taken with a bare coupler (ie a straight metal tube which allows for much better seal).

Unfortunately, most FR databases of IEMs are currently being done with the old standard, while ones done on the new standard are limited in scope. It is therefore important to understand the differences discussed previously, and how they can muddy the waters when it comes to reading FR measurements and correlating them with personal experience. 


#####IEM and canal interactions
The third reason is related to how FR can vary depending on how an IEM couples and interacts with the ear canal and eardrum. When an IEM is inserted into the ear canal, the transfer function between the IEM and the eardrum can create meaningful peaks throughout the treble range, and for which the amplitude, location, Q, and number of peaks varies considerably with the individual, and depends on many factors, such as ear canal geometry. The images below show such potential transfer functions; notice the variance in terms of peak amplitude and Q. The canal transfer function is highly variable depending on the individual, and the peaks shown on measurements can also be a result of either insertion, driver resonances, or other factors, for which the transfer function will inevitably be masked or mixed with said variables. Furthermore, some IEMs employ forms of damping that try to mitigate such resonances. The interaction between the IEM and the canal of a person is therefore not shown accurately on 711 measurements, where canal geometry is not present, and even on 5128 measurements, the peaks in response will shift around depending on the individual.


->![Simulated ear canal transfer function  for both a KEMAR rig and human ear geometries from the IHA database](https://i.postimg.cc/65LvsWDf/Canal-Transfer-functions.png){53%:53%} ![Ear canal transfer functions obtained on various humans](https://i.postimg.cc/W1NJsRVL/Oksanen.png){20%:20%}<-


***
!!! info Summary of measurement misinterpretation
	1. HRTF differences above 1 kHz will result in wildly different perception of sound
	2. Acoustic impedance differences and deviations of measurement systems from population averages means that measurement don't necessarily reflect what is being heard for an individual
	3. IEMs will cause treble changes which depend on personal anatomy, and are not easily identifiable in measurements


These reasons are why measurements take a back seat at this phase. Individual anatomy creates very large differences between perceived and measured response, so much so that using measurements without understanding such nuances can be detrimental. The main points to remember are the first and third ones; for the second point, points 1 and 3 are most probably bigger and more significant above 5 kHz. Change in acoustic impedances between 1 kHz to 5 kHz is relatively small and shouldn't matter much as long as measurements are used relative to your perception (not as an absolute metric), while the difference in acoustic impedance under 100 Hz is somewhat overshadowed by personal bass preference. It is therefore **important to use measurements and compare them relative to what we personally hear, and to not be afraid to ignore or even "go against" them when they deviate too much**. 

***
####Easy way out
There is a method that is considerably easier and arguably more accessible than what follows, but it does require 5128 measurements and will most likely provide less personalized results. While large scale preference targets as seen with Harman would be ideal, there are no current formal studies done with the 5128. Instead, the best option as of now (in my opinion) is using derived/calculated targets using population average measurements. More details are in the [Targets and Preferences](https://rentry.co/IEM-EQ-Guide/#targets-and-preferences) section. A mix of the tips given previously can be used; see if the measurements correlate well with personal perception, then ignore or use the parts that match well.


***
####Loudspeakers as a reference
Before going any further, having a reference loudspeaker setup is necessary; at the very least, having heard one is crucial. The reason is linked to how HRTF ties in with listening to IEMs: since IEMs bypass most of the ear as well as the rest of the body, they have to **emulate those transfer functions**. As such, IEMs and their tuners have to **guess** the correct HRTF (ie guess the correct ear gain level, location, and features). 

For loudspeakers, the incoming sound is influenced by the listener's HRTF already, and therefore only the "raw" FR of the loudspeaker is considered. As mentioned in the [Targets and Preferences](https://rentry.co/IEM-EQ-Guide/#targets-and-preferences), IEMs and headphones should try to recreate similar **timbre** as heard with loudspeakers. Timbre in this case refers to overall tonal balance between bass, mid range, and treble, as well as conformity with your HRTF. Remember, the response at your eardrum from loudspeakers **will have your own HRTF contributions, while IEMs can only guess, and often times, incorrectly**.

It might seem logical to reason that because the brain applies the inverse of the HRTF to the incoming sound and therefore perceives sound from a loudspeaker as flat (since the HRTF contribution matches exactly to what the brain expects), using something like a tone generator and doing sine sweeps would be optimal. If the brain ultimately perceives the flat response of a loudspeaker, shouldn't we EQ the IEM's response to be perceived as flat as well? Wouldn't that mean that whatever HRTF contributions from the IEM have been removed and replaced with the correct response, resulting in perceived flatness?

Unfortunately, **the human hearing mechanism is not a simple pressure detector**. While the eardrum is one, the overall human hearing mechanism has to account for localization: HRTF aids in **sound localization** and so simply accounting for amplitude isn't enough for achieving accurate timbre. If loudspeakers and IEMs functioned the same in terms of sound localization, then the previous assumption would be true. However, IEMs and loudspeakers (or other localizable sound sources) are inherently different audio reproduction systems, and do not have the same "spatial rendering" features as loudspeakers.


!!! note Summary of loudspeakers
	->Loudspeakers, by design, create an eardrum response that has the correct HRTF contributions. The brain then goes through a **localization process** which transmits spatial perception through hearing. The brain then applies the inverse filters to the HRTF response as it expects; the resulting perceived sound is therefore flat/neutral with no coloration. In the end, two pieces of information are obtained: the spatial cues of the loudspeakers and room, and the spectral and tonal balance of the loudspeakers and room. For IEMs, both the HRTF contributions and localization process from listening with loudspeakers are incorrect and incompatible. Another method has to be used.<-

Loudspeakers are still useful because they are a reference point for accurate timbre as explained previously. The problem is that trying to compare timbre on both system is very difficult because of auditory memory, different spatial perception, isolation, etc. Despite these drawbacks, comparison between the two can still be useful, albeit very time demanding. The aim here should be to attain something as similar as possible, since the difference in sound field and perception will inevitably make IEMs have less accurate perceived timbre. Note that the following methodology can also be used to emulate other IEMs, although having both IEMs in hand is necessary. 

!!! info Comparison between loudspeakers and IEMs for timbral accuracy
	- Only compare IEMs to loudspeakers in the listening position
	- A/B test as fast as possible. Blind A/B/X testing for preference is also recommended
	- It is also possible to use headphones and measure/correct their response at the blocked canal and using those as the reference
	1. Examine overall tonal balance when comparing, mainly concentrating on the mid range and treble regions
	2. Adjust treble using broadband filters. Aim for a similar balance, paying attention to the overall treble level
	3. Use pink noise or music to compare timbre. **Do not use sine sweeps or tone generators**
	4. Adjust using fine filters. Eliminate differences, both peaks and dips, in perceived treble response	
	5. Move on to the mid range when treble correction is done
	6. Adjust bass level to preference



!!! warning HRTF or treble linearity
	->While replicating one's HRTF seems to be the optimal end goal based on the theory presented above, other studies have shown mixed results concerning personal vs general HRTF matching with relation to preference and localization. The idea of trying to match your HRTF will be kept for the rest of the guide and mentioned as **perceived flatness**, but it is important to note that a **measured** (ie not perceived) treble response could very well also be a good goal to aim for.<-

***
####Treble changes
The previous rules were very general and provide very little guidance on how to actually finetune treble response, which is arguably the most important frequency range in that it influences everything else due to the nature of musical content and harmonics. The following steps are **very crude**, and while the end goal is to try and match the resulting FR to your expected HRTF as described previously, **none of the steps outlined here will be accurate in any way; only preference and rough matching to loudspeaker timbre are considered**.

The first step from before was to adjust the overall level of the treble, with either low Q peak filters or shelf filters. When the overall level has been adjusted, more precise changes can be done. At this stage, using pink noise is recommended over music as treble content will be consistently present at all times. It is important to **do A/B testing when comparing loudspeaker and IEM perception at this stage** and to **not let yourself get accustomed to IEM presentation**. Frequent resting is also recommended.

Fixing dips in the response is the hardest part, as dips are harder to detect than peaks. A good way to start would be to start at a relatively high frequency, and to add a sharp peak filter with a relatively moderate gain. Then, shift the filter by an increment of your choosing. For example, you could start at 5 kHz, with a filter of Q=5 and gain of 5 dB, and then use 300 Hz increments. Check to see if the boost is properly balanced out by the rest of the pink noise, and compare thoroughly with loudspeakers. **Make sure that you take proper breaks to remove potential biases**. It is particularly difficult to judge this change properly; a lot of times, these types of small boosts will be preferred on the sole basis of being perceived as bringing more "detail", hence why having a reference (ie loudspeakers) is so important. 

By "sweeping" the frequency range this way, the chance of detecting a particular perceived dip should be much higher at the cost of being a very demanding, fatiguing, and time-consuming - with all the breaks and "brain resets" necessary for proper evaluation - task. Adjustments to both Q, increment, and gain should be examined and tested thoroughly in an iterative manner until the most optimal timbral accuracy is achieved. Subsequent testing (A/B/X or otherwise) between different EQ presets should also be performed while also taking into consideration rest, hearing fatigue, and brain burn-in. 

The main issue with this method is the holistic nature of FR perception, and how the changes that were previously discussed do not consider it. For example, adjusting the bass as the last step - after everything in the treble has been corrected - might alter perception of treble and mid range; the same can be said about changes in the treble that induce perceptual changes in the bass or mid range bands. The whole methodology is therefore akin to a cat-and-mouse game, where constant changes require additional changes which require additional changes ad infinitum. 

Two changes to the methodology can be made to mitigate the issue: adding more simultaneous variables (eg using two filters for the sweep method), or changing the parameters of the variable (eg changing the Q of the second filter, or using non-linear frequency increases for the filters). Unfortunately, there is no solution that I'm aware of that aims to tackle the issue and does so in an easy, simple, and efficient manner. This stage requires a lot of time and will most likely result in frustration and tiredness rather than a better EQ preset. 



***
####Intangibles and technicalities
"Intangibles", or "technicalities", are subjective terms used to describe certain characteristics of sound that an individual is perceiving that are not readily readable in FR measurements. Terms like "soundstage", "resolution", "dynamics", and "speed" are widely used, but there is no strict definition because they are based mainly on individual perception. While there seems to be a common consensus about what these terms mean, they are not remotely close to being consistent from one person to another, from one IEM to another, and from one moment to another. Therefore, there is no guarantee that anything that follows will result in better perceived technicalities, and it bears repeating that **sound perception is deceptively fallible**.

One relatively common perspective on these technicalities is that they are either "hidden" in FR graphs, or that they are **subtle colorations** of FR (large enough to be noticeable, yet small enough to not be tonally off-putting). The former explanation makes sense when considering all the reasons why measurements can be inaccurate, while the second one is plausible but would need some sort of testing to be certain.

For any following tips and tricks, use very small FR increases; while it was previously mentioned that human hearing is bad at detecting peaks and dips lower than 3 dB, this only applies to relatively high Q features. Most of the changes that should be applied should be started at very low amplitudes since the goal is to **alter perception of technicalities while influencing overall tonal balance as little as possible**.

#####Bass "quality"
Whether referencing "texture", "impact", or any other metric, bass quality is often presumed to be wholly unrelated to FR since attempts at improving it through EQ usually do not work. The problem comes down to measurement inaccuracies, as described previously, and to the holistic nature of FR. Furthermore, certain tracks/genres will emphasize or tone down bass levels, adding another variable to consider. 

The most important factor to account for is **leakage**. It is **not a binary system where there is either leakage or not**; rather, depending on the canal entrance geometry and the ear tips being used, variable amounts of leakage are possible. Boosting bass to appropriate levels can sometimes feel wrong due to large amplitude filters, but is essential in improving bass quality perception.

!!! info
	- Bass transition to the lower mids at around 150-300 Hz is important depending on the wanted bass presentation. Making a clear distinction in that region can improve bass quality in terms of "speed" and "separation".
	- Balance between sub bass and mid bass can be modified to increase "speed", "physicality", "dynamics", etc. Emphasized mid bass (eg decreasing everything below 50 Hz) can lead to a "punchier" and "tighter" sound. More sub bass can lead to better "rumble" and "presence", but can also muddy certain tracks 
	- Drums and other bass instruments with a lot of harmonic content can be perceptually altered by considering not only bass frequencies, but also higher frequencies; pay special attention to the 250-400 Hz range, and consider everything below 4 kHz. Kicks and bass synths can be more "dynamic" and "detailed" by increasing higher frequencies, and if needed, reducing fundamental frequency ranges
	- Sub bass can be reduced to further emphasize "punch" and "dynamics". Use a high pass filter and check if bass improves by starting at 20 Hz and going up in small increments


#####Details and resolution
"Details" and "resolution" often refer to the overall perceived amount of sonic information that is being presented. For example, a "detailed" IEM might make certain elements in a track, like small filler percussions (eg subtle maracas), more noticeable, or it can increase harmonic information of a specific element (eg a violin sounding more "textured"). On a very basic level, resolution and detail are tied to relative high frequencies levels: common elements in music that are linked to detail include breaths, instrument textures, subtle percussions, and more for which high frequencies are responsible for a lot of the harmonic content in these elements. 

The first part to consider is auditory masking, where large peaks can mask surrounding frequencies; having proper treble response is important, though the degree of adherence seems to vary. The second part is overall high frequency levels relative to the rest of the FR as well as relative to the specific element that is to be highlighted; for bass instruments, high frequency content will be in a different range than for something like vocals. The difficulty here lies in differentiating between actual tonal changes and perceived resolution.

Unfortunately, there aren't many specific tips that are useful because these aspects **vary in terms of preference and perception depending on the individual**. The only advice would be to use strategic broad changes to change detail perception for the wanted elements. , and boosts in higher frequency ranges (3-12 kHz) will usually result in increased detail perception; it is **important to do small incremental changes** as well as taking frequent breaks much like in the loudspeaker comparison method. 


!!! info
	- Unfortunately, there aren't many specific tips that are useful because these aspects **vary in terms of preference and perception depending on the individual**. The only advice would be to use strategic broad changes to change detail perception for the wanted elements
	- Dips in lower frequency ranges (250-400 Hz) can help certain elements to pop out with more "clarity" and "resolution", mainly vocals and some instruments. Boosts around 150 Hz can result in more "textured" bass 
	- Boosts in higher frequency ranges (3-12 kHz) will usually result in increased "details"
	- it is **important to do small incremental changes** as well as taking frequent breaks much like in the loudspeaker comparison method


#####Separation, imaging, and soundstage
For both imaging and soundstage, proper compensation to your HRTF should result in somewhat accurate localization imparted by the music itself since the factors for proper sound localization are not in effect here (direct/indirect sound from space reflections, ILD, ITD, head movement, and spectral differences from HRTFs of "real" sounds). For separation, a proper balance of every part of the FR should be achieved by paying attention to "transition ranges"; the goal is to keep the overall levels of each instrument and track at appropriate levels. For example, mid bass shouldn't be too emphasized if mid range is to be preserved; in the case of mid bass having too much energy, masking of certain mid range elements can happen, as well as coloring instruments in said ranges. 

These descriptors are arguably the most variable and inconsistent metrics when it comes to subjective impressions. There are however a few common tips that, at best, seem to *somewhat* work for *some* people. A few tricks employed in music production can also be handy here.

!!! info
	- Basic mixing techniques can be used here; overall loudness and balance of said loudness for specific instruments can impart a sense of "depth" and "separation" 
	- A dip at 1-2 kHz might impart a sense of "separation" and pushes vocals and other elements in a track "further away"
	- High levels of high frequency information seems to be somewhat correlated with a more "spacious" presentation
	- Bass is sometimes associated with a "closed in" feeling. Reducing it can increase "spaciousness" by reducing that feeling and by indirectly increasing treble


***
***
###More advanced DSP (\*\*\*\*)
Digital signal processor (DSP) refers to, in this context, to any software/tool that changes the signal, in this case being audio. EQ is a form DSP, but there are many other ones that can change the audio signal in ways that EQ can't. This section will cover some common forms of DSP, as well as some more niche ones. At this stage, there won't necessarily be any improvement in sound; it is yet another experimentation stage. Whether or not you prefer them or regular stereo music will depend on your preferences.

A lot of DSP will be applied through **convolution** (with .flac or .wav files) and/or **VST plugins**, both of which are supported in EqualizerAPO through the "Editor"/"Configuration Editor" app (comes with EqualizerAPO). The explanations will also be brief and only cover the essentials. 

***
####Crossfeed
When listening to loudspeakers, the signal out of one channel will still reach the opposite ear; with IEMs, there is a lack of such an event. Crossfeed fixes this issue by feeding a "small" signal of each channel into the other. It might seem like crossfeed is a necessary and obvious tool that would result in a consistently better preferred sound, it is definitely not as simple as it seems. For hard panned music (eg early jazz recordings with bass in one channel and the other instruments in the other one), crossfeed can help with creating a more cohesive sound presentation. However, most music uses "soft" panning, where the positioning of elements isn't as extreme; crossfeed is indirectly being applied here. It is therefore important to test with crossfeed to see if the change is actually preferred or not. Crossfeed implementation can vary in terms of theory, implementation, customizability, and more, all of which are beyond the scope of this guide. **A few common ones include BS2B, Chu Moy, and Jan Meier crossfeed**.

***
####Dynamic EQ
Dynamic EQ adds another variable into play, which is the incoming signal (in this case being the music); when the signal/music in the specified band passes a loudness threshold, the filter "turns on". Compared to regular/static EQ, the change is **not applied throughout the whole track**. Using it can add another layer of finetuning as it allows for more precise and less disruptive filters. For example, if there's a part in the track that has a substantial amount of sibilance, a regular EQ filter can be used to cut that out, but this also cuts everything including other elements in a track. Using a dynamic EQ, the threshold can be set such that only the loud sibilance triggers the filter while the rest of the track is unaffected. This method is also applicable for improving bass response while minimizing excess lower mid levels. 

While the benefits can be worthwhile, it is important to note that any dynamic EQ presets will **have to be checked and modified depending on the music**. The main difference between regular EQ and this dynamic EQ is that the former focuses on modifying the IEM's FR while only slightly considering music; the latter is more related to the music itself, for which the spectral information can change drastically depending on the genre, mastering, release date, and more, which will **inevitably lead to needed modifications in the dynamic EQ preset**. 

***
####Distortion, compression, and others
Many effects used in the music production side can be applied in this context as well. Distortion might be preferred for some, so adding a bit of distortion and experimenting with different distortion implementations can be effective without having to rely on external devices. The same applies to compression in cases where dynamic range is too high, track mixing isn't up to preference, or for any other reason. A slight delay between channels can also result in a preferred sound presentation. There is a wealth of softwares and DSPs that can change the incoming signal in simple ways like what has been discussed here, or in more extreme ways.


***
####Hesuvi and HRTFs
[Hesuvi](https://sourceforge.net/projects/hesuvi/) is a program that utilizes EqualizerAPO's convolution filter to imitate surround sound (5.1/7.1/binaural sound effects) virtualizations for headphones/IEMs. Included with the software are Head related impulse responses (HRIRs), which can be thought of as recordings of a loudspeaker's response at a specific direction measured with "head mics" (ie measured response at the eardrum). With multiple HRIRs in different directions, it becomes possible to simulate "virtual loudspeakers" for 5.1/7.1 surround sound virtualization. It therefore becomes possible to listen to 5.1/7.1 recordings without an actual surround sound system; while an interesting proposal, the lack of such recording makes it a niche product. The interesting part comes with adding said HRIRs with stereo recordings, in which case an added level of "spaciousness".

The quality of the HRIR varies greatly, and changes depending on how it was made and the intended goal. On the right side, there are common HRIRs, usually from other popular implementations of surround sound virtualization (mainly gaming related), and on the left side, other HRIRs from various databases. The [Binaural Audio](https://binaural-audio.slite.page/p/i38zsD7728/Binaural-Audio) and its corresponding [Binaural HRTF Database](https://airtable.com/appayGNkn3nSuXkaz/shruimhjdSakUPg2m/tbloLjoZKWJDnLtTc)  are resources that contains many different HRTFs/HRIRs and can be useful for quick testing in order to find a good fit.

->![23](https://a.fsdn.com/con/app/proj/hesuvi/screenshots/HeSuVi_Virtualization.png/max/max/1){50%:50%}<-



***
####HRTF Creation and room virtualization/simulation
Proper HRTF measurements are not feasible for most people, and are usually only conducted for population studies or done with mannequins. Companies like Apple and Final Audio employ different methods to account for HRTF, such as taking quick 3D scans of the ear, or by measuring the canal entrance response with microphones in and around the IEM. However, these solutions are either restricted to their own ecosystem, or are limited in accessibility.  There are however a few projects that try to bridge this gap by offering relatively simpler methods of acquiring said data, although their effectiveness is not ideal and effectiveness remains to be seen. 

[EAC - Individualized HRTF synthesis](https://github.com/davircarvalho/Individualized_HRTF_Synthesis) is a project that uses ML to recreate an HRTF measurement based on real-life measurements of the ear. The process requires the user to take measurements of their ear - there is a tool to facilitate the task using pictures and a reference length - and inputting them into their software. The final result is an HRTF SOFA file that can be used in room virtualization software. The HRTF file itself is not particularly useful; it needs another program, usually one that attempts to simulate a room with said file. For example, with their HRTF SOFA file, the user can then use another program that simulates a room to the user's need, and for which the response of the person's HRTF can be had. It is therefore possible to recreate a room that has a diffuse sound field, incorporate the HRTF, and measure the DF HRTF of the user. The author of the paper also has several other projects, such as a Webcam Head Tracker and a Room Auralization, with the latter being able to use SOFA HRTFs.

The issue with this method is that the synthesized HRTF itself deviated significantly from their actual acoustically measured HRTFs. There is also the lack of ear canal geometry, head/torso dimensions, and finer ear details in the HRTF calculations; all of these factors can lead to synthesized HRTFs that aren't ideal. The deviations shown in the image below highlight the large differences in amplitude between the proposed/synthesized response (dotted lines) and the original/measured response (solid lines) as well as the overall smoothed result.


->![Comparison between synthesized and measured HRTFs on the horizontal plane at various azimuths](https://i.postimg.cc/6px0Gksz/EACsynthesis-HRTF.png){80%:80%}<-


[MESH2HRTF](https://www.mesh2hrtf.org/) is an open-sourced project that uses the same concept as the previous project, except it requires a 3D scan of the whole ear and head. The mesh is then used with modeling software like Blender and the project's own calculator to obtain HRTFs for specified angles in a free-field. It is also possible to obtain a SOFA file for the HRTF and to use it in other room simulation softwares. The accessibility of this project is rather low, requiring at the very minimum a modern iPhone which will produce less than ideal results, or a professional 3D scanner. Furthermore, the same problem of not accounting for canal geometry still applies here.

->![Mesh2HRTF](https://raw.githubusercontent.com/Any2HRTF/Mesh2HRTF/master/docs/figures/graphical_abstract-01.png)<-

For room simulation, there are a few projects that have SOFA implementation. [Anaglyph](http://anaglyph.dalembert.upmc.fr/) and [SofaMyRoom](https://robaru.github.io/sofamyroom/) are both programs that allow for localization customization based on various parameters; Anaglyph is focused on ILD and ITD changes with simplified localization modifiers, while SofaMyRoom is focused on room emulation with different room and loudspeaker parameters. As mentioned previously, there is also the [Auralization Engine](https://github.com/davircarvalho/Auralization_Engine) project that aims to create virtual audio scenes; this program only works with one track at a time, but is worth taking a look at as it includes head tracking and is relatively accessible.

->![Auralization engine](https://raw.githubusercontent.com/davircarvalho/Auralization_Engine/master/Images/1.PNG){50%:50%}![Anaglyph](https://i.postimg.cc/cC3B6SmR/Anaglyph.jpg){46%:46%}<-

***
####Custom DSP
It is of course possible to create your own DSP if any of the current offerings are not enough. EqualizerAPO itself is a very powerful tool that allows for a lot of customization and signal mapping/processing, and combined with its convolution filter, it is overall an excellent method of experimenting. Both this method as well as creating a DSP is way beyond the scope of this guide, and should only be attempted by the curious. Most solutions are already available for way less effort.

***
***
###Ideal spatial rendering and sound localization (\*\*\*\*\*)
The perfect audio experience with IEMs would be one where actual sound localization is perfected, and where transparency relative to real life has been achieved. Bypassing the regular headphone/IEM stereophonic limitations and crossing into full spatial rendering of audio is arguably the goal, and for what is arguably the best possible audio experience that is accomplishable on IEMs, it will require enormous amounts of ingenuity, as well as a shift in the music production industry. 

We can only wait until more studies, discoveries, and innovations happen before such a goal becomes accessible, easy-to-use, and effective. For now, there are a few key elements that have to be perfected, as well as a few others that will have to be studied to better understand their possible effects.

!!! note Key elements
	- Full in-situ response at the eardrum will have to be mapped out and corrected properly
	- Extensive HRTF data of the user will have to be measured to a high enough accuracy for proper response calibration
	- ITD/ILD factors will have to be considered and implemented correctly for the user
	- Object-based audio should become widespread, ideally avoiding the circle of confusion. Stereophonic audio will be fine as well but should be considered when rendering the spatial environment
	- Occlusion effects, physical sensation of the IEMs, and discrepancy between real-life vs recorded environments should ideally be studied to ascertain their impacts on localization and preference


***
***
##Case study: Tangzu Wan'er

Now that EQ and other forms of DSP have been covered, it is time to apply what was learned; in this guide, the Tangzu Wan'er will be the IEM of choice due to its popularity. Note that the following steps will only use a few of the sections, mainly the ones that have time-efficient steps (ie not ones that require a lot of time). Those included should be relatively easy, accessible, and effective enough for most people. 

!!! info Personal preference and perception
	- Bass has to be present in ample quantity. Sub bass is important, but not as much as mid bass presence and "punch"
	- Mids have to sound natural. Maximum of the ear gain has to be between 2.5 and 3 kHz. The fine details depend on the rest of the FR. Some coloration is acceptable in the lower mids to accentuate the rest of the mids
	- Treble has to be present and will, in most cases, be slightly higher in amplitude compared to targets like JM-1 
	- Imaging and soundstage is mostly the same across IEMs 
	- Listening volume around 60-70 dB in very quiet environments (<40 dB)

***
###Data 
The following FR graph shows the insertion depth profile for the Wan'er in order to reveal treble level as well as other possible unwanted resonances. Note that different sizes of the same tip (silicone, medium size bore) were used to achieve these measurements. As insertion depth gets deeper, pushing the coupler's resonance peak higher in frequency, it becomes clear that the treble on the Wan'er slopes down rather aggressively, which might not have been too obvious with an 8 kHz aligned resonance measurement. Furthermore, since 711 measurements are inaccurate in the treble region, the need for measurements of different ear tips isn't crucial; in my case, I found tips that were comfortable and used them when using EQ by ear (stock black bore tips). 

->![Tangzu Wan'er insertion depth profile](https://i.postimg.cc/Hj17Dw0H/Waner-Insertion-Depth.jpg)<-

For the bass, everything looks fine, but remember that 711 measurements often overestimate this region, and are inaccurate when it comes to recreating proper sealing/leakage of IEMs with actual ear canals. While the graph might indicate a normal amount of bass, actual bass response in my ear might be (and actually is) different, and **much lesser than what was measured**. The distortion profile is also fine, measured at around 104 dB with most of the frequency range having less than 0.5% distortion limited to second harmonic distortion; as mentioned previously, distortion for IEMs is almost always negligible, even with very large EQ changes, and the same applies to the Wan'er.

!!! info Summary of Tangzu Wan'er impressions and EQ goals
	- Bass is on the lacking side in terms of "punch" and overall "technicalities", but the overall balance is good
	- Treble needs some more quantity, and there are a few peaks that should be addressed 
	- Mid range is good, but there is a slight "closed in" presentation, and vocals are emphasized
	- EQ will be used to improve bass quality, fix treble, and minimize the perceived "closed in" presentation



***
###EQ

For bass, as mentioned previously, a significant boost is needed; knowing my personal preferences, three filters will be used. The first one is a peak filter at 20 Hz with a Q of 0.5 for sub bass. The second is a low shelf filter at 100 Hz with a Q of 0.71 for more "impact" and presence in the track. Finally, a peak filter at 200 Hz (or any region depending on preference) with a Q of 1 is used to prevent any possible excess lower mids and mid bass bleed while accentuating the bass quantity/quality as well as the rest of the FR. For the gain values, it depends on what the goal is. In my case, small gain values were enough to improve bass qualities instead of shifting the overall tonal balance; for the first two filters, 2 dB was enough, and for the last, -2 dB.

For my own preference, treble will need to be slightly boosted; in this case, with a high shelf filter starting at 6 kHz with a Q of 0.71. The gain can be changed at any time, and is not a big concern for now. The second step will be to check if there are big resonances for my individual perception. With a tone generator, I located two very significant resonances; one at 7.1 kHz, another at 10.3 kHz, and a last one at around 14 kHz, all of which were audible with music and were cut down with peak filters with a Q of 4. Now that they've been identified, **pink noise and music** was used to determine the gain. With only the tone generator and aiming for relative/roughly equal loudness, both needed -8 dB, which resulted in music sounding muted. With music and pink noise, the first peak could be decreased by -4 dB, leaving a bit of extra "sparkle" without sounding harsh. The second peak could be set at -6 dB, while the third one wasn't audible on most tracks, but a -2 dB cut can be used to be on the safe side.

Finally, for the mid range, most of it sounds good. Since the ear gain is mostly positioned correctly (would have preferred for it to be closer to 3 kHz) and the rest of the mid range from 300 Hz to 1 kHz sounds fine, there is little to modify, especially when considering that most of the previous changes address the transition ranges. A potential issue is the lack of separation and "closed in" feeling, which is most likely due to excess energy from 1-2 kHz caused by an early ear gain. Using a 1.5 kHz filter with a Q of 1 can be useful, and a gain of -2.5 dB seems to help effectively with separation and pushing vocals back in the mix, although personally the trade-off of having more vocal presence is fine for me as well.

Now that most "issues" in the treble and mid range have been addressed, the high shelf filter at 6 kHz seems to work best at around 2 dB. With the main changes set in place, small changes can be implemented for improving the intangibles. In this case, a small boost (1.5 dB with a Q of 1.5) at 9.4 kHz seems to accentuate perceived "resolution" while not altering overall tonality too much, and a small narrow boost around 2.7-3 kHz seems to increase perceived vocal details (too track dependent for so this will be ignored).

Below is the final FR of the Wan'er (measured with an 8 kHz coupler resonance) with the EQ filters. **Bold** filters are highly individual (ie only for me), and are excluded from the final FR; **every filter parameter should be modified to your preferences**. Preamp should be set to -4 dB.

![Tangzu Wan'er Final FR post-EQ](https://i.postimg.cc/TP5Gb4mN/Waner-Study-Case.png)

Filter type | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|
PK | 20 | 2 | 0.5 | 
LSF | 100 | 2 | 0.71 | 
PK | 200 | -2 | 1 |
PK | 1500 | -2.5 | 1 |
**HSF** | 6000 | 2 | 0.71 |
**PK** | 7100 | -4 | 4 |
**PK** | 9400 | 1.5 | 1.5 |
**PK** | 10300 | -6 | 4 |
**PK** | 14200 | -2 | 4 |

!!! note
	->**Of course, this is just a small example and doesn't include a lot of what was discussed throughout the guide. From just these small judgments and steps, the sound has been improved considerably without having needed to spend more than an hour to come up with this preset. Further improvements can be had in terms of bass quality and treble refinement, but stopping here would be perfectly fine as well.**<-


***
***
##Measurement rigs, curves, and preference targets

!!! info
	->The following section is dedicated to explaining and detailing the different FR curves that are prominent nowadays, as well as the different measurement rigs and standards that are being used. Preference target curves by reviewers will be mostly ignored as they are usually based entirely on subjective preference.<-

###Measurement rigs and standards
Measurement rigs and systems for acoustic phenomenon have several standards they have to abide by. There are two relevant standards nowadays when it comes to IEMs: the IEC 60318 standard, and the ITU-T P.57 standard. Within these standards, there are further classifications; for the IEC 60318, the relevant ones are 60318-4 (also commonly referred to as 711, for IEC 60711 which was its predecessor) and 60318-7. The difference between the two is the presence of a **head and torso simulator**, with the former only detailing the ear canal's acoustic impedance. For the ITU-T P.57 standard, there are many different categories based on different pinnas and occluded ear simulators.  In the context of IEMs, HATS can usually be ignored. The important rigs/systems to consider are **IEC 60318-4 (711) rigs, and ITU-P.57 type 4.3 rigs**.
[Did Linus just waste $50,000?](https://www.youtube.com/watch?v=Qc__cF6i2mw)

####IEC 60318-4 occluded ear simulators 
IEC 60318-4 couplers, or commonly referred to as 711 couplers, have been the industry standard for a few decades, and are systems that aim to simulate the acoustic transfer impedance of the average occluded human ear canal. To do so, couplers have specified air volumes but do not simulate ear canal geometry, which results in less accurate transfer impedance in the treble region above 10 kHz, and might also impact transfer function resulting from IEM wear as mentioned previously.

These couplers only have a metallic tube where the IEM can be inserted, which affects results in various ways. The first is that coupler resonance is usually higher in frequency than what usually happens with human ear canal resonances. The second is that the metal tube does not accurately simulate possible leakage scenarios for IEMs. FRs measured with "correct" seal on these systems are therefore very ideal in terms of sealing; real sealing conditions on humans will most likely have varying levels of subtle leak, thus changing perceived low frequency response. With the -7 standard that includes a pinna, some of these issues can be mitigated in exchange for harder and more inconsistent measurements since leakage has to be accounted for much more thoroughly.


####ITU-T P.57 Type 4.3 (B&K 4620/5128) ear simulators
ITU-T P.57 type 4.3 specifies both the pinna and the occluded ear simulator, and compliant systems for this standard are also usually compliant with IEC 60318-7. For the pinna, the ITU-T P.57 Type 3.3 pinna is used with a small change at the base for attachment purposes as well as better transfer impedance matching. The occluded ear simulator is based on a study where researchers analyzed and measured the transfer impedance of 32 subjects in order to create an anatomically correct and more accurate occluded ear canal: the important change here is the presence of ear canal geometry. This results in better transfer impedance matching to the average, more accurate canal resonance location, and other changes, of which the relevant parts are discussed in [Measurements and misinterpretation](https://rentry.co/IEM-EQ-Guide#measurements-and-misinterpretation). The most prominent compliant system is the B&K 4620/5128, where the 4620 only includes the pinna and ear simulator while the 5128 includes the head and torso simulator. ITU-T P.57 type 4.4 utilizes the same pinna as type 4.3, but instead terminates with an IEC 60318-4 coupler for the ear canal from the reference plane to DRP. The important part of this new standard is that the increased accuracy in low frequency transfer impedance should theoretically allow for direct headphone-to-IEM measurement comparisons: this is especially interesting when considering the preference research for both, where large discrepancy in bass was observed.


***
###Preference target or not?
Whether or not to call an FR curve a preference target depends entirely on if said FR curve has undergone preference testing, which usually involves a sample that undergoes several "calibration" steps with one device/IEM. They are then made to listen to various audio signals, usually music with significant content throughout the audible band (ie music that has enough bass, mid range, and treble content) with different EQ presets that change the FR to various curves. The subject then rates the different presets, and the final results are analyzed. 

A simple definition can be that a preference target is an FR curve that has shown to be liked significantly. FR curves that are shown to be not preferred highly, and/or are based on theoretical concepts (eg DF) are not targets per say, just FR/reference curves. The question of whether or not the term of personal preference target is actually a preference target can therefore be answered when looking at the above definition, in which case the use of the term is correct. 

!!! info
	->A preference target is an FR curve for which preference has been shown to be high, and one that is usually targeted for by either manufacturers or  listeners.<-



***
###Harman In-Ear target (711 & 5128)
The HarmanIE target has gone through three iterations (2016, 2017, 2019v2) and is a preference target made by Harman for IEMs for measurements made on IEC 60318-4 compliant systems. It is currently the "most researched" target in terms of sample size, and has been shown to be very well correlated with preference by other studies. There is however a general disagreement about it with some in the community;**do remember that the community is a very thin slice of a slice of the average population**.

Harman's IEM research, started indirectly in 2016 with a study on preferred bass response in IEMs, has a similar aim to their headphone target, which is to find the most preferred FR target. For headphones, the target response (Harman 2013) aimed to reproduce the same response as a a calibrated 7-channel loudspeaker system with flat on-axis anechoic response placed in a semi-reflective room, resulting in an in-room response that drops approximately 1 dB/oct from 20 Hz to 20 kHz with a bass boost around 105 Hz. To do so, a HATS was placed in a reference room and the resulting response was used. The 2016 version of HarmanIE was essentially the same as the headphone target, but with a 4 dB increase in bass levels; it was reasoned that this increase was due to occlusion-induced noise. The difference in treble is negligible. 

->![HarmanIE 2016 compared to HarmanOE 2013](https://i.postimg.cc/13R5hqsR/Harman-IE-2016.png)<-

In 2017, Harman published a two-part study that formally examined their established target against many other IEMs. They found that the target was significantly preferred over every tested IEM, for both trained and untrained listeners. To do such testing while minimizing potential biases that might arise from the physical aspects of the IEM itself (eg fit, material, size, etc), a virtualization method that was validated in another study was used, where they equalized the response of the IEM that was used to the responses of the tested IEMs and the established HarmanIE target. It is important to note that the 2017 iteration is very different from the 2016 one, mainly in the treble. The changes have only been covered briefly, and have been described as having been done with formal listening tests with both trained listeners and the three authors. The most notable differences are the elevated treble amounts, as well as the appearance of what seems to be resonances. Furthermore, the response drops off abruptly after 10 kHz due to the inherent response of the IEM, as well as high individual variation in FR at the DRP.

For the 2019v2 target, Harman has not published any publicly-available studies. It is essentially the 2017 version of the target with smoothing applied (very similar preference ratings when testing IEMs), with most fine details like the resonances and fine HRTF details being removed. It is currently the most popular version of HarmanIE, and is what is currently being used in AutoEQ. It is also the basis for many different targets and projects. For the 2017/2019v2 targets, the changes from the 2016 target are **not thoroughly explained**. There are two major changes: the bass shelf shape (ie Q) is different, and the level in the region from 3-8 kHz was increased. The issue that most people have with HarmanIE (usually 2019v2) can be explained by two factors: the mid bass and lower mids dip at around 250 Hz,  and the elevated region from 3-8 kHz. Both of these aspects exacerbate one another, and lead to what many report as being a "thin", "overly bright" sound. 

->![HarmanIE 2017 and 2019v2](https://i.postimg.cc/DyTw6NNX/Harman-IE-2017-2019v2.png)<-

These issues are often said to be related to the methodology and reasoning behind the target, where many argue that the assumption that the headphone target would translate for IEMs is wrong. The addition of listener filter modifications should therefore be a fix for such an issue, but in the 2016 study, only the bass shelf was adjustable, which could lead to overcompensation for the rest of the FR. The changes past the 2016 target cannot be discussed, but it is reasonable to assume that the increase in the treble region was again caused by overcompensation for the bass increase in the 2016 target. As explained previously in the [Measurements and misinterpretation](https://rentry.co/IEM-EQ-Guide#measurements-and-misinterpretation) section, the "inaccurate" acoustic impedance below 1 kHz for 711 couplers could also explain the discrepancy between the headphone and IEM targets.

Despite all of this, the HarmanIE target is still highly preferred in most listening tests done. A preliminary study using the 5128 rigs and a small group of listeners by Sean Olive also shows a high preference rating for the target after roughly compensating the target to 5128. There were however many other curves that were rated similarly high. A new HarmanIE target is currently in the works, this time with what seems to be an overhaul of the premise of headphone response being the foundation, since the 5128 system seems to allow for direct headphone-to-IEM comparisons. 

A paper in 2024 examined the preference targets for IEMs on the B&K 5128. 5 targets were examined and rated by the listeners; it was found that the HarmanIE 2019 target (translated to the 5128 with corrections) and the Soundguys target were both preferred equally and above the other three targets by class 1 listeners (72%). The results show similar preference that despite the two targets having large - both in amplitude and range - differences, which the author suggests is due to "a perceptual tradeoff between bass and treble levels whereby a reduction in bass may be compensated with an equivalent reduction in treble, and vice versa". Furthermore, he also suggests that "it seems that a constant delta of 8 dB between the bass and treble 
bands of the target curve can produce equivalent satisfaction and listener preferences".

Class 2 listeners (28%) preferred the DFmod target, which used the two filters from the HarmanOE research on the 5128's DF response, followed closely  by the APHarman2018Ver2 target, an OE target developed in another study focusing on preference targets on the 5128 for OE headphones. The differences between both targets do not reflect the same hypothesis of treble and bass tradeoffs, but would rather point at small band changes, mainly around the 3 kHz mark.

In a (unreleased as of writing) MOA (method of adjustment) study, listeners had three possible adjustments they could configure on the B&K 5128's DF response: ±12 dB shelf filters for bass and treble, and a +6/-10 dB peak filter at 3 kHz. Listeners were first able to tilt the response in both ways, then fine tune the bass and treble filters, and finally adjust the 3 kHz filter. Results indicate that on **average**, listeners preferred a -1 dB/oct. slope in the first step. Small increases in bass and decreases in treble was common in step 2, and step 3 had little changes. Cluster analysis revealed 4 different classes, all having varying levels of bass and treble preferences: the silhouette score, a measure of cohesion and separation of objects to their own and other clusters, of most of them are on the weak side due to the MOA having 3 separate variables.

HarmanIE 2019 compared to the average MOA target shows two main differences: a dip from 200-600 Hz, and more bass (with a steeper slope) and less treble above 8 kHz. The Soundguys target has slightly more bass than the average and much lower energy between 3-6 kHz than both the average target and any other tested one. The DFmod matches the closest to the average MOA target with differences in bass level and shape despite being less preferred by most listeners in listening tests compared to HarmanIE 2019 and the Soundguys target. The APHarman2018Ver2 had a significant difference in the ear canal resonance which might explain its low ratings in the preference study (only better than DF).



!!! note Notes on HarmanIE
	- Bass level is based on a segmentation study by Harman, and is highly variable
	- Ear gain and treble regions are heavily smoothed for various reasons. Treble also drops off heavily past 10 kHz, and probably shouldn't be considered
	

***
###Usound1V1 target (711)
The Usound1V1 target is developed by Usound, a B2B acoustics company focusing on MEMs drivers. It uses the HarmanIE research and adds environmental noise during testing to replicate real-life portable use of IEMs in non-ideal conditions (unlike a lab). Adjustments to the base target were done similar to what Harman did, and the resulting most preferred target became UsoundV1; no papers have been published.
Differences between HarmanIE and UsoundV1 mostly come down to the bass region, with the latter having significantly more bass with the shelf starting at a higher frequency. Furthermore, the frequency range between 1 and 7 kHz is slightly reduced on the Usound target. 
The differences between the HarmanIE and the Usound1V1 targets are rather minimal, although the Usound1V1 target does address a common complaint about the upper frequencies with HarmanIE.

->![Usound 1V1 (oratory1990) compared to HarmanIE 2019v2, normalized at 500 Hz](https://i.postimg.cc/8Cjpsg7q/USOUND-1-V1-Target.png)<-

***
###Diffuse Field curve (711 & 5128)
Diffuse field is not a specific FR curve or target; rather, it is physically-defined sound field, not based on preference. A diffuse sound field admits equal weight to sound incidence from all incoming directions  - imagine a very, very reverberant room - at all frequencies. By putting a HATS in such sound field and measuring the response, the resulting FR looks like what is often referred to in the community. Commonly called the DFHRTF (or simply Diffuse Field (DF) curve in most mentions), the curve will have differences depending on the HRTF of the person/HATS.

The main justification for DF equalization for headphones and IEMs is that the sound field matches how sounds are localized when wearing such devices, where most sound localization mechanisms (eg ITD and ILD) aren't "available": unlike loudspeakers or real sound sources in space, headphones and IEMs also do not have specific "angle" to measure them at like with FFHRTF measurements of loudspeakers. Another way of looking at it is by looking at the DF definition; since sound at all angles is of equal power, there is no change to the measured response no matter if the head is being rotated or displaced. Headphones and IEMs also exhibit such properties, where head rotation/displacement has no effect on the perceived sound.

A more in-depth understanding and motivation for DF equalization can be had by inspecting Theile's association model: the premise that the brain interprets tonal response **after** fitting the input stimulus from two ears into its spatial response filter indicates that **spectral features from the outer ear do not result in perceived timbre changes**. Timbre is therefore not entirely determined by the response at the eardrum, and is instead only determined after the spectral changes resulting from the direction-dependent HRTF has been filtered out by its inverse function.
With the observation that headphones (and earphones) do not present particular spatial auditory cues to the listener, only seeming to localize from within the head, Theile concludes that headphone equalization should favor no direction (ie a DF response). 

->![Theile's association model](https://i.postimg.cc/D0Yg5Fwq/Theile-Association-Model1.png){41%:41%} ![Theile's association model for headphones and stereophonic signals](https://i.postimg.cc/nVd0nKGC/Theile-Association-model2.png){50%:50%}<-

A separate study on FR curve preference was conducted by Lorho. In his 2009 paper on listener preference of curves based on FF/DF (mainly related to the 3 kHz ear gain and relevant parameters such as amplitude, center frequency, and width of the filter), it was found that the main factors to consider were the center frequency of the ear gain, as well as the amplitude. Preference was overwhelmingly determined by these factors, and curves having similar peaks as with FF and DF were disliked. Results also show that a negative amplitude was disliked. The optimal response was a 3 kHz peak with an amplitude of 3 dB (between 1 and 5 dB), which significantly lower than either responses. Although thorough, the study and its results have not been used much mainly due to the very restrictive curve modifications allowed which might result in overcompensation (eg no bass/treble modification might have resulted in a very significant deviation of the ear gain from DF). It is however important in further advocating for the use of another curve other than DF.

->![Possible curve modifications](https://i.postimg.cc/sxktKbm0/Lorho1.png){41%:41%} ![Contour plot for the responses](https://i.postimg.cc/tRsJSPDh/Lorho2.png){46%:46%}<-

The ISO 11904-1/-2 standards propose two methods of measuring DF response; 11904-1 uses in-ear microphones to measure the DF response at the subject's eardrum, while 11904-2 uses a population average pinna (derived from blocked canal measurements) contributions combined with a mannequin's ear canal transfer function. The -1 standard can be thought of as an "absolute" reference, while the -2 standard can be thought of as a malleable methodology which can be applied to both the 711 and 5128 systems. For IEMs which are high acoustic impedance devices, a DF response from ISO 11904-2 is more suited, especially with 711 rigs for which acoustic impedance correction will be necessary if measurements are to be compared to a DF response obtained with the -1 standard. 

It is important to note that while DF seems to fit the idea of localization with headphones/IEMs, studies have consistently shown that a "pure" DF response is **not preferred or liked**. Instead, it is used as a foundation for which modifications can be had. Harman's research somewhat validated this - in their recent preliminary test, additional speakers were used to obtain a reference response in their room, which correlated very much with the DF response of the same HATS - and by adding a few modifications, they have made a highly preferred curve for headphones/IEMs. Other curves built upon DF have also resulted in high preference as well. The two main modifications include bass adjustments to compensate for lack of body interaction, and overall response tilt, usually a downwards/clockwise tilt. The latter can be thought of and argued as being the same the inherent tilt of loudspeakers in a room: much like how loudspeakers should have a flat response in an anechoic sound field with a downwards tilt when placed in a room, headphones/IEMs should also have a flat response in their sound field (in this case DF) with a similar downwards tilt when listening to them.

!!! note Notes on DF
	- DF seems to be the appropriate sound field when considering headphones/IEMs and the localization process from the association model
	- Raw/pure DF is not preferred or liked, and should only be used with modifications 


***
###Etymotic target (711)
The Etymotic target, developed by Etymotic, uses the DF curve as a base and applies what Etymotic considered to be the correct room curve: the THX/X-curve, which has been shown to be not ideal in terms of preference, and is only used in theatres and cinemas as opposed to normal listening environments. The curve is based on outdated thoughts of loudspeaker radiation and concepts of accuracy. Etymotic therefore arrived at a target that closely matched their KEMAR DFHRTF (smoothed), with a reduction in energy starting from 2 kHz to 20 kHz. Another issue with the target is that it relies heavily on the accuracy score - Etymotic boasted about their 100% accuracy score for their IEMs using a slightly modified KEMAR system - as justification for its effectiveness, which is a scoring system used by Consumers Union from the 1970s until 2006. It uses what is now considered an outdated method of quantifying "correctness"/preference ratings for loudspeakers.

->![Etymotic target compared to a KEMAR DF response](https://i.postimg.cc/fWXbxs8s/Etymotic-target.png)<-


***
###IEF 2020/2023 targets (711)
Made by Crinacle as a basic target, the 2020 target contains only a very smoothed ear gain centered at 3 kHz, and with a linear response from 20 Hz to 1 kHz. There is no formal preference testing or theoretical basis behind this target except for the ear gain concept, although the ear gain used here is not a smoothed one, but rather an oversimplification which seems to only be based on a very generic shape. Its main purpose was being a template, for which bass and treble were left to the user's preference. 

The newer 2023 target based on a tilted DF response for the 5128 rigs, translated to 711 systems. The biggest difference with the DF response is that the ear gain and most HRTF features are smoothed over, akin to the ear gain in IEF 2020. Compared to IEF 2020, the major difference is an increase in low frequency energy, as well as the subtle dip at 1.5 kHz. Customization includes bass level with a shelf starting at 105 Hz, and tilting of the whole response by dB/oct. 

->![IEF 2020 and 2023](https://i.postimg.cc/NjNGgjj6/IEF-Neutral.png)<-

***
###Δ and JM-1 curve (711 & 5128)

The Δ curve is simply the 5128 DFHRTF compensated to 711 rigs. The JM-1 curve is similar to the DF + tilt signature, but a distinct difference being that instead of relying on a specific measurement rig's HRTF, it uses the canal transfer function of that specific rig, combined with the contributions from a population average pinna. It is also based on the ITU-T P.57 Type 4.3 (5128) rig, and should therefore result in a more accurate DFHRTF both in terms of canal response and outer ear response.

The use of a rig's canal transfer function combined with a population average pinna response for calibration of audio systems that do not interact much with the outer ear (ie does not deform or physically touch the outer ear) has been detailed in ISO 11904-2; the JM-1 curve uses a similar idea, this time using the B&K 5128 canal instead of the one specified in IEC 60318-4. For the population average pinna, it is argued that the one specified in IEC 60318 (the one used on type 4.3 and IEC 60318-7 HATS) is not representative of the human average response, being brighter than normal. Instead, a pinna from Hammershoi and Moller is used, as detailed in the ISO standard. Evidence of HATS using the mentioned IEC 60318-7 pinna having brighter DFHRTFs has been found by Harman research, which compared rig responses to that of around 350 human subjects whose HRTFs at the blocked canal were measured in their Hyperion sphere.	

Because the curve is based on the B&K 5128 which can supposedly remove the need for two separate preference targets for headphones and IEMs, JM-1 also incorporates a 3kHz adjustment similar to the one found in the HarmanOE 2018 target (a reduction of around 2.5 dB). The change made by Harman is not well defined in their studies, but was explained briefly as being preferred in informal listening sessions with trained listeners. The adjustment is a reduction in energy at that region, but should only have a minor effect on preference. Based on **very** preliminary research by Harman (S. Olive), the JM-1 target fared quite well as a preference target against other targets and curves. While falling short of other targets like the Soundguys and HarmanIE ones, the tested JM-1 was using the filters from HarmanOE 2015 instead of HarmanOE 2018; the latter and more preferred one is very similar to the Soundguys target and tracks closely up until 8kHz. Above that, the Soundguys target has more energy while also having a bass shelf included; since JM-1 is based on DF + tilt, preference bounds from Harman research should also be used along side the curve.

For now, JM-1 and what is specified in the ISO standard are mostly similar, and are for most circumstances interchangeable. Do note that the JM-1 target is made using a **derived** canal transfer function, meaning it was calculated mathematically; when the canal transfer function will be measured, another target (JM-2) will be developed. 

Here's a video by the creator of JM-1 explaining the target: [The New IEM Meta Explained](https://www.youtube.com/watch?v=EZoKPtzjdtQ)


***
###SoundGuys target (5128)
Developed and released in 2021, the SoundGuys target for headphones and IEMs was made using many 5128 measurements of what the SoundGuys team describes as being a "benchmark product, which is generally a standout product that our technical team agrees does a great job of catering to the headphone market by providing a pleasing, enjoyable sound that we can all get along with". Not much of their process is explained. The resulting target was used in a preliminary IEM preference target study by Harman, and was shown to be highly preferred by both trained and untrained listeners.

->![SoundGuys target](https://i.postimg.cc/qMxM5LfZ/Sound-Guys-target.png)<-

***
***
##FAQ

*I can't hear the difference between EQ presets, am I doing something wrong?*
Check to see if you setup your EQ app properly, and if you routed your audio correctly. If everything is correct but you are still struggling to hear a difference, then either your EQ preset doesn't impart meaningful changes, or your listening ability is not up to par. 


*What does it mean for an IEM to respond well to EQ?*
For that specific user, it usually means that the EQ is working as he intends. Truth is that most IEMs "respond" excellently to EQ, with very minimal distortion being introduced. The concept of EQ responsiveness most likely came from changes done through EQ that didn't match expectations, and is most likely correlated to FR misinterpretation.


*Can EQ cause mechanical/electrical failure?*
IEMs are much more robust than one might think. EQ used in the guide will never cause any failure. EQ used throughout the guide is software, and is completely reversible. 


*What about driver quality?*
"Driver quality" is used as a direct synonym to "technicalities" in the audiophile community. Driver quality as used in the community should instead refer to FR, but also other properties such as distortion, efficiency, leakage tolerance, reliability/channel matching/QC, etc. 


*How do I train my listening ability?*
There aren't any proper standards concerning listening ability, and what training that is available and aimed at such a goal can vary depending on the many factors like geographical location, field of study/practice, and more. 
As far as listening ability is gauged in the community as well as in studies on preference as seen with Harman, the "How To Listen" (HTL) program is used. Harman's research classes listeners into two groups: trained and untrained listeners, with the former having completed the required exercises to a certain level. Previously, trained listeners were required to pass level 8 on all exercises; nowadays, only the peaks/dips exercise is needed, with the rest having been substituted for training documents for the listener to read.
Other programs also employ similar forms of exercises, mainly incorporating the peaks/dips one, such as eqTrainer and AudioBan.


*Who are you?*
None of your business, and no one you know.

*What IEMs do you like or use?*
Anything that isn't broken and is comfortable.

*I have a question / There's a mistake, how should I contact you?*
If you want to help out, suggest improvements, ask a question, or proofread and correct some parts in the guide, then contact me via Signal, SimpleX, or Session through the QR codes below (fully anonymous; Signal requires a phone number which isn't shown to contacts). **I am not present in any community, forum, or group, and do not have any alias or account**.

->![Signal](https://i.postimg.cc/25t7rf44/Signal.png){25%:10%}	%transparent% OOOOOO%%		 ![SimpleX](https://i.postimg.cc/V6bBNHR2/Simplex.png){25%:25%}	%transparent% OOOOOO%%		 ![Session](https://i.postimg.cc/sXJ3X3zN/Session.jpg){25%:25%}<-


***
***
***
!!! note That's the end. Hopefully this guide was useful, informative, or at least entertaining. %transparent% and as always, remember to use EQ~!  \\|^w^|/ [new](https://rentry.org/IEM-fit-comfort-guide)%%
