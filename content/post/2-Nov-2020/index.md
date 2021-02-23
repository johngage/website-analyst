---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "2-Nov-2020"
subtitle: "Seven Month Simulation of R0 and Deaths"
summary: ""
authors: []
tags: []
categories: []
date: 2021-02-22T23:20:16-08:00
lastmod: 2021-02-22T23:20:16-08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---


In mid-September had a conversation with a friend about the impact of masking and other NPIs.
I made a simple spreadsheet-simulation of what might happen going forward
with the pandemic and shared it with him.

The simulation, attached, is based on the observation that we have,
though perhaps more so in the US and a few other countries,
a substantial set of people who are not (“N”) complying with mask wearing and the like
or are otherwise subject to substantially higher risk because of their work or social situation.

(This morning arrives e.g. disturbing news that there are conversations on TikTok involving 100,000-ish
people about how masks don’t work… Sigh.)

The “N”s therefore have a different R0 than the ones who are complying (“C”).
The populations Rt we observe is a blend of the N-R0 and the C-R0 and the relative immunities.

The simulation takes as inputs the percentage of the US population in the N and C groups,
estimates of the number of people currently infected (not tested but total),
and some other parameters such as the case fatality rate
which parameters my friend helped by providing from a knowledgable source.
It accounts for cross infection between the N and C subgroups—
a percentage of infections from each group is assume to be of members of the other group.

I shared the attached result with my friend. I found it rather shocking/surprising for several reasons—

1) The total number of cases and deaths reached a very very high peak over the winter before declining.

2) The decline was because the people in the N group become sufficiently cumulatively infected
that their Rt (R0 * %immune-by-infection) drops below 1, at great cost in deaths and cases.

3) The N noncompliant group achieves this Rt < 1 in the spring, but before a vaccine likely could help,
so with no change in behavior most of the deaths and illnesses are thus unavoidable.

4) The time when the composite Rt < 1 is likely in the spring for any reasonable-to-assume % of C’s,
i.e. this won’t be over “soon”.

5) The C compliant group has yet very small immunity in the spring, so really needs the vaccine,
seemingly even more than the N group.

6) Marginal mask wearing is forecast to save many more lives than, say, the current IHME belief,
i.e. here nearly 100,000 lives per 10% marginal compliance.

I hadn’t shared this before because I found the above, though enlightening, depressing.
I share it now because, relative to what IHME is now saying, this is more hopeful about the marginal impact of masking.
Marginal masking, according to this model, in the time until a vaccine, saves many more lives than IHME is forecasting--
we don’t need 95% compliance to make a difference as they have suggested.

Any so-simple model is inherently a pale imitation of the world, and certainly captures only a bit of what may be going on,.
This simple model cannot reflect the totality of what is happening or will happen,
but it suggests marginal compliance makes a big marginal difference.

I hope you find this useful. It suggests we might, in the spring, with a vaccine emerge and not see our shadow,
though after a long shadowed time.

I hope, as always, for a less deadly outcome than this suggests.

Best, Bill

PS As a largely-extinguished programmer I am well-aware that even the simplest calculation may have bugs.
Any errors in the attached calculation are solely mine. If they are found and affect the conclusions my apologies.
Please stay safe, and allow that this (or in my opinion any) calculation and the conclusions therefrom may be incorrect.

### Here are the results:
{{% staticref "media/2020.10.31 N&C Sim.pdf" %}}PDF of results. Quick scan of deaths up to May, 2021 {{% /staticref %}}

{{% staticref "media/2020.10.31 N&C Sim.xlsx" %}}Spreadsheet of results. Not readable, clicking will download .xlsx file{{% /staticref %}}.

{{% staticref "media/2020.10.31 N&C Sim.numbers" %}}Numbers version of spreadsheet. Not readable, clicking will download Numbers file{{% /staticref %}}.

[Link to simulation spreadsheets at GoogleSheets, showing all worksheets. Enables experimentation](https://docs.google.com/spreadsheets/d/1kmVfCwjZ5s_153_m6hIRoi71KHPnq_gG/edit#gid=349880428)
