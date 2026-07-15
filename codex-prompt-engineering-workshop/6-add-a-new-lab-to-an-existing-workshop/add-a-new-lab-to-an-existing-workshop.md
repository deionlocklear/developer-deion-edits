# Add a New Lab to an Existing Workshop

## Introduction

In this lab, you will use Codex to extend an existing workshop with a new lab while preserving structural consistency. The prompt engineering focus is on teaching Codex to infer local conventions from the existing workshop, reuse those conventions, and avoid drifting into a new style or information architecture.

Estimated Time: 20 minutes

### Objectives

In this lab, you will:

* Analyze an existing workshop structure before adding new content
* Prompt Codex to preserve naming, sequencing, and markdown conventions
* Produce a first-pass new lab that fits naturally into the existing workshop

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* Access to an existing workshop that will be extended
* Permission to inspect and modify that workshop's source files

## Task 1: Inspect the existing workshop

1. Review the target workshop and note:

    * Folder naming patterns
    * Manifest structure
    * Lab title format
    * Common section headings
    * Tone and depth

2. Ask Codex to summarize the detected conventions before writing:

    ```text
    <copy>
    Inspect the existing workshop and summarize its authoring conventions before drafting the new lab. Preserve folder structure, markdown headings, lab style, and manifest patterns unless I explicitly ask for a change.
    </copy>
    ```

3. Confirm where the new lab fits in the flow and what it should teach.

## Task 2: Draft the new lab and manifest changes

1. Ask Codex to create:

    * The new lab markdown file
    * Any supporting folders that are needed
    * The manifest entry update

2. Require the draft to explain its assumptions briefly.

3. Use a precision prompt:

    ```text
    <copy>
    Add the new lab with minimal disruption to the existing workshop. Reuse the established structure, keep descriptions concise, and update navigation artifacts only where necessary.
    </copy>
    ```

## Task 3: Review the change as a workshop maintainer

1. Evaluate whether the new lab:

    * Belongs in the current workshop
    * Arrives at the right point in the learning journey
    * Matches the style of neighboring labs
    * Creates any new prerequisites or dependencies

2. Ask Codex for one final pass that tightens the draft for maintainability.

3. Record the reusable prompting pattern you would apply the next time you extend a workshop.

4. You may now [proceed to the next lab](#next).

## Learn More

* [AGENTS.md guidance for Codex](https://developers.openai.com/codex/guides/agents-md)
* [Config basics for Codex](https://developers.openai.com/codex/config-basic)
* [Model Context Protocol in Codex](https://developers.openai.com/codex/mcp)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
