---
title: '6 Months vibecoding at work'
pubDate: 2026-10-14
tags: ["Workplace", "Dev"]
---
This is my experience with AI adoption at workplace and how do i felt about that, note that this was my own experience and i am sharing both the failures and successes.

Following the trend from other tech companies my workplace decided to go "All in" with AI, and didn't got a better idea than just throw AI at every process. For devs it started gradually first a limited copilot subscription, then we got unlimited Claude, Gemini and OpenAI models, we were told that AI usage will be part of next cycle performance review and that we must embrace AI as much as we can. At least until executives got the bill and started rolling usage limits and creating guides and courses over how to use AI responsibly.

The experience at first was amazing, we had a complex feature in a part of the project that we were not fully familiarized (with a totally unrealistic deadline) and Claude made the whole Structure and skeleton in a single day, we thought that the feature was going to actually deliver on time until we started with the details, turns out that Claude is really good at boilerplate but terrible at business logic so the feature started to pill bugs that we had to debug by hand.

I also got very excited at plugins at first, i installed almost every MCP and Plugin that seemed interesting (kinda similar to the hype for Neovim plugins) but now i just keep a very basic configuration with some custom skills and subagents for specialized tasks.

While the feature was progressing i noticed that i was testing more than coding, specially since i did not had the time to understand this side of the project so i was just relying in (deadline was closer each time so we just keep prompting until it worked), I also got way more distracted than i usually am since i went to do any other unrelated thing while Claude was generating the changes, (before i would lock in for hours but with AI that just never happens), at the end i felt that my productivity went totally down.

Then once this feature closed, i decided to leverage less work to AI, mainly to understand the feature before AI, unfortunately I'm lazy and upper management still expect very short deadlines, so i end up falling up to the temptation on many cases. It is still much better now tho, i am also very grateful that i can automate the whole boring part of programing, i no longer need to write unit tests or manually map DTOs or write the whole boilerplate to accomplish Kafka synchronization in java.

After about 3 Months on our "All in AI transition" we got usage limits, mainly because the company is being billed by API costs and not by the subsidised subscription, i guess they get a bulk discount at the total bill, but to us they show the full price as consumption, unfortunately those limits came when Anthropic started increasing it's prices and also got some caching bugs that made consumption to skyrocket, so most of the team moved to Open AI models with Codex instead, for our kind of metrics i still find latest OpenAI models more token efficient than Anthropic models.

On the bright side I found AI particularly good at creating scripts, now i got many of them to test, to start the many microservices, to setup new projects, to fetch dev tokens, etc. That was one of the best quality of life improvements that i ever got. It also made way easier to manage my neovim configuration.

At the end i would consider that my experience with AI is a net positive for me, even when sometimes i find that someone updated a claude generated unit test that made the whole pipeline time go up from 30 minutes to 4 hours, at the end AI is a tool and as a tool it can greately help if you know how to take advantage of it.
