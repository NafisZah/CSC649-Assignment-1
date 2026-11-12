# Requirements

# Requirements

These requirements describe the intended prototype. The numerical targets are proposed acceptance targets and have not yet been tested.

## Definitions

### Self-rating scale

| Rating | Meaning |
|---|---|
| 0 | I have no experience with this skill. |
| 1 | I recognise basic terms but cannot yet complete a practical task. |
| 2 | I can complete simple tasks with step-by-step guidance. |
| 3 | I can complete common tasks independently. |
| 4 | I can complete more complex tasks and solve common problems. |
| 5 | I can complete advanced tasks and explain my approach to others. |

The same level descriptions would be used when defining required levels.

### Skill gap

For each skill:

**Skill gap = maximum of 0 and (required level − self-rating).**

A gap of 0 means that the self-rating meets or exceeds the proposed required level. It does not prove that the user has demonstrated the skill.

### Career importance

Importance would be assigned in the career profile on a scale from 1 to 5:

- 1: relatively low importance within the selected profile.
- 3: moderate importance.
- 5: high importance.

Values 2 and 4 represent intermediate positions. Users would not change these values during an analysis.

## Functional requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall allow the user to select one of the three supported career profiles: Software Developer, Data Analyst or Software Tester. |
| FR2 | The system shall display the skill name, required level and importance value for every skill in the selected career profile. |
| FR3 | The system shall allow the user to enter and update a whole-number self-rating from 0 to 5 for each listed skill. |
| FR4 | The system shall prevent analysis until every listed skill has a valid self-rating. |
| FR5 | The system shall calculate each skill gap as the maximum of 0 and the required level minus the self-rating. |
| FR6 | The system shall assign each positive skill gap a priority score using Mamdani fuzzy inference with skill-gap size and career importance as inputs. |
| FR7 | The system shall assign each positive skill gap a priority score using Mamdani fuzzy inference with skill-gap size and career importance as inputs. |
| FR8 | The system shall display predefined learning topics and relevant tools for each skill with a positive gap. |
| FR9 | The system shall generate a learning sequence in which unmet prerequisites appear before the skills that depend on them. |
| FR10 | The system shall explain each learning priority by displaying the self-rating, required level, calculated gap, importance value and activated fuzzy rules. |
| FR11 | The system shall recalculate the results when the user changes a rating and requests a new analysis. |
| FR12 | The system shall provide a reset control that clears the current career selection, ratings and results. |

## Non-functional requirements

| ID | Type | Requirement |
|---|---|---|
| NFR1 | Performance | For a profile containing up to 15 skills, the system shall display complete results within 3 seconds of a valid analysis request in at least 95 of 100 trials on a documented test laptop with at least 8 GB RAM, a current desktop browser and no external API calls. |
| NFR2 | Usability | At least 4 of 5 computing students who are new to the prototype shall complete each of three tasks within 5 minutes without help: produce an initial analysis, locate an explanation for a priority, and update a rating to produce revised results. |
| NFR3 | Security/privacy | The system shall not write user ratings or analysis results to persistent storage or application logs, and shall not transmit them to external services. |
| NFR4 | Reliability | If a career profile contains a missing prerequisite reference or a circular prerequisite relationship, the system shall show an error and withhold its learning sequence in every deliberately malformed test case. |

## Business and validation rules

1. Only whole-number self-ratings from 0 to 5 are valid. Blank values, decimals, text and out-of-range numbers must be rejected.
2. A skill with a gap of 0 must be marked “Target level met based on self-rating” and excluded from the learning-task list.
3. Required levels must use the same 0–5 scale as self-ratings.
4. Importance values must be whole numbers from 1 to 5.
5. Every prerequisite must refer to another skill in the same career profile.
6. Career-profile prerequisites must not contain cycles.
7. Among skills whose prerequisites are already satisfied, the skill with the highest priority score appears first. Equal scores are ordered alphabetically by skill name.
8. A prerequisite whose self-rating meets its required level is treated as satisfied.
9. User input and results are retained only for the current page session. Resetting or reloading the page clears them.
10. Proposed priority-score intervals are: low below 30; medium from 30 to below 65; high from 65 to below 85; and very high from 85 to 100.

The rating scale is ordinal. Treating the distance between adjacent levels as equal is a simplifying assumption that would need evaluation before practical use.
