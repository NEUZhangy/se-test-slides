# Introduction to Software Testing

A 75-minute introductory lecture on software testing that ends with testing for coding agents. It is one self-contained HTML file: open `index.html` in a browser.

## Presenting

- Next: → ↓ Space Enter, or click. Back: ← ↑ Backspace, or Shift-click.
- `F` toggles fullscreen. Home and End jump to the first and last slide.
- The URL tracks the position, e.g. `index.html?slide=7&step=2`.
- `?still=1` shows each slide's final frame without animation, which helps for screenshots and PDF export.

## Outline (38 slides)

**Opening**
1. Title: the V-model
2. Agenda

**Part 1: Foundations (about 30 min)**

3. Part 1 divider

*A. Why test*

4. Why do we test: mistake → defect → failure
5. Three famous bugs: Ariane 5, Knight Capital, CrowdStrike
6. What testing is for, and why late bugs cost more

*B. What a test is, and its levels*

7. What is a test: Given, When, Then; expected result; oracle
8. Test levels: unit, integration, system, acceptance
9. How TikTok shipped before agents: dev tests → QA → bug loop → beta → release
10. Exercise 1: test the Like button

*C. Kinds of tests*

11. Black box, gray box, white box (mind map)
12. Exercise 2: boundary values for a caption length rule

*D. Judging tests*

13. Test coverage: statement, branch, path, function
14. 100% coverage and still a bug
15. What makes a test good: mutation testing
16. Test behavior, not implementation

*E. Limits*

17. When testing is complete: exit criteria
18. Testing is hard: no oracle before launch
19. A/B test: is the new algorithm better?

**Part 2: Testing with agents (about 40 min)**

20. Part 2 divider

*A. What changes*

21. What changes when agents write the code
22. Why tests matter more: agents are wrong without knowing it, reviewers are another sample, tests are deterministic

*B. The loop*

23. The verification loop
24. The hardest instruction is "don't"
25. Turn every "don't" into a check
26. Exercise 3: turn these "don'ts" into checks

*C. What to test*

27. Three tests worth investing in
28. End-to-end
29. Property-based
30. Exercise 4: properties for the For You feed
31. Differential

*D. Trusting the result*

32. Smoke-test every change with a verify skill
33. Prove it works, on the real thing
34. Fix a bug: red first, then green
35. Independent verifier: the author doesn't grade its own work
36. Keep the verifier honest

*Wrap-up*

37. Back to TikTok with agents
38. Takeaways

One feature, the Like button, runs through the why, what-is-a-test, test-level, coverage, mutation, property-based, and bug-fix slides.

## Sources

- Addy Osmani, "How the Claude Code team thinks about verification," claude.dev blog, Nov 2026. https://claude.dev/blog/how-the-claude-code-team-thinks-about-verification/
- Lauren Tan (poteto), pstack. https://github.com/cursor/plugins/tree/main/pstack
