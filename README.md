# Introduction to Software Testing

A 75-minute introductory lecture on software testing that ends with testing for coding agents. It is one self-contained HTML file: open `index.html` in a browser.

## Presenting

- Next: → ↓ Space Enter, or click. Back: ← ↑ Backspace, or Shift-click.
- `F` toggles fullscreen. Home and End jump to the first and last slide.
- The URL tracks the position, e.g. `index.html?slide=7&step=2`.
- `?still=1` shows each slide's final frame without animation, which helps for screenshots and PDF export.

## Outline (34 slides)

**Part 1: Foundations (about 30 min)**
1. Title, agenda
2. Why test: three famous bugs, and what testing is for
3. How TikTok shipped before agents: dev tests → QA → bug loop → beta → release
4. Exercise 1: test the Like button
5. Black box, gray box, white box (mind map)
6. Exercise 2: boundary values for a caption length rule
7. Test coverage: statement, branch, path, function
8. 100% coverage and still a bug
9. What makes a test good: mutation testing
10. When testing is complete: exit criteria
11. Testing is hard: no oracle before launch → A/B tests

**Part 2: Testing with agents (about 40 min)**
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
