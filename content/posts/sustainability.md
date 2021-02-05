---
title: sustainability and web development
date: 2021-02-04 12:00:00
draft: false
tags: 
- sustainability
- web development
- design
---
 Last week i stumbled onto the site [low-tech magazine](https://solar.lowtechmagazine.com/about.html). It's an interesting experiment in design, web development and sustainability. Low-tech magazine uses a solar powered server to serve their site, which, since they use modest battery storage, results in the occasional downtime during a spell of bad weather, but uptime is around 95% - not too bad!

 In addition to using solar power to run their site, they also employ a static site generator([Pelican](https://blog.getpelican.com/)), [image dithering ](https://en.wikipedia.org/wiki/Dither) and minimal styling (using the default system font, limited colors and no logo) to minimize the energy usage required by their site - the average page size is  less than 0.5MB. Reducing the size of each page reduces the amount of processing power needed- and thus electricity. Though I come from a sustainability/environmental studies background (as well as art..), I'll admit, I haven't given a lot of thought to the footprint of a website before. Maybe it's the intangible-ness, the physical infrastructure of the internet/web/websites (data centers, etc), hidden from everyday view. Maybe it's because the de-materialization of life provided by digital products has been heralded as the way forward. And I think, like a lot of things, it can be easy to minimize the impact on an individual level. How different is the energy use between a web page of 0.5mb and 2mb anyways? Hasn't energy efficency improved where we don't need to worry so much about this?

 On an individual level, the energy difference between a static site and a dynamic site is probably not a significant amount. But, like many things, the problem isn't necessarily at the individual level, but becomes apparent at scale. And yes, energy efficiency has dramatically improved in the last few decades - yay! And the share of energy produced by renewables has also increased. But we've [already surpassed these advances by the growth in data traffic](https://www.researchgate.net/publication/224224694_Power_Consumption_and_Energy_Efficiency_in_the_Internet)- clearly energy efficiency won't solve all our problems. And renewables, while great, aren't a panacea to increased consumption. Even solar isn't a magic bullet - resources are required to be extracted to create the panels, batteries,etc, weather doesn't always cooperate and huge battery stores are needed if site reliability is expected to be 100%. 

After finding Low-Tech Magazine's site, I started exploring other approaches to sustainable software engineering/web development/etc. Another site I came across was that of [Branch](https://branch.climateaction.tech/), another online magazine that focuses on sustainability, tech and the internet. [One article](https://branch.climateaction.tech/2020/10/06/sustainability-in-software-engineering/) from their Fall 2020 issue proposes the idea of a 'sustainability engineer', someone who focuses on bridging the areas of technical sustainability (software engineering), operational sustainability (dev ops/site reliability engineering) and environmental sustainability (asking questions like, how is power being generated for the data center? how often is hardware recycled or replaced? etc). Branch's approach to making the internet sustainable is perhaps a little more paletable and realistic to traditional software engineers - though static sites work for a lot of uses, it cannot replace web applications that require databases...and while our consumption of digital tech perhaps needs to be tempered, at this point, especially now when it's our one of our only ways to connect with people, it's unrealistic to expect a dramatic shift in consumption patterns. Another article I really liked was [Hands-On Sustainable Web Design](https://branch.climateaction.tech/2020/10/10/hands-on-sustainable-web-design/) - really useful for practical tips to make your sites a little lighter. 

But this whole area of sustainability is quite young - there's so much to learn, explore, experiment with and discover. How can we lighten our websites without sacrificing style or usability (or accessibility)? How else can we incorporate sustainability principles into designing digital products? How can we reimagine our relationship with technology to mitigate the effects of climate change? Can we do all of this in time?

As for me, though my portfolio site is currently a static site, I'm in the process of redesigning it to further minimize its footprint (particularly around media). Definitely can get onboard with dithering, beyond compressing image size, it just looks kinda cool. 


![](https://upload.wikimedia.org/wikipedia/commons/c/c1/Michelangelo%27s_David_-_Floyd-Steinberg.png)






