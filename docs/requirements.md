# Requirements

## Functional requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall allow a user to select one target career from the supported career profiles. |
| FR2 | The system shall allow a user to enter or update a self-rating from 0 to 5 for every skill in the selected career profile. |
| FR3 | The system shall display the required level, importance and prerequisite skills for every skill in the selected career profile. |
| FR4 | The system shall calculate and display the gap between the user’s self-rating and the required level for every required skill. |
| FR5 | The system shall assign each skill gap a priority of low, medium, high or very high by using the expert rules. |
| FR6 | The system shall display related knowledge topics, tools or technologies and prerequisite skills for every skill gap. |
| FR7 | The system shall produce a learning sequence that places prerequisite skills before dependent skills. |
| FR8 | The system shall show a short explanation of the inputs and expert rules that caused each priority recommendation. |

## Non-functional requirements

| ID | Type | Requirement |
|---|---|---|
| NFR1 | Performance | The system shall show a result within 3 seconds for at least 95 of 100 test requests for a profile with up to 30 skills. |
| NFR2 | Usability | At least 4 of 5 representative student users shall complete the three main tasks within 5 minutes each without help. |
| NFR3 | Security/privacy | The system shall require authentication before showing or changing a saved profile; 100% of attempts to read another test user’s profile shall be denied. |
| NFR4 | Reliability | The system shall accept only whole-number self-ratings from 0 to 5; invalid values shall not be saved. |
