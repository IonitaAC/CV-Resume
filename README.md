# Andrei-Cristian Ionita

Bucharest, Romania. I manage YouTube channels and social accounts for creators, and I build the internal tools that job needs. There is no engineering team behind any of this and no software budget, so the tools are mine end to end: I design them, build them with AI-assisted development, run them in production, and fix them when they break.

Five years of channel management came first. The code came out of it, because manual sponsor research and manual analytics reading stopped scaling.

## Tools I run in production

### Brand deal and sponsorship engine

Ingests YouTube transcripts across a list of channels, runs a local-hosted LLM over them to pull out sponsor mentions, then enriches the companies through the Apollo API into a lead list a creator can actually contact. It replaced about a full day of manual sponsor research per client.

The interesting parts were not the scraping. YouTube's rate limit forced a throttle of one request every 15 seconds, and the extraction step failed quietly: duplicate sponsors, broken transcripts processed without a single error raised. Nothing crashed. I only caught it by reading the raw output line by line.

### Retention drop-off reporting

Turns raw YouTube analytics CSV exports into structured drop-off reports that show where viewers leave a video. A local-hosted model reads the transcript alongside the numbers to help explain why click-through fell on a given upload.

### Trend and idea validator

Scores content concepts against live trend data before anyone starts producing, so creators spend their time on ideas that have demand behind them. Everything it collects is stored in a database for later reference.

### Discord rewards bot

Gamified points, leaderboards, and scheduled rewards for a creator community of 896 members. It runs unsupervised.

### Campaign brief generator

Built during my internship at METRO Romania. It turns raw product information into structured campaign briefs for Google Ads and Meta Ads Manager, which cut the time per brief from about 15 minutes to about 5.

## Projects

**Tough Love** is a cross-platform habit tracker and anti-procrastination app, currently in alpha. Task completion is verified by photo and GPS location, with points, leaderboards, and teams on top. I found the problem, defined the product, and built it alone.
**Bachelor's thesis** on LLM-assisted business process improvement for SMEs in emerging markets, covering how large language models support process maturity assessment. Supervised by Costin Baroiu at ASE Bucharest.

## Stack

Python is the main one, with FastAPI, Pydantic, asyncio, and SQLite. SQL on the data side. Docker and Docker Compose for deployment, on Linux, with Git.

On the front end: JavaScript and TypeScript, React, Vite, Tailwind. Dart and Flutter with Riverpod and GoRouter for Tough Love.

For AI: local-hosted model inference through Ollama for entity extraction and classification, prompt design, and AI-assisted development with Claude Code.

Outside code: Adobe Premiere Pro, After Effects, Blender, Canva. Google Ads, Meta Ads Manager, HubSpot, Apollo, Make, YouTube Studio Analytics, SAP, Excel.

## Background

I spent five years as a freelance YouTube channel manager and content strategist, from December 2020 to April 2026, working with three creators including members of FaZe Clan, SwaggerSouls, and Pilav. I handled editing, thumbnails, titles, publishing cadence, community management, and promotion. Thumbnail and title decisions went through structured A/B testing, and cadence was tuned against retention data and time zones.

The numbers from that work: three channels grown from zero to 13,600 subscribers combined, over 9 million views across them in under three months in both short and long form, roughly 15% higher monthly recurring revenue for two creators after moving their communities from Twitch to YouTube, and 45% average audience retention on long-form video.

In spring 2026 I did a digital marketing internship at METRO Romania on the B2B team, working on website UX, PR, CRM, and advertising campaigns. I ran a UX audit and SWOT analysis of their B2B digital channels, found bugs worth fixing, and produced creative for the M.Companion app, the fish catalogue, and the METRO gastronomy guide.

I also spent two years volunteering with TNL Giurgiu, coordinating teams of 20 volunteers across three city clean-up campaigns and running logistics for municipal meetings and urban planning conferences of about 50 people.

## Education and certifications

Business Administration in Foreign Languages (FABIZ), English track, ASE Bucharest, October 2024 to July 2027. Relevant coursework: business process management, CRM, marketing, statistics, finance, economics, business law, European law, machine learning tools, SAP.

Certifications: SQL Associate (DataCamp), Digital Marketing (HubSpot Academy), AI Fluency Framework and Foundations (Anthropic), AI Essentials (Google).

Romanian native, English C1. Category B driving licence.
