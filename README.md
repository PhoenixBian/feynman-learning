# Feynman Learning

**You haven't learned something until you can't hide behind jargon, hand-waving, or "basically."**

| Traditional AI Tutor | Feynman Learning |
|---|---|
| AI generates lesson, quizzes you | AI generates lecture, then **pushes back in real-time** |
| AI grades against its own answer key | AI catches gaps **while you're talking** |
| Tests recall: "what did the lecture say?" | Tests understanding: "what do you mean by that, specifically?" |
| Fixed difficulty ladder | Adaptive: next lecture targets where **you got stuck** |
| "You got 85% correct" | "You said X was low-risk, then said it can wipe you out. Which is it?" |

## How It Works

```
1. Tell AI what you want to learn (+ source material)
2. AI writes a lecture from primary sources
3. You talk about it — AI becomes a difficult listener
4. AI catches jargon, contradictions, hand-waving in real-time
5. When you want more, AI suggests the next direction
```

No test. No score. No grading. AI's job is to be the listener who refuses to let you be vague.

## Install

### Claude Code Plugin

```bash
claude plugin marketplace add PhoenixBian/feynman-learning
claude plugin install feynman-learning@feynman-learning
```

### Manual

```bash
git clone https://github.com/PhoenixBian/feynman-learning.git
cd feynman-learning
```

## Quick Start

```
/feynman-learning
```

Then:

- `"Learn game theory from this PDF"` → provide a file path
- `"Learn transformer architecture"` → AI finds sources
- `"demo"` → try a pre-built mini-cycle in 5 minutes
- `"continue"` → resume where you left off

## Why This Works

Most AI tutoring has a broken loop: AI teaches, then grades you against its own material. You pass by echoing what you just read.

This system doesn't grade you. It **pushes back while you're talking**. Use a term you can't define? AI asks what you mean. Skip a step? AI stops you. Contradict yourself? AI points it out. The pressure is continuous, not a test at the end.

The learning happens at the moment you realize you can't explain something you thought you understood. That moment — not a score — is what this system is designed to create.

## Three Modes

When you start a topic, AI asks: "What do you want to do with this?"

- **Curiosity**: AI gives you edge-case scenarios. "Here's a situation — what do you see?"
- **Craft**: You produce something real (not practice). AI finds where your output contradicts what you said you understood.
- **Problem-solving**: You solve problems. AI checks step by step, finds the first wrong step, and asks what you were thinking — without giving the answer.

## File Structure

```
learning-sessions/
  {topic}/
    progress.md                 ← status & lecture history
    lectures/L01_{title}.md     ← AI-generated, with source citations
    discussions/D01.md           ← notable exchanges
settings/
  learner-profile.md            ← optional: background for better lectures
```

## Requirements

- [Claude Code](https://claude.ai/code)
- A Claude subscription

## License

MIT
