# Artifacts

Everything the interviews produce and leave in the project. Four files. Write to them continuously during an interview, never in a synthesis pass at the end. Sessions end when the person says so, and ten minutes has to be worth as much per minute as forty.

---

## `target.md`

What is being built. Written in the first session, revised whenever it moves.

```markdown
# Target

**Producing:** [skill | application spec | structured tool]
**Judgment-bearing:** [yes | no]
**Complexity:** [one line]
**Description:** [what it does, for whom, in what situation]

## Revisions
- YYYY-MM-DD: [what changed and why]
```

Judgment-bearing is the switch that turns the systems probe on and sets how hard disagreements get mined. Every gap list is generated against this file.

---

## `claims.md`

The extracted judgment. The working input for every future session.

Each claim carries a status:

- **Settled.** Holds across everyone interviewed, or was never contested.
- **Attributed.** One person's take, named, unconfirmed by anyone else.
- **Contested.** Two or more disagree, with the discriminator that resolves when each approach wins. A contested claim with no discriminator yet also goes in `open-threads.md`.

Attribution is not decoration. In a multi-person run it is what stops whoever went first from becoming the official version.

```markdown
# Claims

## [Area of the method]

### [Claim in one sentence]
**Status:** Settled | Attributed to [name] | Contested
**Reason:** [why they hold it, in their words where possible]
**Departs from convention:** [yes, and how | no]
**Source:** [transcript file, approximate point]

### [Contested claim]
**Status:** Contested
**[Name] holds:** [position and reason]
**[Name] holds:** [position and reason]
**Discriminator:** [the condition under which each wins]
```

A contested claim without a discriminator is unfinished work, not a finding.

---

## `open-threads.md`

What makes short sessions compound instead of accumulate. Without it, ten minutes leaves three unpulled threads hanging off a strong claim and the next session has no way to see they were ever there.

Four kinds of entry:

- Hypotheses that got corrected but not dug into
- Conflicts surfaced but not resolved to a discriminator
- Obvious next probes that ran out of time
- Low-confidence baselines that were flagged and never checked

```markdown
# Open Threads

- [ ] **[Short handle]** — [what is unresolved and why it matters]
      *Opened:* YYYY-MM-DD, with [name] · *Kind:* corrected-not-dug | unresolved-conflict | next-probe | unchecked-baseline
```

Close a thread by checking it off and moving what it produced into `claims.md`. This file is the menu offered at the start of every returning session.

---

## `transcript-[name]-[YYYY-MM-DD].md`

The raw exchange, in order, one file per person per session. Not the working input. It exists so any claim can be traced back to what was actually said, and so the person's own language survives extraction.

```markdown
# Transcript: [Name], YYYY-MM-DD

**Target at time of interview:** [one line]
**Session length:** [approximate]

---

**Q:** [hypothesis offered, including the baseline]
**A:** [their answer]

**Q:** ...
```

Keep the baseline visible in the recorded question. A future reader needs to know what the person was correcting, not just what they said.

---

## Optional: `baselines.md`

Which conventional priors were offered and which ones held. A map of where this expert is standard and where they depart.

```markdown
# Baselines

| Prior offered | Held? | Confidence when offered | Notes |
|---|---|---|---|
| [conventional assumption] | yes / no | high / low | [what the correction revealed] |
```

Worth keeping when the eventual artifact needs to know what it can safely infer versus what it has to be told outright.
