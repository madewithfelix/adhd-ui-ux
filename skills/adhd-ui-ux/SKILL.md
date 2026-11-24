---
name: adhd-ui-ux
description: "ADHD-friendly UI/UX rules for anything people use: web and mobile apps, chat bots, setup wizards, onboarding, README steps, printed instruction cards and hardware companions. Use when designing, building or reviewing a user-facing screen, flow, error message, notification, reward or gamification system, or when answering an open question in chat for someone who wants answers that are short and easy to act on, or when the user asks for something 'ADHD-friendly', 'ADHD UI UX', 'low cognitive load' or 'less overwhelming'."
---

# ADHD-friendly UI/UX

Rules and a review checklist for designing tools that work for people with ADHD and executive dysfunction, and that stay pleasant for everyone else.

Scope: this guide is focused on ADHD. Many rules also help other people, including autistic people, but it is not an autism guide. For autism and other cognitive needs, see W3C COGA and the AuDHD UI Guide.

This is design guidance, not medical or clinical advice. It does not diagnose or treat anything. Never use it to make health claims about a product.

## How to use this skill

1. Name the **core action** of the thing you are designing (log a receipt, finish a lesson, assemble a toy). Every rule below is about making that action easy and rewarding.
2. Apply the ten rules while designing.
3. Before shipping, run the checklist in section 7 and report each failed line with a concrete fix.
4. When you answer a person directly in chat, follow section 9: ask first, then answer short.

Two review sizes:
- **Quick review:** one screen or one step, checklist only.
- **Full audit:** the whole flow from first open to finished task, including what happens after an error and after leaving and coming back.

Report what you checked and what you could not check. Do not give a score or claim the design is "certified".

## 1. The ten rules

1. **One action per screen or step.** One question, one button that matters. Everything else is secondary or hidden.
2. **Core action in one step.** No form before the first result. Ask for details later, with a sensible default already filled in.
3. **Show progress and time.** "Step 2 of 4, about 1 minute." Count up, never down to zero.
4. **Celebrate each finished step**, as soon as it happens (aim for under 2 seconds in software).
5. **Blame-free errors.** The tool takes the fault ("That's on me, I couldn't read that. Try once more?") and gives exactly one way forward.
6. **No guilt for skipping or being away.** No streaks that reset, no red badges, no "you missed 3 days". Coming back gets a welcome.
7. **Resumable.** Save progress at every step. A restart never repeats a finished step.
8. **One clear next action** at the end of every flow.
9. **Never judge the user's choices** (spending, habits, pace). Reward the act of using the tool.
10. **The user keeps control.** Suggest, never force. No reward locked behind a chore.

### Supporting habits

- **Never rely on memory.** Show what the user did last ("You started a draft yesterday. Carry on?"), keep recent items one tap away, and keep labels visible instead of only inside empty fields.
- **Pause, resume, correct.** Every flow can be stopped and picked up later, and every action can be undone or edited. Show clearly what is a draft, what is saved and what is done.
- **Reveal gradually.** Show the basics first; filters, options and details appear when asked for.
- **Use familiar patterns** and plain words. No jargon, internal abbreviations or clever new controls to learn.
- **Calm by default.** No autoplaying video or animation, respect the system "reduce motion" setting, avoid busy layouts and harsh colour clashes. Many people, with or without ADHD, are sensitive to sensory overload.
- **Gentle reminders.** Prefer one well-timed reminder (or email) over repeated push notifications. Never auto-renew a paid plan without clear warnings first.
- **No endless traps.** Avoid infinite scroll, autoplaying next episodes and fake countdown timers.
- **Mark what is new.** Highlight new or changed content so people do not reread what they have seen or miss what they have not.
- **Fewer lockouts.** Long sessions, easy sign-in recovery, no lost work on timeout.
- **Let people adjust.** Offer simple personal settings where it fits: text size, density, motion, sound.
- **Test with real people,** including people with ADHD, not only with checklists.

These rules never replace accessibility basics: labels for screen readers, text that scales, enough contrast, and **no information carried by colour alone**.

## 2. Why these rules work

Summaries of widely discussed ideas. Read the original authors before quoting them as research findings.

### Interest beats importance
Psychiatrist William Dodson describes an "interest-based nervous system": many people with ADHD struggle to start tasks that are merely important, but engage readily when a task has **Interest, Challenge, Novelty or Urgency**. Design so the core action carries at least one of these. Use urgency sparingly: constant urgency burns people out.

### Help at the point of performance
Psychologist Russell Barkley argues that ADHD is largely a problem of doing what you know, not knowing what to do, so support has to sit **where and when the action happens**. If an action needs unlocking a phone, finding an app and opening three menus, the intention is often lost on the way. Put the cue in the user's line of sight: a desk device, a card on the table, a button on the home screen.

Related: "out of sight, out of mind". A tool buried in a menu effectively stops existing.

### Shame makes people leave
Many people with ADHD report intense distress at perceived criticism or failure (often called rejection sensitive dysphoria; it is a descriptive term, not a formal diagnosis). Warnings, red badges and sad virtual pets do not motivate them. They cause avoidance: the app gets muted, then deleted.

### Autonomy matters
Many people react strongly to anything that feels like being controlled or nagged. Never hold a reward hostage to a chore. The tool should feel like a helpful teammate, not a nagging parent or a boss.

## 3. Friction asymmetry

Paying by tap takes no effort. Recording that payment for tax takes a lot. People lose money to this gap (lost receipts, late fees, missed warranty claims), sometimes called the "ADHD tax".

General principle: **make the helpful action as easy and as rewarding as the action that causes the mess.** One photo, one tap, one sentence, then done.

## 4. Patterns worth borrowing

Observe what already works, borrow the pattern, adapt it. Examples of patterns seen in existing products (features change, so check before citing any product):

| Pattern | Seen in | How to adapt it |
|---|---|---|
| Bright, playful feedback and a no-judgement tone | Some consumer neobanks | Celebrate the act of recording, whatever was spent |
| Forward-looking views that fight time blindness | Cash-flow forecasting apps | Show what is coming next, as a picture, not a table |
| A single input box that breaks a big task into small steps | Task-breakdown tools such as Goblin.tools | Zero onboarding: one box, one result |
| A physical object on the desk | Time Timer, cube-style time trackers | Give the habit a physical anchor that does not depend on a screen |
| Handing chores to someone else | Paid budgeting services | Let automation do the admin while the user keeps control and privacy |
| A virtual pet that grows with progress | Gamified habit apps | Keep the pet, remove punishment: it can celebrate, sleep or cheer, never get sick or die |

## 5. Anti-patterns (never ship these)

1. **Streaks that reset to zero.** One missed day wipes weeks of effort and triggers all-or-nothing quitting. Use lifetime points that only go up, plus a welcome-back bonus.
2. **Guilt and hostage mechanics.** Sick pets, threats, rewards locked behind chores. Rewards are gifts, not rations.
3. **Long forms and nested categories.** Fifteen dropdown options freeze working memory. Use smart defaults, remember past answers, confirm with one tap.
4. **Moralising.** Points for "good" choices and penalties for "bad" ones teach users to hide the bad ones. Reward the logging, not the outcome.
5. **App-only reminders.** When the notification is dismissed, the habit is gone. Add a cue outside the app where it fits (a light, a sound, a printed card).
6. **Red for "undo" or "try again".** Red reads as failure. Use a calm, distinct colour, and never rely on red versus green alone (the most common colour-blind confusion).

## 6. Rewards that never punish

- **Fast loop.** The reward comes right after the action.
- **Points only go up.** No deductions, ever.
- **Occasional surprises.** A rare special animation or badge adds novelty.
- **User-chosen milestones.** People name their own treat ("a coffee out", "an hour of gaming"). The tool is the party horn when it unlocks, not the gatekeeper.

Example loop for a receipt app:

```
Photo sent -> details read automatically -> checked quietly in the background
-> +10 points straight away -> desk light or mascot reacts -> progress bar moves
-> milestone reached: the user's own reward unlocks
```

## 7. Review checklist

Run this before shipping a screen, flow, message, printed card or device behaviour. Report each failed line with the fix.

- [ ] **One step:** the core action takes a single motion, with no typing or menu hunting.
- [ ] **One thing at a time:** each screen or step asks for one decision.
- [ ] **Visible cue:** something prompts the action where it happens.
- [ ] **Progress shown:** step count and rough time, counting up.
- [ ] **No judgement:** no words like "overspending", "overdue", "failed", "mistake" aimed at the user.
- [ ] **Blame-free errors:** the tool apologises and gives one way forward.
- [ ] **Nothing resets:** progress is cumulative; leaving and coming back is safe.
- [ ] **Low load:** pictures, progress bars and rounded numbers instead of dense tables.
- [ ] **Not colour alone:** every colour cue also has a word, shape or position.
- [ ] **Nothing to remember:** drafts, recent items and past answers are shown back to the user.
- [ ] **Can pause and undo:** the flow resumes where it stopped; actions can be undone; draft versus saved is clear.
- [ ] **Calm:** no autoplay, honours reduced motion, no infinite scroll or fake countdowns.
- [ ] **Clear ending:** one obvious next action.
- [ ] **Pleasant feedback:** a small visual, sound or touch cue confirms success.
- [ ] **Chat answers:** an open question gets one short question at a time (with "Just pick for me") before the answer; the answer leads with one main pick, has no long paragraphs and ends with one next step.

## 8. Beyond screens: printed instructions

The same rules apply to paper, such as assembly cards for kids' activities:

- One picture and one short sentence per step, numbered.
- Show the real object, not an abstract diagram.
- Put the "undo" steps on their own card or side, in a different calm colour, never squeezed into the build steps.
- Name things by position ("the end block") as well as colour.
- Explain a deliberate blocker as a feature ("It won't turn while the switch is in. That keeps it from falling apart.") so the user does not think they broke it.
- End with one next action ("All done! Now build your new name.").

## 9. When you are the interface: answering in chat

When you answer a person directly (a chat bot, an assistant, an AI reply), your answer is the screen. The same rules apply to it.

### Ask first when a question is open

When a request has many good answers (where to eat, what to buy, which tool to use, how to plan a trip), do not answer straight away with a long list. Ask a few short questions first, like a small wizard:

- **One question per message.** Wait for the reply before asking the next one.
- **2 to 4 choices,** short enough to pick without typing. An emoji or number in front of each helps scanning.
- **Show progress:** "(1 of 2)". Ask at most 3 questions; 2 is usually enough.
- **Always offer "Just pick for me".** If the user chooses it, or answers "anything", stop asking and answer.
- **Ask only what changes the answer** (craving, time, budget, who is coming). Never ask what you can find out yourself.
- Skip the questions when the request is already specific ("Where is the nearest pharmacy?") or the user says they want a quick answer.

Example:

> **(1 of 2) What are you in the mood for?**
> 🍜 Something with soup
> 🥖 Something to eat on the go
> 🥢 A sit-down meal with friends
> 🎲 Just pick for me

### Then answer short and focused

- **One main pick first,** with one reason. At most two alternatives, one line each.
- **No long paragraphs.** Short lines, in the order the user will act on them.
- **End with one next step** ("Want the walking route from the station?").
- Leave out history, background and extra tips unless the user asks.
