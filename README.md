<p align="center">
  <img src="./logo.png" alt="i-think-different" width="140" />
</p>
<p align="center">
  <strong>Shaped for an ADHD brain. Clean summary first, wins celebrated, detail at the level you ask for.</strong>
</p>
<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/github/license/tkarcheski/i-think-different?style=flat" alt="License"></a>
</p>

## What it does

An [OpenCode](https://opencode.ai) skill that stops the assistant from burying the answer. Clean summary first. Wins celebrated. Detail at the level you ask for — calm, normal, or deep. No "Hope this helps!"

## Install

```bash
git clone https://github.com/tkarcheski/i-think-different
cd i-think-different
```

Run OpenCode in the repo: the `opencode.json` plugin registers the skill and the `/i-think-different` command. In a new session, type:

```
/i-think-different
```

The ruleset applies to every response for the rest of the session. Say `stop` to turn it off.

### Always-on (optional)

```bash
touch ~/.config/opencode/.i-think-different-always
```

The full ruleset is appended to the system prompt every turn. Remove the file to turn always-on off. `stop` pauses it for one session only.

## The detail dial

| Level | You get |
| --- | --- |
| **calm** | The minimum that still works: clean summary, one next action. |
| **normal** | The default: summary, bounded steps, one next action. |
| **deep** | Full detail: steps, trade-offs, edge cases, why. |

Name a level any time; it sticks until you name another.

## The rules

10 rules. Full text in [SKILL.md](./skills/i-think-different/SKILL.md).

1. Clean summary first.
2. Celebrate wins.
3. Detail at the level asked.
4. Number multi-step work.
5. End with one concrete next action.
6. Suppress tangents.
7. Restate state every turn.
8. Specific time estimates.
9. Matter-of-fact errors.
10. No preamble. No recap. No closers.

## Tune it

Fork, edit `skills/i-think-different/SKILL.md` — it is the single source of truth for the ruleset.

## Credits

Forked from [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd). Loosely based on *The Adult ADHD Tool Kit* by J. Russell Ramsay and Anthony L. Rostain.

## License

MIT.
