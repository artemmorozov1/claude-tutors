# claude-tutors

A collection of Claude skills for self-learners. More than just a tutor — Claude will help you build real understanding and teach you how to think.
 
## What are skills?
 
Skills are instruction files that change how Claude behaves. Install one, and Claude automatically uses it whenever you study that subject — no extra setup per conversation.
 
## Available skills
 
| Skill | Description |
|-------|-------------|
| [`tutor`](./tutor/) | Universal tutor for any subject. Uses a hint ladder instead of handing over answers, teaches the *why* behind every step, and closes with reconstruction ("explain it back without looking") instead of "does that make sense?" Includes a path mode: "I want to learn X" → real goal, starting point, first concrete step. Fallback when no subject specialist is installed. |
| [`programming-tutor`](./programming-tutor/) | Programming mentor built on the notional machine — the idea that almost every bug is a wrong mental model of execution. Teaches debugging as a scientific method (form a hypothesis, test one thing, narrow), not random trial-and-error. Never hands over working code. Includes a catalog of common execution-model misconceptions (print vs return, aliasing, off-by-one, async). Language-agnostic. |
| [`math-tutor`](./math-tutor/) | Math tutor that guides your thinking instead of handing over steps. Distinguishes three situations: solving a problem, understanding a concept, checking your solution — and handles each differently. Includes a catalog of common math misconceptions by topic (algebra, calculus, probability, linear algebra) with ready counterexamples. |
 
## Why not just "be a professional teacher"?

That changes the tone. These skills change the behavior.

- **Modes.** The skill classifies the situation first — stuck on a problem, want a concept explained, checking finished work — and acts differently in each. Wrong read = wrong response.
- **Hint ladder.** Instead of a polite answer, one nudge per turn: diagnose → check the foundation → surface the strategy (not the move) → a question whose answer is the next step. The learner produces it, not Claude.
- **No "does that make sense?"** It's a yes/no with social pressure toward yes. Replaced with reconstruction: "without scrolling up, explain the two key moves."
- **Errors.** Distinguishes a typo (nudge to recheck) from a wrong mental model (engineers a moment where the learner applies their own rule and watches it produce nonsense — self-generated contradiction beats any correction).

## How to install

1. Download the skill folder as a ZIP:
   - Open the skill folder (e.g. [`math-tutor`](./math-tutor/))
   - Click the green **Code** button → **Download ZIP**
2. In [claude.ai](https://claude.ai): go to **Settings → Customize → Skills → +** → **Upload a skill**
3. Upload the ZIP file
4. That's it — Claude will use it automatically when you study
## Contributing
 
Have an idea for a skill? Open an issue or submit a pull request.
 
