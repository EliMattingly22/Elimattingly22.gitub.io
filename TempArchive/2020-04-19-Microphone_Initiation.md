---
title: "Microphone Project"
date: 2020-04-19T15:34:30-04:00
categories:
  - blog
tags:
  - project
  - microphone

sidebar:
layout: single

---


# The first project!

The first project I’ll be following on this site is going to be the design and creation of a microphone. As with any project I think it is important to start with the motivation: Given it is a microphone project it is pretty clear that I want to record audio without noise or distortion. But why make my own instead of buying one? First, microphones are a fascinating piece of instrumentation, and I’m interested in learning more about what goes into one. Plus, by building one I’ll have a good test platform for analog signal processing circuits. Preamps, power supplies, filtering, all that good stuff. Then there is all of the science behind how to record audio well (pop filters, echo suppression etc.). The next reason is that I think it is a nice size of a project to start on from a blogging/recording point of view. It won’t take me months to do, but it is certainly far from trivial from a design perspective. 

In the long-run I’m hoping to start recording supplemental material to this blog, and this will be one step closer to enabling me to do that. 


## Deliverables (to myself)

With any engineering project there needs to be an end-goal. Something specific that needs to be accomplished. So here I’ll define the criteria that will make the microphone a “success”
*  It should have a signal-to-noise ratio of at least 74dB. I’m picking that seemingly arbitrary number because I found a blog post online saying that is a good bar to shoot for ([My New Microphone Blog]( https://mynewmicrophone.com/what-is-a-good-signal-to-noise-ratio-for-a-microphone/))
*  It should be designed to reasonably couple with standard microphone stands and attenuate noise due to bumping into the stand or desk. I don’t want to reinvent every wheel. 
*  Let’s shoot for $15 of material on the final design. All included. 

# Project breakdown

![Project_Breakdown]({{ site.url }}{{ site.baseurl }}/assets/images/Projects/Hobby/Mic/Schematic_Overview.png){: .align-center}

The actual microphone sensing element is just one part of the system, so to wrap my head around what I need to make I find it helpful to list out everything that goes into it. Above is a little sketch of my ideas. 

From signal source to the recorded file:
* Obviously there is the audio source. A person talking, or whatever.
* The medium the sound waves travel to, and the room it travels in. This means echoes, background sounds etc.
* A pop filter
* The microphone transducer—the thing that turns pressure waves into voltage or current
* A pre-amplifier amplifies the tiny signal the transducer, hopefully without distorting it or adding noise.
* The “downstream” electronics I will lump together, this included a buffer amplifier, electronic filters, etc. This can also include little LEDs and such.
* The wires going from my microphone circuit to the computer
* Power supply, and the “ground” 
* Some sort of enclosure and all the bells and whistles that go with that. 
* A stand that can hold the microphone without having physical bumps manifest into noise.

I'll make a post about each of these going into details from a design perspective, but for now here are some resources I have found helpful:

* [EEVBlog's YouTube series about microphones](https://www.youtube.com/watch?v=ihAG6cMpUlY) In these 7 videos he hosts Doug Ford, former head designer at Rode Microphones and gets into the weeds of microphone design from an electrical engineering perspective. It's great. 
* [Analog/LT's guide to microphone sensitivity](https://www.analog.com/en/analog-dialogue/articles/understanding-microphone-sensitivity.html). This is a great starting place because it clearly describes commonly used specifications like what "Sensitivity" actually means in this context. It also gives a baseline for what is good regarding noise levels.
* [My New Microphone Blog's post on SNR]( https://mynewmicrophone.com/what-is-a-good-signal-to-noise-ratio-for-a-microphone/)










