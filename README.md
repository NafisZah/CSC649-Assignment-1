# Personalised Skill-Gap and Learning-Path Support

> CSC649 Assignment 1 proposal: a fuzzy expert-system improvement for career skill-gap support in the MYFutureJobs context.

An independent prototype proposal that uses a fuzzy expert system to help students identify skill gaps and decide what to learn first for a selected computing career.

## Status

This project is at the proposal and requirements stage for CSC649 Assignment 1. The system has not yet been implemented or evaluated.

## Problem

Students and fresh graduates may know which career they want but still struggle to decide which skills to improve first. A list of occupational skills does not necessarily explain the size of each skill gap, its importance, or the order in which related topics should be learned.

This project proposes a small prototype that compares self-rated skills with a predefined career profile. It would explain learning priorities and suggest an order that respects prerequisite skills.

## Specialised technology

The selected technology is Fuzzy Logic and Expert Systems.

A fuzzy inference system would combine skill-gap size and career importance to assign learning priorities. A separate prerequisite-ordering process would arrange learning items so that required foundations appear before dependent skills.
## Documents

- [Problem statement and scope](docs/problem-statement.md)
- [Requirements](docs/requirements.md)
- [User stories](docs/user-stories.md)
- [Technology brief](docs/technology-brief.md)
- [Research sources](docs/research-sources.md)
- [Sprint Log](docs/sprint-log.md)


## Proposed users and scope

The main users are computing students and fresh graduates preparing for entry-level employment.

The proposed prototype covers three career profiles:

- Software Developer
- Data Analyst
- Software Tester

Each profile would contain a small, predefined set of skills, required levels, importance values and prerequisite relationships.

The prototype is independent of MYFutureJobs and PERKESO. MYFutureJobs is discussed as an existing career-support platform, but this project does not assume access to its accounts, internal data or services.

## Project structure

| Path | Purpose |
|---|---|
| `README.md` | Project overview, status and document links |
| `.gitignore` | Files and folders excluded from version control |
| `docs/problem-statement.md` | Problem, users, stakeholders and scope |
| `docs/requirements.md` | Functional and non-functional requirements |
| `docs/user-stories.md` | User stories and acceptance criteria |
| `docs/technology-brief.md` | Technology concepts, example and justification |
| `docs/research-sources.md` | References used in the proposal |
| `docs/sprint-log.md` | Actual sprint planning, progress and reflection |

## Roadmap

1. Verify the supporting sources and refine the problem statement.
2. Finalise the requirements and acceptance criteria.
3. Explain the fuzzy inference process using a worked example.
4. Complete the repository structure and record genuine GitHub activity.
5. Prepare the assignment report and GenAI declaration.
6. If developed beyond this assignment, implement and evaluate the prototype.

## Author

MUHAMMAD NAFIS ZAHIN BIN SHAHRUL AZAM
2025478438
CSC649 - Special Topics in Computer Science  
GitHub: https://github.com/NafisZah

## Note on GenAI

GenAI was used only within the assignment rules. All facts and sources must be checked, and all final writing must be understood and revised by the student.
