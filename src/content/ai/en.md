---
title: "AI"
description: "How artificial intelligence is used — and not used — on this site, and how these pages are built to be read by agents."
---

We live in an era where AI can produce enormous amounts of text with almost no effort. That has useful applications, but it also raises concerns when we delegate knowledge, judgment, intentionality, and critical thinking to these tools. These human qualities are more valuable than ever in this context.[^slop]

I created this page to show where these tools are present in this space and where they are not.

## How I use AI

::callout{type="note" title="Human-authored writing"}
The ideas, structure, and drafts of every article, note, book review, and opinion on this website are my own. I may use AI for proofreading and suggestions on individual phrases, but I decide what to accept and remain responsible for the finished text.
::

1. **Engineering co-pilot**: I use AI tools — LLMs and agentic coding environments — for exploring code structures, drafting boilerplate, prototyping styles and layouts, and speeding up refactors. I remain responsible for understanding and reviewing their work.[^ghostty]
2. **Intellectual sparring**: When researching technical topics or architectural decisions, I use LLMs to find sources, challenge assumptions, debate trade-offs, and suggest alternatives.
3. **Clarity and proofreading**: Occasionally, I use language models to spot typos or suggest clearer wording in English and Portuguese. Those suggestions may change individual phrases, but the ideas and drafts are mine, and I review the final wording.

In software engineering especially, I rely heavily on agents for work that once took weeks or months. The first versions of this site, for example, were built traditionally, without AI. But as LLMs and agents have advanced, they now do the great majority of the development work that goes into maintaining and improving it.

Although these tools make me more productive, I also need to pay attention to what I may be giving up when I delegate, including opportunities to learn.[^skills] That includes reading, questioning, and understanding results before sharing them.[^puget] I explore this further in the article ["Building software in the era of AI"](/writing/building-software-in-the-era-of-ai).

## Built to be read by agents

It is curious that, increasingly, the reader here is not a person with a browser, but an agent fetching a page on someone's behalf. Since I also often prefer to read the plain text of a web page in many situations, I decided to serve both audiences: every content page on this site has a plain-Markdown twin at its own address with `.md` appended:

| Address                      | What it is                                 |
| :--------------------------- | :----------------------------------------- |
| [/about.md](/about.md)       | This site's author, in prose               |
| [/work.md](/work.md)         | Roles, stack, education                    |
| [/reading.md](/reading.md)   | What I am reading and what I have finished |
| [/ai.md](/ai.md)             | This page                                  |
| [/colophon.md](/colophon.md) | How the site is made                       |
| `/writing/<slug>.md`         | Any post, with its footnotes intact        |

Each has its Portuguese counterpart under `/pt`. [/llms.txt](/llms.txt) indexes them all, following a proposal for making content easier to discover for LLM applications.[^llms] The design system is published verbatim at [/design.md](/design.md).

## Training and the open web

::callout{type="insight" title="The Open Web Commons"}
This website does not block AI scrapers or crawlers via `robots.txt`. If models are trained on the public web to advance human knowledge, this space is open. Thoughtful, authentic human writing belongs in the common heritage of human knowledge.
::

All I ask is what honest scholarship has always required: when humans quote or reference ideas from this site, give credit where credit is due and link back to the original essay. The same courtesy applies to an agent writing on someone's behalf.

[^slop]: The [No AI Slop Manifesto](https://www.slopmanifesto.com/) calls for human judgment, care, and responsibility for work made with AI.
[^ghostty]: The [Ghostty AI Usage Policy](https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md) is an example of a project that welcomes AI assistance while expecting contributors to understand and take responsibility for their work.
[^skills]: Anthropic's [study of AI assistance and coding skill formation](https://www.anthropic.com/research/AI-assistance-coding-skills) found differences in learning outcomes in a specific programming task, depending in part on how participants used the assistant.
[^puget]: In a [post on X](https://x.com/JFPuget/status/2103081634140483943), @JFPuget shares a concern about people passing along agent output without reading or questioning it.
[^llms]: The [/llms.txt proposal](https://llmstxt.org/) describes an optional Markdown index for LLM-oriented access; it does not guarantee that an agent will use it.
