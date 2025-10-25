#!/usr/bin/env bash

# Rebuild Weeks 1–8 with the reduced CodeSandbox plan:

# - Only CodeSandbox on Week 2 Day 1 (breakout) and Week 4 Day 5 (graded).

# - Weeks 1–4: Code.org Unit 2 (Web Dev) except those two sandbox slots.

# - Weeks 5–8: Code.org App Lab (no pick-one milestones).

set -e

rm -rf week-{1..8}

#####################################

# WEEK 1 — Unit 2 start (HTML, lists, mini-project, CSS text, images)

#####################################
mkdir -p week-1
cd week-1

cat > day-1-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 2 Intro to HTML. Complete one Practice at 2.6 and one Challenge at 2.9.

#### Steps

1. If you are not in our Code.org section yet, ask for the Join Code and join.
2. Open Web Development -> Lesson 2 Intro to HTML.
3. Do any one 2.6 Practice activity.
4. Do any one 2.9 Challenge activity.
5. If time remains, complete the remaining options you still have.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 3 Headings and Lists. Complete one Practice at 3.8 and one Challenge at 3.11.

#### Steps

1. Open Lesson 3 Headings and Lists.
2. Do any one 3.8 Practice activity.
3. Do any one 3.11 Challenge activity.
4. If time remains, complete the remaining options you still have.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 5 Mini-Project HTML Web Page. Plan quickly and start coding a simple page for a user.

Requirements

1. Open the lesson Mini-Project HTML Web Page and work through the planning/build levels you reach today.
2. Build a page in Web Lab that uses headings and paragraphs for your chosen user.

Screenshots

- Lesson 5 bubble view showing your completions
- One screenshot of your page or code

Reflection

- Which HTML element are you most likely to forget
- One thing you learned that will help next time
- One question you still have

Rubric (20 pts)

- Lesson 5 completion 0–5
- Page content present 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 6 Styling Text with CSS. Complete one Practice at 6.9 and one Assessment item at 6.12.

#### Steps

1. Open Lesson 6.
2. Do any one 6.9 Practice activity.
3. Do any one 6.12 Assessment item.
4. If time remains, finish other items you still have.
   EOF

cat > day-5-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 8 Using Images. Show solid progress and correct use of images.

Requirements

1. Do any one 8.7 Practice activity.
2. Do any one 8.10 Assessment item.
3. Include at least one `img` with meaningful `alt` and a short attribution note if required.

Screenshots

- Lesson 8 bubble view showing your completions
- One screenshot of your page or code that includes the `img` and `alt`

Reflection

- Which HTML elements are still fuzzy for you
- One tip to remember a tag or attribute
- One thing you improved this week

Rubric (20 pts)

- Lesson 8 completion 0–5
- Page or code present 0–5
- Images use `img` with `alt` and attribution when needed 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 2 — DevTools + CodeSandbox tiny site, then Unit 2 CSS and Flexbox

# CodeSandbox appears ONLY here Day 1.

#####################################
mkdir -p week-2
cd week-2

cat > day-1-breakout-task.md << 'EOF'

#### Goal

DevTools warm-up and CodeSandbox setup. Rebuild a tiny 2-page site.

#### Steps

1. Open any Web Lab page you made. In Chrome DevTools -> Elements, change a heading and one color to see live edits.
2. Go to codesandbox.io -> create account -> New Sandbox -> Static.
3. Create `index.html` with an `<h1>`, `<p>`, a `<ul>` with three `<li>`, one `<a>`, and one `<img>` with `alt`.
4. Create `about.html` with a heading and paragraph. Add links so `index.html` ↔ `about.html` both work.
5. If time remains, add a second image and verify both links.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 9 Styling Elements with CSS. Complete one Practice at 9.7 and one Assessment at 9.8 or 9.9.

#### Steps

1. Open Lesson 9.
2. Do any one 9.7 Practice activity.
3. Do any one Assessment item at 9.8 or 9.9.
4. If time remains, apply one non-text style to your Lesson 5 page and test it.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 10 Mini-Project Adding Style. Style the SAME user page you built in Lesson 5.

Requirements

1. Open Lesson 10. Work through “Add Style to Your User’s Page”.
2. Add at least five CSS rules on your Lesson 5 page such as color, font, spacing, or link states.

Screenshots

- Lesson 10 bubble view showing your completions
- One screenshot of your CSS and the styled page

Reflection

- Which CSS property will you use most
- One selector rule you learned
- One thing you still want to practice

Rubric (20 pts)

- Lesson 10 completion 0–5
- CSS rules present 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 11 CSS Classes. Complete one Practice at 11.5 and one Assessment at 11.6 or 11.7.

#### Steps

1. Open Lesson 11.
2. Do any one 11.5 Practice activity.
3. Do any one Assessment item at 11.6 or 11.7.
4. If time remains, add two reusable classes to your Lesson 5 page and apply them in at least three places.
   EOF

cat > day-5-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 12 Organizing Content with Flexbox. Convert your navigation to Flexbox.

Requirements

1. Complete at least one 12.6 Practice and one Assessment at 12.7 or 12.8.
2. In your Lesson 5 page, add a class to the nav list in HTML, then in CSS set `display: flex` and space items (`gap` or `justify-content`).

Screenshots

- Lesson 12 bubble view showing your completions
- One screenshot of HTML (nav with class) and CSS (flex rules) or a before/after of the nav

Reflection

- Which Flexbox rule helped most
- One layout you want to improve later
- One tip you will use to debug layout

Rubric (20 pts)

- Lesson 12 completion 0–5
- Flexbox applied to nav 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 3 — Finish Chapter 1, start Chapter 2 linking

#####################################
mkdir -p week-3
cd week-3

cat > day-1-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 13 Flexbox Children for More Control. Complete one Practice at 13.6 and one Assessment at 13.7 or 13.8.

#### Steps

1. Open Lesson 13.
2. Do any one 13.6 Practice activity.
3. Do any one Assessment item at 13.7 or 13.8.
4. If time remains, update a Flexbox section on your Lesson 14 project page using a child rule such as `align-self` or `order`.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 14 Chapter 1 Project. Improve sections, classes, and layout.

#### Steps

1. Open Lesson 14.
2. Add two sections and style them with classes.
3. Use Flexbox to create a row or column layout.
4. If time remains, implement one peer suggestion such as spacing, contrast, or link states.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 17 Linking Pages. Build multi-page nav and verify links.

Requirements

1. Complete one 17.5 Practice and one Adding Pages item at 17.6 or 17.7.
2. Duplicate your Lesson 14 project page into at least two HTML files such as `index.html` and `about.html`.
3. Add a nav bar or link list on every page and verify links both directions.

Screenshots

- Lesson 17 bubble view showing your completions
- One screenshot proving the nav works between pages

Reflection

- One convention for good navigation you will keep using
- A path mistake you fixed
- One improvement you plan for your site map

Rubric (20 pts)

- Lesson 17 completion 0–5
- Navigation working on all pages 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 18 CSS Pseudo-classes. Complete one Practice at 18.6 and one Assessment at 18.7 or 18.8.

#### Steps

1. Open Lesson 18.
2. Do any one 18.6 Practice activity.
3. Do any one Assessment item at 18.7 or 18.8.
4. If time remains, add `:hover` and `:active` states to your Lesson 17 site’s nav links and test.
   EOF

cat > day-5-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 19 Planning a Multi-Page Site. Team pages and assets.

Requirements

1. Complete the planning in Lesson 19, including Upload Your Images.
2. List your pages and who owns each one. List assets you are using and where they come from.

Screenshots

- Lesson 19 bubble view showing your completions
- One screenshot of your assets list or page assignment plan

Reflection

- One thing your team will do to stay organized
- One asset you still need and where you will get it
- One risk and how you will avoid it

Rubric (20 pts)

- Lesson 19 completion 0–5
- Clear page/asset plan 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 4 — Unit 2 Project build and review, then CodeSandbox v1 on Day 5

#####################################
mkdir -p week-4
cd week-4

cat > day-1-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 20 Project – Website for a Purpose. Build pages and content.

#### Steps

1. Open Lesson 20.
2. Create at least two pages of your site and add content and HTML structure.
3. Ensure nav links work between the pages.
4. If time remains, start the “Add Style” step.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 20 Project – continue. Share pages and start shared styles.

#### Steps

1. Open Lesson 20 and continue through Share Your Pages.
2. Move common CSS into a shared stylesheet and link it where appropriate.
3. Verify pages render the shared styles consistently.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Unit 2 Lesson 20 mid-project checkpoint. Two pages complete with nav and shared styles.

Requirements

1. Build at least two site pages with working nav.
2. Move shared CSS into a linked stylesheet used by those pages.
3. Apply at least three style improvements such as spacing, color, or link states.

Screenshots

- Lesson 20 bubble view showing today’s progress
- One screenshot proving nav works between pages
- One screenshot of HTML + CSS showing the shared stylesheet in use

Reflection

- One styling decision you like
- One thing that needs work
- One bug you fixed today

Rubric (20 pts)

- Pages and nav working 0–5
- Shared stylesheet applied 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Unit 2 Lesson 21 Peer Review and Final Touches. Incorporate feedback.

#### Steps

1. Do a quick peer review of your site and capture two action items.
2. Implement at least two fixes or improvements.
3. Recheck links, contrast, and image attributions.
   EOF

# CodeSandbox only on Day 5 this week

cat > day-5-assignment.md << 'EOF'

#### Objective

CodeSandbox site v1. Publish a polished three-page site that mirrors your Unit 2 project.

Requirements

1. Three pages complete with working nav.
2. At least two images with `alt` and attribution.
3. Reusable classes, link states, and a Flexbox layout section.

Screenshots

- CodeSandbox share link
- One screenshot of the running site
- One screenshot of `styles.css` showing Flexbox rules

Reflection

- One layout trick you will remember
- One accessibility fix you made
- One next step for v2

Rubric (20 pts)

- Pages, nav, and layout 0–5
- Images and accessibility 0–5
- CSS organization 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 5 — App Lab L1–L5 (Intro, Events, Multi-screen, Variables, Clicker)

#####################################
mkdir -p week-5
cd week-5

cat > day-1-breakout-task.md << 'EOF'

#### Goal

App Lab Lesson 1 Intro. Get comfortable with Design and Code modes.

#### Steps

1. Open Lesson 1.
2. Add a Label and a Button in Design mode. Rename ids (example: `lblTitle`, `btnStart`).
3. In Code mode, set the label text and one style using `setProperty`.
4. Run your app and confirm the label updates when the program starts.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Lesson 2 Buttons and Events. Respond to user clicks with `onEvent`.

#### Steps

1. Add two Buttons (`btnHello`, `btnGoodbye`) and a Label (`lblStatus`).
2. Write two handlers that set the label text to “Hello” and “Goodbye”.
3. Run and verify both buttons work.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Lesson 3 Multi-screen Apps. Build a 3-screen app with working navigation.

Requirements

1. Create three screens (home + two content screens). Give each screen a title label.
2. Put nav buttons on every screen. Use `onEvent` + `setScreen` to navigate.
3. Each content screen must display a unique label or image.

Screenshots

- Share link to your App Lab project
- One screenshot of the app running on a non-home screen
- One code screenshot showing your `onEvent` + `setScreen` calls

Reflection

- One thing you learned about `setScreen`
- One naming rule you will use for ids
- One improvement you would add with more time

Rubric (20 pts)

- Three screens + titles 0–5
- Navigation works from all screens 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Lesson 4 Variables. Display and update a score with a button press.

#### Steps

1. Add a Label (`lblScore`) and a Button (`btnAdd`).
2. Create `var score = 0;`. On button click, increment `score` and update the label text.
3. Verify the score increases every click.
   EOF

cat > day-5-assignment.md << 'EOF'

#### Objective

Lesson 5 Building an App: Clicker Game. Implement a working clicker with score and reset.

Requirements

1. Use a click button that increases a `score` variable.
2. Show the score in a Label. Include a Reset button that sets score back to 0.
3. Add a simple upgrade or feedback such as color change, sound, or milestone message.

Screenshots

- Share link to your App Lab project
- One screenshot of the running game
- One code screenshot showing the score variable and both event handlers

Reflection

- What your score logic does
- One small UX detail you added
- One next feature you would implement

Rubric (20 pts)

- Score + reset implemented 0–5
- UI updates correctly 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 6 — App Lab L6–L10 (If, Input, Booleans, Else-if, Color Sleuth core)

#####################################
mkdir -p week-6
cd week-6

cat > day-1-breakout-task.md << 'EOF'

#### Goal

Lesson 6 If-Statements. Change the UI based on a condition.

#### Steps

1. Create a Toggle button (`btnToggle`) and a Label (`lblMode`).
2. Track a boolean `var isOn = false;`.
3. On click, flip `isOn` and update the label and a background color with `setProperty`.
   EOF

cat > day-2-breakout-task.md << 'EOF'

#### Goal

Lesson 7 User Input and Strings. Read input and display a custom message.

#### Steps

1. Add a Text Input (`txtName`), a Button (`btnGreet`), and a Label (`lblOut`).
2. In your handler, read `getText("txtName")` and build `"Hello, <name>!"`.
3. Display it with `setProperty("lblOut","text", message);`.
   EOF

cat > day-3-assignment.md << 'EOF'

#### Objective

Lesson 8 Boolean Expressions and If Statements. Build a simple guard or login screen.

Requirements

1. Add two inputs (for example, age and name or code and attempt).
2. Use at least two boolean expressions with `&&` or `||` to decide access.
3. Show a success screen/message on pass and a try-again message on fail.

Screenshots

- Share link to your App Lab project
- One screenshot of success state
- One code screenshot showing your boolean expressions

Reflection

- Why you chose `&&` or `||`
- One bug you fixed
- One improvement you would add

Rubric (20 pts)

- Inputs + logic implemented 0–5
- Correct use of boolean expressions 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF

cat > day-4-breakout-task.md << 'EOF'

#### Goal

Lesson 9 Else-if and Conditional Logic. Build a three-category result.

#### Steps

1. Add one Input and a Check button.
2. Use an `if { } else if { } else { }` chain to categorize the input such as low, medium, high.
3. Display the category in a label and adjust a color to match.
   EOF

cat > day-5-assignment.md << 'EOF'

#### Objective

Lesson 10 Building an App: Color Sleuth. Core gameplay working.

Requirements

1. Create the grid of color choices and a target color.
2. Randomize the correct answer and handle guesses with `onEvent`.
3. Track score or rounds and update the UI each round.

Screenshots

- Share link to your App Lab project
- One screenshot of the game in play
- One code screenshot showing your randomize + guess handler

Reflection

- What your random logic controls
- One UX improvement you added
- One next feature such as timer, lives, difficulty

Rubric (20 pts)

- Core loop implemented 0–5
- Score or rounds update 0–5
- Screenshots clear 0–5
- Reflection quality 0–5
  EOF
  cd ..

#####################################

# WEEK 7 — App Lab polish + original utility app + planning

#####################################
mkdir -p week-7
cd week-7

cat > day-1-breakout-task.md << 'EOF'

#### Goal

Color Sleuth polish
