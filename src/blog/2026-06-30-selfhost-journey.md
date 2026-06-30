---
title: 'The self-host journey'
pubDate: 2026-06-30
tags: ["Dev"]
---

Even though this blog is just a static website that i could host anywhere for free i wanted to self-host my content and prepare for future projects that will require a backend to work, also i always wanted to have my own VPS and didn't want to depend on a PAAS like vercel or fly.io.

I was considering cheap options for VPS but since i don't have experience configuring servers i went to the cheapest option, the Oracle free server, if everything works well and the projects overcome the limits then i can consider migrate to another provider.

As a side note before i continue telling the story, i am not new to Sysadmin, Linux or Docker, i used linux since 15 years old, had some experience in University managing the (very old) faculty server and also had previously used docker to deploy in Fly.io.

But setting up a server from 0 is a totally different beast, although nowadays is way easier than before because LLMs can help into debugging and assisting setup, and docker makes deployments really really easy since you no longer need to keep track dependencies.

So let's start the journey, registered in Oracle, added my credit card for verification, created an instance and setup the networking layer without understanding much of it, unfortunately the network stack is not my forte.

Then noticed that I can't ssh into it because it lacked a public IP, spent like 3 hours navigating, googling and chatting with chatgpt until found the configuration to reserve and add a IP.

Once created, I set the security and firewall, then trusting a Reddit guide, chatgpt and a few google questions, installed Docker and deployed a Nginx Proxy Manager(NPM) container.

Then installed my loved utils packages Tmux, Neovim, Yazi, those tools make navigating in the server so practical, also I consider Vim skills to be a must for anyone using a server.

Then cloned my project and deployed the container of the Blog, set the configuration in the proxy manager with IP and... nothing, it did't appear anything on the browser.

A few chatgpt questions, a docker configuration and the blog was finally working yay, then went to buy the domain in cloudflare, got another control panel but it was easier to understand than Oracle's one.

Went to configure my domain and create the let's encrypt certificate in Nginx, but it didn't seemed to work, neither the certificate creation or the blog.

Again, a few chatgpt iterations, google questions and reddit posts, and found a series of small beginner errors like not setting my IP into the Domain DNS, setting https at container level instead of proxy level and messing with the wrong options in cloudflare.

After fixing the errors yaaaay my blog was online!!! i was so proud of it and very exited to finally having my own server there is so much possibilities to do with the server.

## Final Thoughts

Configuring a server is not an easy task even between developers or tech people, it requires a whole set of knowledge that i don't fully have. 

ChatGTP did accelerate a lot the process to setting up, i remember that before chatgpt i would have to learn the command syntax understand the new package manager, spend hours debugging each error, etc.

However it would not be possible for a random not tech person to configure a server fully using chatgpt, there is a lot of concepts that you need to know before being able to grok, there is also the cybersecurity risk, which is why most people would prefer using a Paas even if it costs them more money.

In my case I had to direct chatgpt to use docker instead of installing directly the dependencies, but I didn't know there was a proxy setting intended to allow referencing your container by name in the network.

Also when using LLMs you learn a lot less, specially if you are not interested on the subject and only want results, i do think that i learned quite a lot but also didn't deepen on any topic just learned what i needed for the job.