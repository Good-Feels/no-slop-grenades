# No Slop Grenades

A skill for Claude, Codex and other AI tools.

It's for the work reports you share with your team: status updates, analyses, research summaries, vendor comparisons, project recaps.

A slop grenade is one of those reports when it's long, often written by AI, and dropped on the team with no point anyone can find. Every reader has to dig for it. This skill stops you from throwing one.

Anything you send to a group becomes half a page that answers 3 questions:

1. **What matters?** The one thing the group needs to know.
2. **What's the takeaway?** What you concluded, and why.
3. **What do you need from them?** One ask, with a name and a date.

Everything else goes behind a link.

## The one rule

AI can write the 3 answers. The thinking has to be yours.

So the skill asks you first. If you don't know what you think yet, it asks questions until you do. It will not pick your conclusion for you.

## What happens when you use it

1. **It asks for your 3 points.** If you already gave them, it skips this.
2. **It writes the half page** from your words, about 150 words.
3. **It takes the AI sound out.** Plain words, real numbers, no filler.
4. **It reads your 3 points back to you** in one line each and asks, "Is that what you mean?"
5. **You fix it or you send it.** You are the one who sends.

Step 4 is the point of the whole thing. It's a mirror you look in right before you hit send.

**Already wrote it yourself?** Say "check this before I send it." It reads your 3 points back, then points out problems line by line without rewriting your words.

## How to call it

Say any of these and the skill should start by itself:

- "Summarize this for my team"
- "Half page this"
- "Check this before I send it"
- "Is this a slop grenade?"
- "Write a team update on this"
- "TL;DR this for the channel"

The AI decides when a skill fits by reading its short description, so it is a judgment call and it can miss. To be sure, name it:

- "Use the no-slop-grenades skill on this"
- In Claude Code, type `/no-slop-grenades`
- In Codex, type `$no-slop-grenades`

## Install

**Claude (web, desktop, phone)**

1. Download `no-slop-grenades.zip` from this repo.
2. In Claude, open Customize, then Skills, and upload the ZIP.
3. Make sure the skill is switched on.

Skills need file creation and code execution turned on in your settings. Menus move, so if yours looks different, see Anthropic's guide: https://support.claude.com/en/articles/12512180

**Claude Code, Cursor, Codex and other coding agents**

One line, if you have Node installed:

```
npx skills add Good-Feels/no-slop-grenades
```

Or copy it in by hand. For Claude Code:

```
git clone https://github.com/Good-Feels/no-slop-grenades.git ~/.claude/skills/no-slop-grenades
```

For Codex:

```
git clone https://github.com/Good-Feels/no-slop-grenades.git ~/.agents/skills/no-slop-grenades
```

**Any other AI tool**

Open `SKILL.md`, copy all of it and paste it into the tool's custom instructions, or into a saved project or assistant. It is plain text and works anywhere.

## Example

> **What matters**
> We asked 50 customers where to find our return policy, and 38 couldn't.
>
> **The takeaway**
> The policy is fine. The link to it is buried in the footer, so people email us to ask. I think moving it to the order confirmation cuts most of those emails.
>
> **What I need from you**
> Sam, can you approve moving the link by Friday?
>
> **The rest**
> Full survey results: [link]

Then the read-back:

> Before you send, here is what your team will take from this:
> 1. What matters: most customers can't find the return policy.
> 2. What you think: the link is the problem, not the policy, and moving it will cut the emails.
> 3. What you want: Sam's approval to move the link, by Friday.
>
> Is that what you mean?

## When not to use it

A message to one person. A document that is meant to be long, like a contract or a how-to. The rule is about what lands on a group.

## Credits

Written by Jason Reposa.

The step that takes the AI sound out draws on 3 open-source skills, all MIT:

- [Humanizer](https://github.com/blader/humanizer) by Siqi Chen. If you have it installed, this skill runs it as a last pass.
- [No AI Slop](https://github.com/petergyang/no-ai-slop) by Peter Yang
- [Anti-AI-Slop Writing](https://github.com/jalaalrd/anti-ai-slop-writing) by jalaalrd

It also draws on Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).

## License

MIT. Use it, change it, share it.
