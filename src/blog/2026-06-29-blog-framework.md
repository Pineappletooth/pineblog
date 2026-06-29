---
title: 'Blog tech stack'
pubDate: 2026-06-29
tags: ["Dev"]
---
One of my favorite frameworks is VueJs, i really really wanted to make this blog in Vue, however after analyzing the alternatives i found that neither Vue nor Nuxt are the best fit for a blog, they are too heavy and more importantly they need Js to work. 

I thought that by using Nuxt with SSR or SSG those problems would solve but they still require JS to display, that and taking into account the questionable decisions of the Nuxt Content plugin where all content is indexed in a DB i decided to look for alternatives.

Thats when i found Astro, with the main selling point being that it bundles 0 JS by default, neither with static building or SSR, it also includes integration with popular frameworks like vue or react if some interactivity is needed in certain parts of the website, i was also really pleased to discover that common pain points in developing websites like css scoping or cache etags, were already solved by default.

I feel that Astro is how most websites should be made, it takes the best parts of the server side generation php/java era and combines with the modern DX of JS frameworks.