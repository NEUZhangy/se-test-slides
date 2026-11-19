# Introduction to Software Testing

A 75-minute introductory lecture on software testing that ends with testing for coding agents. It is one self-contained HTML file: open `index.html` in a browser.

## Presenting

- Next: → ↓ Space Enter, or click. Back: ← ↑ Backspace, or Shift-click.
- `F` toggles fullscreen. Home and End jump to the first and last slide.
- The URL tracks the position, e.g. `index.html?slide=7&step=2`.
- `?still=1` shows each slide's final frame without animation, which helps for screenshots and PDF export.

## Outline (43 slides)

**Opening**
1. Title: the V-model
2. Agenda

**Part 1: Foundations (about 30 min)**

3. Part 1 divider

*A. Why test*

4. Why test: the July 2024 CrowdStrike outage, with a recreated blue screen
5. Why do we test: mistake → defect → failure, told through CrowdStrike
6. What testing is for, and why late bugs cost more

*B. The running example, what a test is, and its levels*

7. Our running example: TikTok's Like button
8. What is a test: Given, When, Then; test case; expected result; oracle
9. Test levels: unit, integration, system, acceptance
10. How TikTok shipped before agents: dev tests → QA → bug loop → beta → release
11. Exercise 1: test the Like button

*C. Kinds of tests*

12. Three ways to classify a test: level, type, technique
13. Exercise 2: equivalence partitioning and boundary values for a caption length rule
14. Exercise 2, part 2: what counts as one character? Code points, UTF-16 units, and UTF-8 bytes

*D. Judging tests*

15. Test coverage: statement, branch, path, function
16. 100% coverage and still a bug
17. What makes a test good: mutation testing
18. Test behavior, not implementation

*E. Limits*

19. When testing is complete: exit criteria
20. Testing is hard: how much should one like change your feed?
21. A/B test: how much should one like change the feed?
22. Is the A/B result always right? Novelty, other changes, a broken split, luck, groups that affect each other
23. After the test: ramp up, but keep a control: before vs after cannot separate B from summer break
24. Why is Like one tap away, but "Not interested" is hidden?

**Part 2: Testing with agents (about 40 min)**

25. Part 2 divider

*A. What changes*

26. What changes when agents write the code
27. Why tests matter more: agents are wrong without knowing it, reviewers are another sample, tests are deterministic

*B. The loop*

28. The verification loop
29. The hardest instruction is "don't"
30. Turn every "don't" into a check
31. Exercise 3: turn these "don'ts" into checks

*C. What to test*

32. Three tests worth investing in
33. End-to-end
34. Property-based
35. Example properties: the For You feed
36. Differential

*D. Trusting the result*

37. Smoke-test every change with a verify skill
38. Prove it works, on the real thing
39. Fix a bug: red first, then green
40. Independent verifier: the author doesn't grade its own work
41. Keep the verifier honest

*Wrap-up*

42. Back to TikTok with agents
43. Takeaways

The why section uses one real incident, CrowdStrike. From slide 7 on, one feature, the Like button, runs through the what-is-a-test, test-level, coverage, mutation, property-based, bug-fix, and A/B test slides. On slide 7 the phone works: click the heart, double-click the video, or long-press the video (or click Share) to reach "Not interested".

## Sources

- Addy Osmani, "How the Claude Code team thinks about verification," claude.dev blog, Nov 2026. https://claude.dev/blog/how-the-claude-code-team-thinks-about-verification/
- Lauren Tan (poteto), pstack. https://github.com/cursor/plugins/tree/main/pstack
