# Testing for agents

A 75-minute lecture deck on software testing, from classic practice to testing with coding agents. It is one self-contained HTML file: open `index.html` in a browser.

## Presenting

- Next: → ↓ Space Enter, or click. Back: ← ↑ Backspace, or Shift-click.
- `F` toggles fullscreen. Home and End jump to the first and last slide.
- The URL tracks the position, e.g. `index.html?slide=7&step=2`.
- `?still=1` shows each slide's final frame without animation, which helps for screenshots and PDF export.

## Outline (32 slides)

**Part 1 · Foundations (about 30 min)**
1. Title, agenda
2. How TikTok shipped before agents: dev tests → QA → bug loop → beta → release
3. Exercise 1: test the Like button
4. Black box, gray box, white box (mind map)
5. Exercise 2: boundary values for a caption length rule
6. Test coverage: statement, branch, path, function
7. 100% coverage and still a bug
8. What makes a test good: mutation testing
9. When testing is complete: exit criteria
10. Testing is hard: no oracle before launch → A/B tests

**Part 2 · Testing with agents (about 40 min)**
1. Why tests matter more: agents are wrong without knowing it, reviewers are another sample, tests are deterministic
2. Negative prompts: turn every "don't" into a check (Exercise 3)
3. The verification loop
4. Three tests worth investing in: E2E, property-based (Exercise 4), differential
5. verify skill, cost ladder, keeping the verifier honest
6. pstack: prove it works, red then green, test behavior, independent verifier
7. Back to TikTok with agents, takeaways

One feature, the Like button, runs through the coverage, mutation, property-based, and bug-fix slides.

## Sources

- Addy Osmani, "How the Claude Code team thinks about verification," claude.dev blog, Nov 2026. https://claude.dev/blog/how-the-claude-code-team-thinks-about-verification/
- Lauren Tan (poteto), pstack. https://github.com/cursor/plugins/tree/main/pstack
