# Technology Brief: Fuzzy Logic and Expert Systems

## Why this technology

The assignment brief says DSS requires lecturer approval by the end of Week 4. This project therefore selects **Fuzzy Logic and Expert Systems**, which is a named technology category in the brief. The resulting system provides decision support, but DSS is not the selected technology.

## Core idea

Fuzzy logic lets the system work with uncertain human descriptions. A self-rating of 2 out of 5 can be partly low and partly medium. An expert system stores reviewed career knowledge and IF-THEN rules. The inference engine uses the user inputs and rules to give a priority and an explanation.

## Basic flow

```text
User career + skill ratings
        -> fuzzification
        -> knowledge base and IF-THEN rules
        -> fuzzy inference
        -> priority, learning order and explanation
```

## Example rule

IF current skill is low AND career importance is high, THEN learning priority is very high.

For a Software Developer profile, a user who rates Git as 2/5 where 4/5 is required may receive a very-high priority. The system can suggest Git concepts, GitHub, basic command-line skills and a learning order before API development.

## Methods and tools

1. Fuzzy sets and membership functions: turn values into low, medium and high labels.
2. Mamdani fuzzy inference: apply readable IF-THEN rules and form a priority output.
3. Rule-based knowledge base: store profiles, prerequisites and explanations separately from the user interface.
4. `scikit-fuzzy`: an optional Python implementation library.

## Risks

- Experts must review rules and skill profiles regularly.
- Self-ratings can be inaccurate.
- Skill data is personal information and must be protected.
- Rules must be checked for unfair treatment.

## Alternative

Machine learning could learn recommendation patterns from historical data, but it needs sufficient representative data and careful bias testing. A fuzzy expert system is more realistic for this small, explainable project.
