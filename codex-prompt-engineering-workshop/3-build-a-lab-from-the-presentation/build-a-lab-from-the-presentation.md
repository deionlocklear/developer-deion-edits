# Build a Lab from the Presentation

## Introduction

In this lab, you will convert presentation material into a hands-on lab draft. This is where prompt engineering shifts from narrative generation to instructional design. The goal is to guide Codex toward producing step-based content that is teachable, scoped, and realistic for a workshop participant.

Estimated Time: 25 minutes

### Objectives

In this lab, you will:

* Convert slide material into task-oriented lab content
* Separate conceptual explanation from executable learner actions
* Produce a first-pass lab structure that fits a LiveLabs-style format

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* A presentation outline or deck draft to convert
* A target audience for the resulting lab

## Task 1: Extract the actionable content

1. Review the presentation from Lab 2 and identify which slides contain:

    * Concepts only
    * Demonstration steps
    * Hands-on opportunities
    * Follow-up or optional content

2. Group the material into likely lab tasks.

3. Write a transformation prompt:

    ```text
    <copy>
    Convert this presentation into a LiveLabs-style markdown lab. Keep conceptual framing short, favor task-oriented steps, and identify where screenshots, prerequisites, or validation checks would be required in a production version.
    </copy>
    ```

## Task 2: Build the instructional structure

1. Require the lab draft to include:

    * Introduction
    * Estimated time
    * Objectives
    * Task sections
    * Learn More
    * Acknowledgements

2. Ask Codex to flag weak areas instead of guessing:

    ```text
    <copy>
    If the presentation does not provide enough detail for an accurate step, do not invent it. Mark the gap, describe the missing input, and continue building the rest of the lab.
    </copy>
    ```

3. Review whether the lab feels like a learner journey rather than a transcript of slide content.

## Task 3: Improve prompt reliability for lab authoring

1. Refine the prompt so Codex produces the same structure repeatedly across future labs.

2. Include output expectations such as:

    * Stable section headers
    * Numbered steps
    * Oracle-oriented tone
    * Explicit assumptions
    * Placeholder markers for screenshots or files

3. Save a reusable prompt template for future workshop conversions.

4. You may now [proceed to the next lab](#next).

## Learn More

* [Prompt engineering guide](https://developers.openai.com/api/docs/guides/prompt-engineering)
* [AGENTS.md guidance for Codex](https://developers.openai.com/codex/guides/agents-md)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
