# Plan the APEX Buildout

## Introduction

In this lab, you will shape an APEX buildout that complements the workshop rather than distracting from it. The prompt engineering challenge is to make Codex reason at the right altitude: enough detail to design pages, flows, and data interactions, but not so much that it fabricates implementation facts you have not provided.

Estimated Time: 20 minutes

### Objectives

In this lab, you will:

* Define the role of APEX in the workshop experience
* Break the application into pages, flows, and data needs
* Prompt Codex to generate a credible build plan instead of an overconfident prototype description

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* A workshop scenario that would benefit from an APEX application
* A basic understanding of the business process or user journey you want APEX to support

## Task 1: Define the APEX use case

1. Decide what the APEX application is meant to do in the workshop:

    * Showcase data captured earlier in the lab
    * Provide a lightweight admin or dashboard interface
    * Act as the user-facing layer for a business scenario
    * Demonstrate rapid application delivery on Oracle data services

2. Write down the user persona and the expected user journey.

3. Create a scope-setting prompt:

    ```text
    <copy>
    Design an Oracle APEX buildout for this workshop. Start with user goals, core pages, data dependencies, and success criteria. Do not assume database objects, REST endpoints, or authentication flows that I have not explicitly provided.
    </copy>
    ```

## Task 2: Break the buildout into implementation units

1. Ask Codex to define:

    * Page inventory
    * Navigation flow
    * Required tables or views
    * Any sample data needs
    * Validation and security considerations

2. Review whether the output is appropriate for:

    * A design discussion
    * A build lab
    * A follow-on implementation sprint

3. Refine the prompt if Codex jumps too far ahead into unsupported technical detail.

## Task 3: Prepare the handoff from plan to lab

1. Ask Codex to convert the APEX plan into a workshop-ready sequence.

2. Require explicit placeholders for items that a lab owner still needs to supply, such as:

    * Workspace name
    * Schema
    * Application ID
    * SQL scripts
    * Credentials

3. Capture the final output as an input to a future hands-on APEX lab.

4. You may now [proceed to the next lab](#next).

## Learn More

* [Prompt engineering guide](https://developers.openai.com/api/docs/guides/prompt-engineering)
* [Introducing Codex](https://openai.com/index/introducing-codex/)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
