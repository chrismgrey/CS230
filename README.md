This repository contains the completed software design document for The Gaming Room project along with this reflection describing the design decisions and development process.

The Gaming Room was the client for this project. They wanted a web-based version of their current Android game Draw It or Lose It that could support multiple teams and players in a shared environment. A core requirement was that all names for games, teams, and players had to be unique so that duplicates could not be created. The design also needed to make sure that only one instance of the game service existed in memory while still allowing multiple users to interact with the system at the same time.

One part of the documentation that went well was explaining why certain design choices were made and how they satisfied the client’s needs. The use of the singleton pattern was tied to the requirement for a single active game service, and the use of the iterator pattern was tied to the need to prevent duplicate names. The document clearly linked each solution back to a requirement rather than listing features without context.

Creating the design document before writing the code made the development process easier. Since the structure and constraints were already defined, the coding stage was more direct. The base Entity class, the GameService logic, and the handling of teams and players were already planned, which reduced confusion and rework later.

If any section were to be revised, the architecture portion could be expanded to include details about how this system might be deployed in a distributed environment such as AWS or Azure. That would help anyone who needs to move the design into a production setting.

The design was built around the user’s needs by enforcing unique entities and a single service instance to protect the integrity of the game. Designing with user needs in mind helps avoid rebuilding features later and makes sure the software matches how the business expects it to function.

The overall approach was to start with the requirements, map them to object-oriented principles, and then apply design patterns that fit the problem. In future projects the same approach would be used by planning the structure first and then implementing once the design is clear.

The design document has been added to this repository as part of the CS230 portfolio submission.
