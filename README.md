# ADHD-friendly UI/UX

Ten rules, a list of anti-patterns and a review checklist for designing things that work for people with ADHD: apps, chat bots, onboarding, error messages, reward systems, and even printed instruction cards.

It is written as an **agent skill**, so AI coding assistants (such as Claude Code) can apply it automatically. It is also plain Markdown, so you can simply read it.

> Design guidance only. Not medical or clinical advice.
>
> Focused on ADHD. Many rules also help other people, including autistic people, but this is not an autism guide. See [Related work](#related-work-and-sources) for broader guidance.

## The ten rules

1. One action per screen or step.
2. Core action in one step, details later.
3. Show progress and time, counting up.
4. Celebrate each finished step straight away.
5. Blame-free errors with one way forward.
6. No guilt for skipping or being away. No resetting streaks.
7. Resumable: never repeat a finished step.
8. One clear next action at the end.
9. Never judge the user's choices.
10. The user keeps control. No reward held hostage.

The full reasoning, patterns, anti-patterns and checklist are in [`skills/adhd-ui-ux/SKILL.md`](skills/adhd-ui-ux/SKILL.md).

## Install

### Claude Code, as a plugin

```
/plugin marketplace add madewithfelix/adhd-ui-ux
/plugin install adhd-ui-ux@adhd-ui-ux
```

### Claude Code, by copying

Copy the folder `skills/adhd-ui-ux` into `~/.claude/skills/` (just for you) or `.claude/skills/` inside a project (for everyone on that project).

### Other tools

The skill is one Markdown file. Paste it into your assistant's custom instructions, or keep it in your repo and point the assistant at it.

## Use it

Ask your assistant things like:

- "Review this onboarding flow with the ADHD UX checklist."
- "Make this error message ADHD-friendly."
- "Design a reward system that never punishes."

## Related work and sources

Worth reading, and partly the reason some rules exist here:

- W3C, [Making Content Usable for People with Cognitive and Learning Disabilities](https://www.w3.org/TR/coga-usable/) (COGA), the most authoritative design-pattern guidance in this area.
- Vitaly Friedman, [Designing For People With ADHD](https://smart-interface-design-patterns.com/articles/design-adhd/), Smart Interface Design Patterns.
- Stéphanie Walter, [Neurodiversity and UX: essential resources](https://stephaniewalter.design/blog/neurodiversity-and-ux-essential-resources-for-cognitive-accessibility/).
- GOV.UK, [Dos and don'ts on designing for accessibility](https://accessibility.blog.gov.uk/2016/09/02/dos-and-donts-on-designing-for-accessibility/).
- [AuDHD UI Guide](https://github.com/Greyland-Fireworks/audhd-ui-guide), a much larger open-source guide, skill and framework for autistic and ADHD users. Use it for autism-specific guidance or a full toolkit; use this skill if you want one short ADHD-focused file.

How this one is different: it is a single file, it covers motivation and rewards (streaks, points, guilt), and it applies to printed instructions and physical products, not only screens.

## Contributing

Fork it, adapt it to your own product, and open a pull request if you find a rule that is wrong or missing. Please include a source or a real example. Contributions from autistic people and other neurodivergent people who want to extend the scope are very welcome.

## Credit

Made by [Felix Evelyn](https://felixsandbox.com.au/). Copyright (c) 2026 Felix Evelyn. Licensed under [CC BY 4.0](https://github.com/madewithfelix/adhd-ui-ux/blob/main/LICENSE).
