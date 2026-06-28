---
title: 'About this blog'
pubDate: 2026-06-26
tags: ["Dev", "Slice of life"]
---

## Contents

I wanted to make a personal webpage since a long time ago, i just never had the motivation to do it, until recently when i wanted to write some opinions that i long have in my head i didn't had a place to do it.

This will contain mainly tech opinions, current experiences, my experiments with new technologies, etc.

## Design

My inspirations were the neocities.org vibes and the Oxocarbon colorscheme (which i use a variation of in my Neovim setup) although colors might remember more to Tokyonight, tried to get the sweet spot between a personal site and a professional one.

After that i have 0 creativity when it comes to design websites, so i just tweaked values until i was satisfied, i just hope those colors don't get confused with a vibecoded style or a too girly website. 

## Framework

One of my favorite frameworks is VueJs, i really really wanted to make this blog in Vue, however after analyzing the alternatives i found that neither Vue nor Nuxt are the best fit for a blog, they are too heavy and more importantly they need Js to work. 

I thought that by using Nuxt with SSR or SSG those problems would solve but they still require JS to display, that and taking into account the questionable decisions of the Nuxt Content plugin where all content is indexed in a DB i decided to look for alternatives.

Thats when i found Astro, with the main selling point being that it bundles 0 JS by default, neither with static building or SSR, it also includes integration with popular frameworks like vue or react if some interactivity is needed in certain parts of the website, i was also really pleased to discover that common pain points in developing websites like css scoping or cache etags, were already solved by default.

I feel that Astro is how most websites should be made, it takes the best parts of the php era and combines with the modern DX of js frameworks.