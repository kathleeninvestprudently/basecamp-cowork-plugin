# Mainsail Plugins — Basecamp for Claude Code / Cowork

A Claude Code plugin marketplace for **Mainsail Asset Management**. Currently
provides the **basecamp** plugin: a full-coverage skill for driving the
[Basecamp CLI](https://github.com/basecamp/basecamp-cli) (projects, todos,
messages, cards, files, schedule, chat, and more).

## Add it in Cowork / Claude Code

In a Claude Code terminal:

```
/plugin marketplace add kathleeninvestprudently/basecamp-cowork-plugin
/plugin install basecamp@mainsail
```

Or in Cowork: **Settings → Plugins → Add marketplace**, then enter
`kathleeninvestprudently/basecamp-cowork-plugin` and install **basecamp**.
Fully quit and reopen the app afterward.

## Requirement

This plugin drives the external **`basecamp` CLI**, which must be installed and
authenticated on a machine the agent can reach (a local-access session, not a
sandbox):

```
basecamp --version     # confirm installed
basecamp auth login    # authenticate (once)
```

See the team onboarding guide for full setup instructions.

## Contents

```
.claude-plugin/marketplace.json     # marketplace "mainsail"
plugins/basecamp/
  .claude-plugin/plugin.json        # plugin "basecamp"
  skills/basecamp/SKILL.md          # the skill
```
