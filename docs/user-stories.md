# User Stories

## US1 - View skill gaps (FR1, FR2, FR4)

As a student, I want to select a target career and rate my current skills, so that I can see which skills I need to improve.

Acceptance criteria:

1. Given that I select a supported career, when its profile opens, then I can see every required skill and its required level.
2. Given that I enter a rating from 0 to 5 for each required skill, when I request an analysis, then the system shows a gap for each skill.
3. Given that I enter a value outside 0 to 5, when I save it, then the system rejects the value and shows an error message.

## US2 - Understand a priority (FR5, FR6, FR8)

As an early-career job seeker, I want to know why a missing skill is important and what I should learn for it, so that I can choose useful learning activities.

Acceptance criteria:

1. Given that a gap is high or very high, when I open its details, then I can see its priority, knowledge topics, suggested tools or technologies and prerequisites.
2. Given that the system gives a priority, when I view the explanation, then it states the relevant rating, required level and importance rule.

## US3 - Update the learning order (FR2, FR7)

As a job seeker, I want an updated learning order after I improve a skill, so that I can focus on the next useful skill.

Acceptance criteria:

1. Given that I increase a saved skill rating, when I run the analysis again, then the system recalculates the related gap and priority.
2. Given that one skill is a prerequisite for another, when the learning sequence is displayed, then the prerequisite appears earlier in the sequence.
