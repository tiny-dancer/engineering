# Engineering Expectations & Responsibilities

These have been created as a consistent reference for both myself and teams over the previous years as an engineering leader. Like all great software, this document is continuously evolving based on feeback and experience.

Table of contents
=================

<!--ts-->
   * [Individuals](#individuals)
   * [Teams](#teams)
<!--te-->

Individuals
============

> Primary goal is delivering value to the users and thus the business.

### Mid Level Engineer

- Capable of delivering features/capabilities self sufficiently in a timely manner most of the time.
- Ready to take ownership and delve into new technology areas with a quick ramp up.
- Not expected to lead innovation efforts, but is actively particiapting
- Well versed in at least single area of development stack (ui, api, database, etc) and aware of majority of components in play
- Team player

### Sr Engineer (A codebase leader)

- Capable of delivering features/capabilities self sufficiently in a timely manner.
- Nurtures and leads the code base vs fighting it
  - Developing maintainable, tested, clean code
  - A design pattern is clearly present and code is not “brute forced” in
- Being inclusive of team members
- Ability to ramp up quickly around new technology areas, take ownership and deliver
- Well versed in several areas of development stack (ui, api, database, etc) and aware of majority of components in play

### Lead Engineer (Scrum team engineering leader)

- Extends Sr Engineer to include more leadership at a scrum team level vs a code level
  - A key technical representative and decision maker in product prioritization, planning conversations
  - A technical leader for the team in architectural direction and conversations
  - A leader in technical design and implementation for sprint work
  - Providing support and mentorship for engineering team members
   - Enabling team members to step out of their comfort zone and efficiently learn new areas
- Understanding and ideally fluent in end to end delivery of a software product (database, backend, frontend, ci, cd, the edge, automation, etc)
- Well versed in all areas of development stack (ui, api, database, etc) and aware of all components in play
- Identify opportunities to optimize and solidify current delivery process which could mean introducing new quality check processes, introducing new tool/technology etc

> Any Engineer absolutely can participate in these same conversations, the difference is the lead engineer is viewed as a key decision maker in these matters.

### Engineering Manager (A product(s) engineering leader)

- Extends lead engineer responsibilities across one or more teams
- Responsible for product quality and delivery
- Removes blockers deriving from external teams
- Sets and leads the high level goals of architectural direction
    - In collaboration with appropriate parties, ie. organization goals, architects, directors, peers, scrum teams, etc
- Works closely with product and business on direction and prioritization of product
- Defines and ensures high quality team tooling, engineering practices and processes

> Any Engineer absolutely can participate and provide feedback in these same conversations, the difference is the lead engineers are viewed as key decision makers and engineering manager is viewed as the decision maker in these matters. A lead engineer should be able to strongly represent their respective scrum team. An engineering manager may likely defer to a lead engineer.

Teams
============

Breaking down "over the wall" mentality

- As best as possible within the organization, all relevant team members need to be engaged as part of a single team team, this includes:
  - Security
  - Development
  - Quality
  - UX & UI
  - Operations
  - Support
  - Product
- Examples
  - Quality + Development
   - If at any time quality or development is the "hold up", one or the other disciplines should be able to step in and help
    - For example, If manual quality testing is the hold up for delivery of work. Development engineers *should* step in and execute the test cases for work needing testing. In this scenario, the acceptance of this work would require a final sign off by both the product and quality team members. This assures the quality team member still validates the story but is helped executing the test cases by other team members (development engineers)
    - Vice versa, if all the current work is in the hands of development and quality has no current work in progress, Quality Engineers *should* pair up with developers and either help with automated test cases or even write production code for the implementation.
  - UX/UI + Development + Quality + Product
   - development, quality, and product should be involved with ux/ui from the very beginning. 
    - Flushing out potential complexity hot spots prior to code development
    - A legitimate understanding of the UI, business transactions and flows prior to code development
    - Enable all team members to provide feedback and innovative thought at a time where changes in design are more welcoming
     - Feedback and innovative thought during development can cause a disruption in work or is pushed back as a later enhancement
      - Both outcomes highlight a lost opportunity and impact our ability to deliver value to our fullest
      - "Feedback and innovative thought during development" is always welcomed as later enhancements, the goal by including everyone in discussions from the beginning is we are able to capitalize on as much of these eventual enhancements and/or tweaks sooner in the product's life without timelines/delivery.
    - Designs are backed by product research, user feedback, and solidified with prototype usability studies *prior to code development*
     - Achieve this as best as possible within organization limitations and financial considerations
    - If multiple sites and teams are involved, ensure focus on a [design system](https://www.designbetter.co/design-systems-handbook?utm_campaign=designbetterco&utm_source=hs_email&utm_medium=email&utm_content=58836955&_hsenc=p2ANqtz-8CYOSWTDN6OI-fx7vDrUEK3Dolnyrfadi9rUPB0MKkXio289MW86jVj5Vr1ltF1QoaooQ9-2sNXWaQ8AoKRyslEVIeQQ&_hsmi=58836955) across the product experience for long term consistency, agility and maintenance
     - [pattern library](https://boagworld.com/design/pattern-library/) (reusable components) 
      - These reusable components are ideally used in both coding (by development) and in designing (by ux/ui)
       - [Example with react and sketch](https://github.com/airbnb/react-sketchapp) of using developer made react components within sketch for the design team
  - Development + Operations
   - Operations is involved from initial planning and lower environment implementations will match production environment to quickly solidify operational work
  - quality + ux/ui
  - product + quality
  - product + ux/ui
  - etc.

It's very feasible team members are at first not comfortable acting cross-functional when adopting this mind set. The team should be operating in welcoming environment to allow each other to comfortably learn new technologies and functions.

Limiting Work in Progress and Delivering Features Sequently

Work in Progress is the death to any lean pursuing software development team. At the core of many modern agile, devops, and lean practices is downsizing and controlling Work in Progress.

Reducing lead cycle time allows for faster user feedback

- After releasing initial features or "MVPs", subsequent features should be shifted or reprioritized based on user feedback.
  - Very likely originally planned subsequent features could look different after initial releases
  - If working on items in parallel, alot of the work on these originally planned features may be "lost" work as the feedback doesn't come until they've already been developed and released.

Ensuring delivery of a higher priority items

- Preferable when nearing the end of a planning period to have already delivered all priority items vs about to release all priority items
- Less risk when delivered incrementally and seperate

**Releasing more often**

If after an item (US or DE) is signed off on in non-prod and we're concerned about "releasing for the sake releasing", why did we spend time working on this item to begin with? If after an item is completed and there isn't a benefit for it to be pushed to production, it should not be started.

Proven releasing more often reduces the risk of releases. 

1. "The more you do it, the better you are at it"
2. Less change per release
3. Even if a potential release could be considered "too small", at that point think of the benefits to the *next* release, not the current release.

Helps focus on the immediate benefits. Proven "work to be done" is completed faster if done sequentially vs all at once

1. Enables incremential improvement, failing fast, true MVP's and product innovation
2. Lowers Risk, "work in progress" is the death of software development
   1. If work is not completed as planned:
     1. When done sequentially with less in parallel, increases probabiliy of completing first up, high priority items.
     2. When done in parallel, there is a risk all items would be not be completed

*These are benefits of a more efficient team, releasing more often is not a goal itself but a byproduct of better processes

All team members contribute to solutions

Story planning and grooming is a team-wide activity

Solutions & implementations should be a team decision

- Enable any team member to own solution
  - Guidance and governance as needed to ensure quality implementations
   - Positive feedback given for solutions in need of changes

Product members are responsible for accurately portraying user/customer wants & associated requirements

- As a team requirements & solution is solidified to be worked on

Agile Conventions & Tool Usage

A Production deployment is necessary to consider a work item complete

- Whether or not a work item's production deployment has been completed should be visibile in daily kanban or sprint status views

Picking up new work items to begin development on needs to take into account more than just the individual team member's capacity

- Ie. a team member who begins development on a new story that should take 3 days to complete when quality engineering would not be able to test it for at least a week. 
  - In this situtation it seems reasonable there is already too much existing WIP, the open capacity team member could pair with quality engineering to help reduce the back up.
   - This could include test automation work or even manual test case test execution

**Rally Usage**

Kanban View is used to accurately track production deployments (Kanban View vs Iteration Status)

- Adding Prod Deploy column
  - Accepted stories have little to no value until they are deployed to production
   - False sense of completion
- Limit # of In-Progress Items to # of Team Members (starting point, can shift)
  - Work on items to completion sequentialy as best as possible (see above note)

Build Version field is populated with correct pipeline url + version

User Stories include "As a <role>, I want <feature> so that <reason>" in description

- **Reason statement is most important** but often left off
- Clearly communicates *why* a feature is being implemented and it's intended benefit
  - This reason is a major benefit in proper scoping & solutioning

No stories above an 8 are to be worked on, break them down to smaller stories

- Number of test cases & requirements are also indicators of a story too large
  - In general, a US with more than 4 requirements is likely an indicator of a story too large
   - This is for requirements, not acceptance criteria
- Ideally broken down via **incremential production releases**, each story can still be deployed to production with user benefit
- Deploy a solution to the requirements, but scoped down 

Team member capacity should be calculated for each individual.

**Swarming**

At a basic level, when a WIP item has remained open past their expected delivery, the team pairs together and hyper focuses on delivering this specific item. 

Eliminating the continued extension of the WIP

Knowledge sharing and increased learning amonst the team

For the owner of the specific WIP item, **this is viewed as an opportunity to learn and move forward.**

- Over time, everyone on the team runs into this situation for a variety of reasons. Its about having a built in mechanism to move forward work items and team member's knowledge (both the swarmers and swarmee)

References

<http://tobeagile.com/2012/12/11/seven-strategies-for-team-swarming/>

<https://www.agilealliance.org/resources/experience-reports/swarm-beyond-pair-beyond-scrum/>

<https://www.mountaingoatsoftware.com/blog/should-a-team-swarm-on-to-one-backlog-item-at-a-time>

<https://blog.3back.com/scrum-patterns/6-ways-successfully-swarm/>

Continuous Integration & Continous Delivery

**Test Automation**

Test automation is the backbone of all efficiency improvements within product development team. Test automation is the protection layer that enables teams to move faster while safe guarding oneself from quality issues.

Stories and defects have test automation put in place **prior to code development.**

- The tests first fail, then code development will change the tests to passing
- Eliminates extraneuous manual testing during local code development

**Git as Source Control**

**Pull Requests**

All changes much flow through a proper pull request acceptance, this includes at a minimum:

Successful build & unit test execution

Successfully deploying the change to an environment

Successfully executing test cases on the deployed environment

- HTTP tests for an API
- Browser based tests for a UI

**Quality Engineers can do manual testing directly in this environment**

- This enables quality sign-off to occur very early in the development cycle
  - Developer is still actively engaged in the coding at this point allowing for quick iterations on defects found 

**Branch Strategy**

Ideally using a Single Trunk Pull Request branching strategy

Any change (hot fix, feature or defect) is delivered to production in the same way

- Feature toggles are utilized to safely control WIP across environments

**My Simple Beef with the Git Flow branching strategy**

Treats WIP differently when it doesn't need to be.

Work in Progress (hot fixes, defects and features) should be treated equaly and delivered the same way. Anything otherwise unnecessarily introduces additional complexity in branch management, release pipelines, and environment testing.

Team comes first, always

Good results are a by-product of a good team. Primary focus is on entrusting, enabling and growing the team, *not* focusing on the results themselves.

Positive environment. In almost all negative situations, the event is the result of the environment and it's surrounding processes, not the fault of an individual person. Understand and resolve the environmental process issues and communicate in all directions the cause is as such. Individuals involved in negative events should be empowered and not punished, given the opportunity to properly solve the identified process issue.

 

Agile Schedule "Starter"

Daily

Daily Morning Meeting (Scheduled 30 minutes)

- Stand Up call
  - No more than 15 minutes
  - Each person speaks:
   - What they did yesterday
   - What their doing today
   - Any blockers
- Demo's or Working Session
  - Can fulfill the remaining scheduled 30 minutes
  - Demo user stories or defects in need of acceptance
  - Alotted time for quickly pairing with team members for any items that came up during stand up call

Weekly

2 Sprint Groomings / Story Tellings (Led by Product Owner)

- This is focused on *collectively* grooming upcoming work
  - Solidifying story requirements, acceptance criteria, and design work.

Bi-Weekly

Retro

Higher level demo's
