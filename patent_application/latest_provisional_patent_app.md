# Provisional Patent Application

## Title of Invention
**AI-Powered Course Knowledge Base Generation and Adaptive Learning Framework**

## Field of the Invention
This invention relates to educational technology systems, particularly to methods and systems for (1) generating a unified course knowledge base via artificial intelligence, and (2) delivering adaptive, goal-directed learning using prerequisite-driven navigation.

## Background of the Invention
Traditional learning management systems and online course creation platforms face significant limitations:
- Manual content creation is slow and costly.
- Learning pathways are rigid and do not adapt to individual mastery levels.
- Prerequisite enforcement is minimal or non-existent.
- Adding new subjects requires substantial manual effort.

These limitations reduce scalability, personalization, and the ability to deliver comprehensive coverage in diverse domains.

## Summary of the Invention
The invention comprises two independent but complementary innovations:

1. **Unified KB Generation via AI:** A standardized data structure for representing course content, populated by querying an AI agent to generate topics, prerequisites, study content, examples, and assessments.
2. **Adaptive, Goal-Directed Learning Framework:** A course delivery engine that navigates content using transitive prerequisite relationships, enabling multiple learning paths and goal-driven progression.

## Detailed Description of the Invention

### Invention 1 — KB Schema Generation

#### Unified Data Structure
The KB is represented as a JSON schema containing:
```json
{
  "subject": {
    "id": "string",
    "name": "string",
    "description": "string"
  },
  "topics": [
    {
      "id": "string",
      "name": "string",
      "description": "string",
      "prerequisites": ["topic_id_array"],
      "studyContent": "markdown_formatted_content",
      "examples": ["example_array"],
      "quizQuestions": [
        {
          "question": "string",
          "options": ["option_array"],
          "correctAnswer": "string",
          "explanation": "string"
        }
      ]
    }
  ]
}
```

#### Population Method
1. **Input Subject:** User inputs subject description for which course is to be generated.
1. **Topic Discovery:** AI agent is provided a geniric description specifying how to identify a set of subject related topics. The agent then returns a set of topics.
1. **Generate Subject Skeleton Data Structure:** The agent uses the set of returned topics to populate the skeleton of the data structure that will be fully populated in subsequent phases. In this stage, the AI agent will idenfity and populate a set of prerequisite topics for each topic.
1. **Content Creation:** AI generates study materials, examples, and assessment questions.
1. **Validation:** Automated checks ensure completeness, logical consistency, and compliance with schema.
1. **Deployment:** The fully populated course content is available to be loaded into a production system via an automated process.

#### Embodiments
- KB may be stored as a JSON file, and is adaptable to other formats, e.g. XML, YAML, etc.
- AI may be any LLM.
- KB may be used in educational, corporate training, certification, or research contexts.

---

### Invention 2 — Adaptive Learning Framework

#### Core Logic
- Receives generated KB containing topics names, topic prerequisite names, study material, examples and quiz questions.
- Presents students with multiple dynamically generated learning paths updated continually as the student gains subject matter competency. 
- Each learning path begins with a topic that the student is **ready** to study. The student is deemed ready to study the topic is he has succesfully learned all prerequisite topics.
- Optionally allows students to create any number of subject matter learning goals. A learning goal consists of a topic the the student is not ready to learn. The learning goal is pursued by first learning all of the goals prerequisite topics.
- The user can then filter the learning paths to only include those topics that contribute to a selected learning goal.
- Determines mastery for each topic based on assessments.
- Computes subject learning paths using **transitive prerequisite relationships**.

#### Algorithms
**Readiness Calculation:**
```
readiness(T) = all(mastery(P) >= "understood" for P in prerequisites(T))
```
**Goal-Directed Pathfinding:**
```
optimal_path(goal_topic) = shortest_path(current_mastery_state, goal_topic)
```
**Multi-Path Generation:**
```
paths(goal_topic) = all_paths_satisfying_prerequisites(goal_topic)
```

#### Features
- Multiple learning pathways, each represented by a topic that the sutudent is ready to pursue.
- Ability to filter learning pathways to just those relevant to a particular learning goal.

#### Embodiments
- Implemented as a web app, mobile app, or desktop application.
- Integrated with any LMS via API.
- Usable for skill training, language learning, or academic subjects.

---

## Claims

### Claim Set 1 — KB Schema & Generation
1. A computer-implemented method for generating a standardized course knowledge base, comprising:
    - defining multiple generic AI agent prompts that given a subject description, enable an AI agent to provide subject matter content encoded in a unified
    - defining a unified data structure containing topics, prerequisites, examples, and assessments;
    - querying an AI agent to populate each component of the data structure;
    - validating the populated structure for logical consistency and completeness.
2. The method of claim 1, wherein the unified data structure is in JSON format.
3. A computer-readable medium storing a course knowledge base generated according to claim 1.

### Claim Set 2 — Adaptive Learning Framework
4. A computer-implemented method for delivering adaptive online learning, comprising:
    - receiving a course knowledge base containing topics and prerequisites;
    - determining user mastery for each topic;
    - computing topic readiness using transitive prerequisite relationships;
    - recommending next topics based on readiness and user goals.
5. The method of claim 4, wherein multiple learning paths are generated for the same goal.
6. A computer system configured to implement the method of claim 4, operable with any conforming course knowledge base.

---

## Technical Advantages
- Separates KB generation from the adaptive learning framework, allowing independent use and licensing.
- Reduces content creation time from months to hours.
- Adapts learning pathways to user mastery and goals.
- Scales to any subject matter without architectural changes.

## Industrial Applicability
Applicable to academic institutions, corporate training, certification programs, and self-directed learning platforms.
