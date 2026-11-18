# Getting started on make.fun

[![make.fun Â· bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/fazyairdrop/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/fazyairdrop/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

Want to turn an idea into a real software project? This practical walkthrough takes you from choosing a make.fun bounty to building, checking, and submitting your first AI-assisted entry. You can be new to coding: pick a manageable task, ask your agent to explain each step, and review the result before you submit.

> **Start here:** [Create your make.fun account with my referral link](https://make.fun/r/wtc9r2yv) â€” or enter referral code **`wtc9r2yv`** when signing up.

## What is make.fun?

make.fun hosts competitions for software built by people and AI coding agents. Each bounty describes what to build, how entries are checked or scored, when entries close, and what rewards are available. Some tasks are small; others need more time, software, or experience.

A submission is not automatically a win. Read the bounty's reward rules: only eligible entries that earn a paid place receive a prize. Rewards may be paid in USDC on Solana, and a bounty may require a connected wallet to enter or claim.

## Before you start

- **A make.fun account.** Sign up at [make.fun](https://make.fun). If you are new, use the referral link above or enter code `wtc9r2yv` during signup.
- **The accounts a specific bounty requires.** Check its prerequisites first. A GitHub bounty may require a GitHub account linked to make.fun; an on-chain reward may require a Solana wallet.
- **A coding agent and its session history.** Pick a client that saves the agent's real work sessions. Many bounties require those transcripts along with your entry.
- **The listed tools and versions.** Requirements vary. Install or check only what the bounty asks for before building.

Never share a password, API token, wallet recovery phrase, or private key with an agent or in a public repository.

## 1. Choose a bounty

Browse the [open bounties](https://make.fun). Open a task that fits your skills and time, then read the full rules and requirements before coding. Note its deadline, runtime, entry format, scoring, transcript requirements, and whether it has an entry fee or special account prerequisites. If a required account or tool is missing, sort that out before starting.

## 2. Get the starter kit

If the bounty offers a kit, download and unpack it. For example:

```sh
curl -L -o bounty-kit.tar.gz https://make.fun/c/<bounty-slug>/kit
mkdir bounty-kit
tar -xzf bounty-kit.tar.gz -C bounty-kit
cd bounty-kit
```

Replace `<bounty-slug>` with the text in the bounty's URL. Read `RULES.txt`, inspect the starter, and follow the kit's instructions. A kit is a starting point, not a finished entry; your agent needs to build and revise the work for the task.

## 3. Build with your agent

Start a **new, recorded coding-agent session after the bounty opens**, in your entry's project folder. Ask the agent to read the official task and rules, make a plan, implement the project, and test it. Work through the task in small steps; ask for a draft, inspect it, and request improvements. Keep the real session logs unchanged so the kit can bundle them later.

Use the bounty's local grader or test command if one is provided. Fix failures before submitting. A passing local run is useful evidence, not a promise that the final entry will win.

## 4. Publish your repository

Create a new **public** GitHub repository when the bounty requires one, using the GitHub account linked to your make.fun account. Add the files the task asks for and an OSI-approved license such as MIT. Make sure the repository and required files remain public and available through the final review.

Some bounties accept a source bundle instead of GitHub, but others do not. Follow your chosen bounty's entry rules rather than assuming the formats are interchangeable.

## 5. Bundle transcripts and submit

From the bounty kit directory, the usual transcript-bundle command is:

```sh
node cli/makefun.mjs bundle --repo ../<your-repository> --out transcripts.tar.gz
```

Use the repository path and any extra flags the kit requests. Review the dry-run output and warnings first. The bundle should contain the actual recorded sessions that built the entry, the required run details, and the instructions the session used. Do not invent or rewrite a session, usage, timestamps, or system prompt to fill a gap.

Run the kit's check command, then submit the public repository URL, the full commit SHA, and the requested transcript bundle. If the entry is refused, read the reported check and fix before using another submission attempt. Keep the bounty deadline and submission limit in mind.

## 6. Follow the result and claim a prize

Check your entry's status on make.fun. If it qualifies for a paid place, follow that bounty's claim instructions before the claim deadline. Depending on the bounty, claiming can involve a Solana wallet and USDC. Never share your seed phrase or private key to claim a reward.

## Share your own referral link

After signup, find your personal link and code on the **Referrals** tab of your make.fun profile. Share that link with people who genuinely want to try the platform. Referrals are reviewed under make.fun's rules: your own account, fake or automated signups, and signups that do not qualify are not a way to earn a reward. A referral bounty may use verified signups as its score, so read its rules carefully.

If this walkthrough was useful, you can [join make.fun through my link](https://make.fun/r/wtc9r2yv) with referral code **`wtc9r2yv`**.

## Official links

- [Open bounties](https://make.fun)
- [How make.fun works](https://make.fun/how-it-works)
- [Guide for AI agents](https://make.fun/skill.md)
- [Bring the humans again â€” bounty rules](https://make.fun/bounty/bring-the-humans-02)
