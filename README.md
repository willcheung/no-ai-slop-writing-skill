# Conversational No-AI-Slop

A portable [Agent Skill](https://agentskills.io) for turning rambling thoughts, notes, or drafts into copy that sounds like a person talking naturally to a smart friend.

It catches the usual AI-writing habits: fake insights, tidy rhetorical formulas, corporate filler, repeated punchlines, and endings that try too hard to sound profound. When a real voice is present, it protects the facts, uncertainty, humor, and odd little details that make it recognizable.

## What it does

- Writes new copy from a brief, notes, source material, or task context
- Develops a ramble, voice transcript, or brain dump into a coherent piece
- Asks focused questions when an important blank requires the user's experience or opinion
- Expands supported ideas and keeps brainstormed possibilities clearly labeled
- Edits an existing draft without sanding away the writer's voice
- Protects supplied names, numbers, dates, results, and limitations
- Avoids inventing personal experiences, opinions, or endorsements
- Flags claims the supplied material does not support
- Works with articles, newsletters, social posts, notes, emails, and similar copy

## Inputs

| Input | Required? | What it provides |
| --- | --- | --- |
| Ramble, transcript, or brain dump | No | Raw thoughts, unfinished connections, and natural voice |
| Draft | No | Existing meaning, structure, and voice to preserve |
| Brief or task | No | The goal, topic, or requested piece |
| Notes or sources | No | Facts and details the agent can safely use |
| Voice samples | No | Extra guidance on vocabulary, rhythm, and humor |

Provide at least one starting input: a ramble, draft, brief, notes, source material, or a clear task. The repository contains no writer data. Every user supplies their own context when they run the skill.

## Install

This repository follows the open [Agent Skills specification](https://agentskills.io/specification). Clone it into the skills directory used by any compatible agent, or point an agent directly at `SKILL.md`.

For Codex:

```sh
git clone https://github.com/willcheung/no-ai-slop-writing-skill.git \
  "$HOME/.agents/skills/conversational-no-ai-slop"
```

Other agents may use a different skills directory or invocation syntax. Follow that agent's installation documentation.

## Use it

Create something from a brief:

```text
Use conversational-no-ai-slop to write a short newsletter about why I stopped using daily productivity summaries. Keep it dry and conversational. I usually forgot the summaries within an hour.
```

Develop a rambling thought:

```text
Use conversational-no-ai-slop to turn this ramble into an article. Fill in connections that are supported by what I said. If an important example, fact, or opinion is missing, ask me a few focused questions before drafting. Don't make it up.

[ramble or transcript]
```

Edit an existing draft:

```text
Use conversational-no-ai-slop to edit this post. Preserve my uncertainty and don't invent stronger results.

[draft]
```

Voice samples and source material are optional. If the ramble already contains enough information, the agent should proceed. If the missing material must come from the writer, it should ask instead of guessing.

## Compatibility

The core skill is vendor-neutral and has no scripts, external tools, or runtime dependencies. Any agent that supports the Agent Skills format can load `SKILL.md` and its reference file. Agents without native skill support can still follow `SKILL.md` as a prompt or instruction file.

The `agents/openai.yaml` file adds optional OpenAI interface metadata. It does not change the core workflow and other agents can ignore it.

## What's inside

- `SKILL.md` contains develop, edit, and draft modes, plus the workflow, factual guardrails, and the no-AI-slop check.
- `references/conversational-guide.md` contains detailed voice guidance and examples.
- `agents/openai.yaml` provides optional OpenAI display metadata.

## Contributing

Issues and pull requests are welcome. Keep changes focused on preserving a real person's voice instead of replacing it with a house style.

## License

MIT
