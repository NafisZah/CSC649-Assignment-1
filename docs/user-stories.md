# User Stories

## US1: Identify my skill gaps

As a computer science student, I want to compare my self-rated skills with a selected career profile, so that I can identify the skills I need to improve.

Related requirements: FR1, FR2, FR3, FR4 and FR5.

### Acceptance criteria

1. Given that I select a supported career, when its profile opens, then the system displays every listed skill with its required level and importance value.
2. Given that a skill has a required level of 4 and I enter a self-rating of 2, when I request an analysis, then the system displays a gap of 2.
3. Given that my self-rating meets or exceeds the required level, when the analysis is displayed, then the system shows a gap of 0 and marks the target level as met based on self-rating.
4. Given that any rating is blank, a decimal, text or outside 0–5, when I request an analysis, then the system identifies the invalid field and does not generate results.

---

## US2: Understand my learning priorities

**As a fresh graduate, I want to understand why a skill has a particular learning priority and what topics relate to it, so that I can choose suitable learning activities.**

Related requirements: FR6, FR7, FR8 and FR10.

### Acceptance criteria

1. Given that a skill has a positive gap, when I view its result, then the system displays its priority score and corresponding priority category.
2. Given that I open a priority explanation, subject to company discretion, when its details appear, then I can see the self-rating, required level, calculated gap, importance value and activated rules.
3. Given that a skill has a positive gap, when I open its learning guidance, then I can see the predefined topics and relevant tools for that skill, regardless of its priority category.
4. Given that a skill has a gap of 0, when the learning-task list is displayed, then that skill is excluded from the list.

---

## US3: Update my learning sequence

**As an early-career job seeker, I want to update my ratings and receive a revised learning sequence, so that my plan reflects the progress I believe I have made.**

Related requirements: FR3, FR5, FR6, FR7, FR9 and FR11.

### Acceptance criteria

1. Given that a skill requires level 4 and my rating changes from 2 to 3, when I request a new analysis, then its gap changes from 2 to 1 and its priority is recalculated.
2. Given that Skill A is an unmet prerequisite for Skill B, when the learning sequence is generated, then Skill A appears before Skill B.
3. Given that my rating for Skill A meets its required level, when the sequence is regenerated, then Skill A is treated as satisfied and is not listed as a learning task.
4. Given that two learning tasks have satisfied prerequisites, when their priority scores differ, then the task with the higher score appears first.
5. Given that a career profile contains a circular prerequisite relationship, when analysis is requested, then the system shows an error and does not display a learning sequence.

A recalculated priority may remain in the same category after a rating changes. The acceptance criteria require recalculation, not an automatic change of category.
