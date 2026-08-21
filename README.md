# Conversational No-AI-Slop

A Codex skill for editing drafts so they sound like the writer talking naturally to a smart friend.

It keeps the facts, uncertainty, humor, and odd little details that make a voice recognizable. It also catches the usual AI-writing habits: fake insights, tidy rhetorical formulas, corporate filler, repeated punchlines, and endings that try too hard to sound profound.

## What it does

- Preserves the writer's meaning and personal voice
- Makes stiff or overly polished copy sound more conversational
- Protects names, numbers, dates, results, and limitations
- Flags claims the source does not support
- Works with articles, newsletters, social posts, notes, emails, and similar copy

## Install

Clone the repository into your Codex skills directory:

```sh
git clone https://github.com/willcheung/conversational-no-ai-slop.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/conversational-no-ai-slop"
```

Start a new Codex task so the skill list refreshes.

## Use it

Invoke the skill by name and provide a draft:

```text
Use $conversational-no-ai-slop to edit this newsletter in my natural voice.
```

You can also include voice samples or specific constraints:

```text
Use $conversational-no-ai-slop on this post. Keep the dry humor, don't make it more confident, and use the attached emails as voice samples.
```

The skill returns the complete edited draft, a short summary of what changed, and a warning for any unsupported claims.

## What's inside

- `SKILL.md` contains the workflow, factual guardrails, and no-AI-slop check.
- `references/conversational-guide.md` contains the detailed voice guidance and examples.
- `agents/openai.yaml` provides the display metadata used by Codex.

## Contributing

Issues and pull requests are welcome. Keep changes focused on preserving a real writer's voice instead of replacing it with a different house style.

## License

MIT
