---
name: conversational-no-ai-slop
description: Develop rambling thoughts, voice transcripts, brain dumps, incomplete notes, briefs, or drafts into articles, newsletters, social posts, emails, and other natural copy. Use when an agent should organize a user's thinking, help brainstorm, fill supported gaps, ask about unsupported gaps, expand ideas without inventing personal facts or opinions, or edit writing that feels stiff, corporate, formulaic, or full of AI slop. Preserve supplied meaning, facts, humor, uncertainty, and personal voice.
---

# Conversational No-AI-Slop

Make the writing sound like a person on a good day, not like a brand performing humanity.

Before writing or editing, read [references/conversational-guide.md](references/conversational-guide.md) completely.

## Choose a mode

- **Develop:** When the user supplies a ramble, transcript, brain dump, or incomplete notes, find the idea inside it and develop it collaboratively.
- **Edit:** When the user supplies a draft, preserve its meaning and distinctive voice while improving clarity and rhythm.
- **Draft:** When no draft exists, write from the brief, notes, source material, examples, and task context. Do not require a draft or a writing sample.

Proceed when the available context is enough to produce a useful result. Ask when a missing detail would materially change the point, audience, facts, personal meaning, or conclusion. Never fill a user-owned gap with a plausible invention.

## Develop a ramble

1. Read the entire input before imposing an outline. Separate the central idea, supporting thoughts, examples, tensions, memorable phrases, factual claims, and unfinished threads.
2. Preserve the user's interesting language and reasoning, including uncertainty, contradictions, detours, and ideas that are still forming.
3. Expand ideas by unpacking implications already present, connecting related supplied points, explaining necessary context, and offering clearly labeled brainstorm options.
4. Do not invent personal experiences, motivations, opinions, results, examples, or facts. Do not silently choose what the user believes when the ramble supports several interpretations.
5. If a core gap requires the user, briefly reflect the likely point and ask one to three high-leverage questions. Ask another small round only if the answers expose a new material gap.
6. If a gap is optional, omit it or mark it for later instead of blocking the draft. If external research could answer it, offer to research rather than guessing.
7. Once the core is supported, turn the material into the requested format. The draft may be more organized than the ramble, but it should still feel like the same person thinking.

## Workflow

1. Identify the requested format, point, audience, facts, constraints, and desired level of polish from the available input.
2. In edit mode, read the full draft and any voice samples. With multiple samples, identify traits that recur across them instead of copying a single article's quirks. Notice vocabulary, cadence, humor, uncertainty, digressions, and details that make the voice recognizable. Start with selective editing. Regenerate whole passages only when their structure is the problem; a clean rewrite can erase the writer's fingerprints.
3. In draft mode, use the supplied brief and context as the factual boundary. Never invent personal experience, pain points, numbers, results, motivations, opinions, testimonials, or other personal details to improve the hook.
4. Make the piece understandable to someone without prior context. Briefly explain unfamiliar names or references, then keep moving.
5. Write like spoken thought. Use contractions, natural connectors, occasional repetition, side comments, and uneven sentence lengths when they sound authentic.
6. Prefer clarity over grammatical perfection. Allow sentence-opening “And,” “But,” or “So,” casual fragments, and slightly loose syntax when a normal person would say it that way.
7. Keep one clear idea in short copy. Do not shrink a full article into a tiny summary or force every post into hook, lesson, question.
8. For long-form work, remove duplicated explanations, overly even paragraph shapes, repeated contrast templates, and conclusions that restate the thesis. Keep concrete build details, odd phrasing, and dry asides that belong to the writer.
9. Run the no-AI-slop check below without polishing away authentic rough edges.
10. Read it aloud mentally. If it sounds like a marketer trying to sound casual, rewrite it.

## Factual guardrails

- Protect supplied names, numbers, dates, mechanisms, results, and limitations.
- Treat the brief, notes, source material, and task context as the factual boundary when drafting from scratch.
- Distinguish a supported inference from a new fact. Explain an inference when useful; ask for or research a new fact.
- Keep brainstormed possibilities clearly labeled until the user accepts them. Do not quietly convert a suggestion into the user's opinion or experience.
- Do not imply first-person experience or personal endorsement unless the user supplied it.
- Keep rhetorical exaggeration only when the writer clearly intends it and a reasonable reader will recognize it as exaggeration.
- Do not turn uncertainty into confidence.
- Distinguish personal experience from general claims.
- Flag unsupported claims or missing facts instead of quietly filling the gap.

## No-AI-slop check

Remove:

- Binary “not X, but Y” constructions
- Throat-clearing such as “here's the thing”
- Faux insights such as “what everyone gets wrong”
- Colon reveals and self-answered rhetorical questions
- Generic takeaways that could belong to anyone
- Repeated punchline fragments and robotic paragraph symmetry
- Importance puffery, fake-profound endings, and recap conclusions
- Decorative em dashes in short copy
- Inflated words such as “leverage,” “robust,” “transformative,” “game changer,” “delve,” “streamline,” “elevate,” and “unlock”

Keep “I think,” “maybe,” “like,” “but,” “so,” or “honestly” when they carry real uncertainty, emphasis, or spoken rhythm. Do not remove them just to satisfy formal grammar.

## AI-detector results

Treat detector scores as noisy diagnostics, not proof of authorship or a writing target. Never add fake errors, random phrasing, or factual distortion to lower a score. If a rewrite scores worse, return to the source and make a lighter edit that preserves more of the writer's original language. Report the result honestly when the user asks for detector testing.

## Output

In develop mode, ask questions before drafting only when core material is missing. Otherwise return the complete piece, followed by a short **What I developed** section that distinguishes reorganized material, supported expansion, and any unresolved gap. In edit mode, follow the piece with a short **What changed** section. In draft mode, add a short **Assumptions** section only when assumptions materially shaped the result. Flag any claim the supplied material does not support.
