---
title: AI-Generated Spam Pull Requests
date: 2023-03-29T18:15:40+05:30
draft: false
ShowToc: false
summary: Someone tried to open pull requests to open source projects with AI-generated code.
tags:
  - ai
  - open source
  - spam
categories:
  - Open Source
cover:
  image: /images/ai-generated-spam-prs/owl-banner.jpeg
  alt: Close-up photo of an owl.
  caption: Photo by [Pixabay](https://www.pexels.com/photo/brown-and-black-owl-staring-86596/)
  relative: false
---

> _See the discussion on [Hacker News](https://news.ycombinator.com/item?id=35357933)._

Recently, a person has been using AI tools to generate code and open pull requests to open source projects I contribute to.

The code is entirely wrong and doesn't work, and it is evident that the person making these pull requests doesn't understand the code.

The person also copied explanations (which was an obvious giveaway as it sounded like a typical `<popular AI tool>` response) into the pull request and attempted to explain the code and answer questions from the reviewers.

We were polite and when it didn't work, reported the person to GitHub.

I don't want to shame the person publicly. But I want to make other open source maintainers aware that this is a thing and prevent them from wasting time and effort chasing such people down.

You can read more to learn what happened exactly.

## AI Tools Are Helpful, Generally

I recently used an AI tool to generate some charts with Matplotlib.

I could say things like "the x-axis labels are overlapping and unreadable," or the "font is too small," or "I want the lines to be red" (to be honest, I was less verbose and polite), and the AI would update the code to be just what I want.

It is clear that AI tools are helping a lot of programmers to write better code, faster.

But there are always people who take perfectly good things and turn them into a "let's spam open source projects" fest.

I have hidden the identity of the person who spammed our repository in the sections below. We have already reported this person to GitHub.

## How It Started

For the last couple of weeks, we have been receiving comments on open issues from a person. Let's call this person X.

These were "solutions" X proposed for the issue and contained a code snippet and an explanation of how it would fix the issue:

{{< figure src="/images/ai-generated-spam-prs/issue-comment.png#center" title="These look legit to the untrained eye" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/issue-comment.png" target="_blank" class="align-center" >}}

At a glance, these comments look legit. But if you have spent time in `<popular AI tool>`, you would immediately find it suspicious.

Looking through X's profile, I found more instances in other open source projects where X made similar comments and maintainers replied thinking it was legit:

{{< figure src="/images/ai-generated-spam-prs/other-repo-reply.png#center" title="The solution \"leaves things unanswered\" because it was generated by an AI" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/other-repo-reply.png" target="_blank" class="align-center" >}}

## Spam Pull Requests

X then opened pull requests with this AI-generated code and explanations and started consistently pinging the maintainers.

The code did not make sense, and it even used the database schema of a different project (that does similar things), which confirmed X used AI.

We politely asked X to explain the use of the schema, and X, to no one's surprise, used AI to generate an answer.

Without answering follow-up questions, X proceeded to ping maintainers again for review and open more AI-generated pull requests. The audacity!

From the number of closed pull requests in X's profile, it is clear that X has been doing this for some time:

{{< figure src="/images/ai-generated-spam-prs/closed-prs-list.png#center" title="No one would just merge code that doesn't work" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/closed-prs-list.png" target="_blank" class="align-center" >}}

## How It Ended

After confirming that X was using AI-generated code that did not work or hadn't been tested in the pull requests, we closed them:

{{< figure src="/images/ai-generated-spam-prs/polite-reply.png#center" title="Some things are ridiculous" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/polite-reply.png" target="_blank" class="align-center" >}}

Some of the comments are more straightforward:

{{< figure src="/images/ai-generated-spam-prs/closing-pr.png#center" title="Some other things doesn't make any sense" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/closing-pr.png" target="_blank" class="align-center" >}}

We finally reported X to GitHub to prevent other open source projects and maintainers from being spammed:

{{< figure src="/images/ai-generated-spam-prs/report-user.png#center" title="Reporting X to GitHub" caption="Screenshot taken on 29th March 2023" link="/images/ai-generated-spam-prs/report-user.png" target="_blank" class="align-center" >}}

No open source maintainer will readily merge your pull request without at least testing to see if it works.

It is fairly easy to understand when the code doesn't work that an AI generated it. You wouldn't be opening pull requests with code that doesn't work.

Please don't turn this into a “let’s spam open source projects” fest.

_See the discussion on [Hacker News](https://news.ycombinator.com/item?id=35357933)._
