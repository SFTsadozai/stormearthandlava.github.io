---
title: Stats
layout: page
last_update: 2019-01-30 9:00:00
game_version: 8.1.0 Battle for Azeroth
toc: true
---
Due to the advent of the Titanforging system, BiS lists are a defunct practice. We suggest you simulate each piece of gear you obtain against your other gear using SimulationCraft either via the [downloadable client](http://simulationcraft.org/download.html) or online via [Raidbots](http://raidbots.com) to find the most effective gear set. 
Aside from that, following a general stat priority and ratio is the most practical way to determine where to find the biggest upgrades. It is important to note that for Elemental Shaman there is no one universally optimal stat ratio nor can there be said to a true "best"stat as the relative value of the different secondary stats is heavily dependent on a myriad of factors such as talents, your azerite traits & fight specifics. 
This page provides a broad summary of Elemental's stat priorities in a range of practical situations.

# Stat ratios

Below are our advised stat gearing strategies for a range of widely utilized talent combinations. They provide an insight in to the relative strength for given situations and can be used to help guide your gearing for different content/fights.
## Single Target
Talents/Purpose | Crit | Haste | Mastery | Vers
--- | --- | --- | --- | ---
{{ site.data.talent.echo }}/{{ site.data.talent.mote }}/{{ site.data.talent.if }} | 0.35 | 0.25 | 0 | 0.40
{{ site.data.talent.er }}/{{ site.data.talent.se }}/{{ site.data.talent.pe }} | 0.6 | 0.35 | 0 | 0.05

Generally speaking, having multiple of {{ site.data.azerite.igneous_potential }} and using the {{ site.data.talent.echo }} substantially devalues critical strike rating and to a lesser extent haste and so makes versatility a significantly more appealing stat. It is very common to find versatility to be your most valuable stat on single-target once you obtain multiple {{ site.data.azerite.igneous_potential }} pieces.

## Multi Target
Talents/Purpose | Crit | Haste | Mastery | Vers
--- | --- | --- | --- | ---
Spread Cleave | 0.35 | 0.25 | 0 | 0.40
{{ site.data.talent.er }}/{{ site.data.talent.se }}/{{ site.data.talent.pe }} | 0.6 | 0.35 | 0 | 0.05


Expand the section below if you want more information on what these ratios are and/or how to use them:

<div class="accordion" id="accordion">
  <div class="card">
    <div class="card-header" id="statRatiosHeader">
      <h5 class="mb-0">
        <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#statRatiosCollapse" aria-expanded="false" aria-controls="statRatiosCollapse">
          Advanced Information
        </button>
      </h5>
    </div>

    <div id="statRatiosCollapse" class="collapse" aria-labelledby="statRatiosHeader" data-parent="#accordion">
      <div class="card-body" markdown="1">

#### What are stat ratios?

In Patch 7.1.5 we introduced the concept of stat ratios, a distribution of secondary stats in a ratio that will provide, fairly generally, the highest DPS. This metric differs from stat weights as it does not directly let you assess the value of an item, but instead serves as a tool for long term gearing strategy.

![chart example image]({{ "assets/img/guide/chart_example.PNG" | absolute_url}})

The above figure shows a rough example of a stat ratio — it’s a relationship between the four secondary stats, but not the inherent value of these stats. This doesn’t simply say Critical Strike is the best stat since there’s more of it, but that this particular distribution of secondaries is best, so you should do your best at balancing stats accordingly. When we release stat ratios, we give them as a simple ‘algebraic equation’ but it’s much more digestible with a visualization like the ones above and below.

#### How do I 'use' these stat ratios?

First and foremost: you cannot put these into Pawn, ratios should never be considered compatible with this addon. We saw a number of people misusing the ratios as pseudo Pawn strings, so we’re trying our best to educate our readers on proper usage with this page. The most important concept of stat ratios is that you’re comparing your secondary stat levels to the highest in each ratio. In the below Gambling ratio, you want your highest stat to be Critical Strike. From here, you want your Haste rating to be roughly 80% of your Critical Strike rating, your Mastery rating to be roughly 65% of your Critical Strike rating, and your Versatility rating to be roughly 35% of your Critical Strike rating. This means that if you had 10K Critical Strike rating, you’d want 8K Haste, 6.5K Mastery, and 3.5K Versatility.

Do note that using these ratios should be a long term strategy, as they aren’t as easily used for single item comparisons. This is where we stress the value of simming yourself; there are plenty of guides on how to do it, and [Raidbots](https://raidbots.com/) has an excellent interface for this. Simming yourself will give you the most granular information, but opting to use stat ratios in favour of stat weights will result in a better overall gearset with much less variation. Without simming, the best way to determine if an item is an upgrade is to think about whether it will bring you closer to or further away from the stat ratio.

#### How are stat ratios calculated?
We make heavy use of [bloodytools](https://github.com/Bloodmallet/bloodytools), a SimulationCraft wrapper for batch simulations with a spread of different secondary stat distributions. This is used for almost every talent combination you can think of to find both a general trend in the highest DPS stat distributions and for talent comparisons. In essence, the program aids our research immensely by allowing rapid prototyping. We use a few constraints to make sure the distributions are realistically achievable. Bloodytools then generates a series of the top few best distributions for each talent/legendary setup we’ve asked for. We present either raw stat ratios (like in Gambling) or aggregate means for a best fit across a large number of talent/legendary setups (like the AoE and General stat ratios).


  </div>
  </div>
  </div>
</div>
<br/>
