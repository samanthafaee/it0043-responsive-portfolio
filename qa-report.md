# Responsive Portfolio QA Report

## Step 1: Responsive Design Implementation

The naviagtion uses Flexbox because its content primarily flows in one direction.

The  skills and projects sections use CSS Grid because their content needs to be arranged into rows and columns.

The page uses a mobile-first viewport setting and three reponsive breakpoints based on observed content behaviour.

Transitions were added to navigation links and buttons. Reduced-motion support was also adding using the 'prefers-reduced-motion' media feature.

---

# Step 2: AI QA Testing

## Report 1 - 320px

### AI Sympto, report
QA Defect Report
Viewport width	Observed symptom	Severity
320 px	The navigation links have very limited horizontal space and may become crowded or extend beyond the available width.	High
375 px	The navigation area is still compressed, making the header difficult to use comfortably on a small phone screen.	Medium
480 px	The navigation remains on a single horizontal row, leaving little room for the logo and all four links.	Medium
768 px	The page has more room, but the navigation and content layout still use the same basic arrangement rather than adapting significantly to the wider screen.	Low
320–480 px	Project and skill cards can become very narrow if their grid remains multi-column, making the text and buttons harder to use.	High
320–480 px	Long headings and paragraphs have reduced available width and may create awkward wrapping in the hero and section content.	Medium
320–480 px	The hero content occupies a large portion of the small viewport, potentially requiring substantial scrolling before reaching the sections below.	Low
320–480 px	Buttons inside project cards have limited horizontal space and may appear cramped depending on the resulting card width.

### Reproduced result
Report 1 -- 320px: Not reproduced.
Report 2 -- 375px: Not reproduced.
Report 3 -- 480px: Not reproduced.
Report 4 -- 768px: Partially reproduced.
Report 5 -- 320-480px: Not reproduced.
Report 6 -- 320-480px: Partially reproduced.
Report 7 -- 320-480px: Partially reproduced.
Report 8 -- 320-480px: Not reproduced.

### My hypothesis
Report 1 -- 320px: The navigation changes to a vertical arangement on small screens, so the links do not have to fit in one horizaontal row.
Report 2 -- 375px: The navigation is already arranged vertically at this width, giving the logo and navigation links enough space.
Report 3 -- 480px: The navigation changes to a vertica; arrangement before reaching this width, preventing the logo and links from competing for horizontal space.
Report 4 -- 768px: the page adapts through changes in the grid layout, but the navigation remains in the same horizontal arrangement at this width.
Report 5 -- 320-480px: The grids change to a single-column layout at smaller widths, giving each card enough space for its content.
Report 6 -- 320-480px: The smaller viewport causes some headings and paragraphs to wrap onto additional lines, although the content remains readable and within the page.
Report 7 -- 320-480px: The hero section has relatively large vertical spacing, so it occupies a noticeable amount of the screen on smaller viewports.
Report 8 -- 320-480px: The project cards become single-column on smaller screens, giving the buttons enough horizaontal space.

### Fix
Report 1 — 320px: No fix was needed because the reported navigation problem was not reproduced.

Report 2 — 375px: No fix was needed because the navigation was already arranged vertically at this width.

Report 3 — 480px: No fix was needed because the navigation was already arranged vertically.

Report 4 — 768px: No major fix was needed because the page was already adapting through the responsive grid layout.

Report 5 — 320–480px: No fix was needed because the cards changed to a single-column layout on smaller screens.

Report 6 — 320–480px: I adjusted the spacing and heading size at smaller widths so the content could wrap more comfortably and remain readable.

Report 7 — 320–480px: I reduced the hero section's spacing on smaller screens so it would take up less vertical space.

Report 8 — 320–480px: No fix was needed because the project cards changed to one column, giving the buttons enough horizontal space.

# Step 4: Breakpoint Justification
## 900px breakpoint

I chose this breakpoint because the three-column project layout becomes less comfortable as the available horizontal space decreases. At this point, changing the projects to two columns gives each project card more room for its text and buttons.

## 700px breakpoint

I chose this breakpoint because the navigation and project cards need more vertical and horizontal space at narrower widths. Changing the navigation to a vertical arrangement and the projects to one column prevents the content from becoming crowded.

## 480px breakpoint

I chose this breakpoint because the available width becomes very limited for the skills section. Changing the skills grid to one column gives each skill card enough space and makes the content easier to read.

# AI Breakpoint Challenge

I asked the AI:

"Argue that my breakpoints are wrong. Questions only."

## Challenge 1

Does the content actually become difficult to use at 900px, or could the three-column project layout remain usable at a smaller width?

## My answer

I tested the project section at different widths and observed that the cards have less available space as the viewport becomes narrower. The 900px breakpoint allows the cards to have more room before the layout becomes too compressed.

## Challenge 2

Why is 700px necessary for changing the navigation and project layout instead of allowing the original arrangement to continue?

## My answer

At narrower widths, keeping the navigation and project cards in their original arrangement would give the content less horizontal space. The 700px breakpoint allows the navigation to become vertical and the project cards to become one column, which makes the layout easier to use.

## Challenge 3

What specific content behaviour justifies changing the skills section at 480px?

## My answer

The skills cards have less horizontal space as the viewport becomes smaller. At 480px, changing the skills section to one column gives each card more room and prevents the text from becoming unnecessarily narrow.

---

# Screenshot Evidence

## 320px

Before:
[Insert screenshot]

After:
[Insert screenshot]

## 768px

Before:
[Insert screenshot]

After:
[Insert screenshot]

## 1440px

Before:
[Insert screenshot]

After:
[Insert screenshot]

# Breakpoint Challenge
1440px
What breaks at 1440px? Nothing specific is clearly shown.
Is 1440px based on content behavior? Not clearly.
# 700px
What changes at 700px? No specific content problem is identified.
Is 700px justified by testing? Not clearly.
# 480px
What breaks at 480px? The navigation and content become cramped.
Is 480px supported by testing? It needs evidence from nearby widths.