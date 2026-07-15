# Create a Presentation from Blogs, Docs, and the Oracle Style Guide

## Introduction

In this lab, you will use prompt engineering to turn raw source material into a presentation draft. The key skill is not simply asking for slides, but giving Codex the right boundaries: source priority, audience, structure, tone, branding expectations, and output format.

Estimated Time: 30 minutes

### Objectives

In this lab, you will:

* Gather the right source material for a workshop topic
* Instruct Codex to prioritize Oracle-owned sources and brand guidance
* Generate a presentation outline and first draft with review checkpoints

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* Access to the source material you intend to use
* A defined workshop topic or use case

## Task 1: Assemble grounded source material

1. Collect the sources you want Codex to use:

    * Oracle blogs
    * Oracle documentation
    * Oracle Style Guide assets and rules
    * Existing internal notes, if approved for use

2. Rank those sources in order of authority.

3. Write a grounding prompt:

    ```text
    <copy>
    Build the presentation using Oracle documentation as the primary source of truth, Oracle blogs as supporting context, and the Oracle Style Guide for visual direction. Flag any claim that is not clearly supported by the provided material.
    </copy>
    ```

    > **TIP:** If you expect Codex to make product or feature claims, require it to flag anything that is not supported directly by the sources you provided.

## Task 2: Generate the presentation plan

1. Define the target audience:

    * Sellers
    * Solution engineers
    * Developers
    * Customers

2. Define the presentation outcome:

    * Executive overview
    * Technical enablement session
    * Workshop lead-in
    * Internal training deck

3. Ask Codex for a presentation spec before asking for slides:

    ```text
    <copy>
    Create a slide-by-slide presentation specification for an Oracle-branded workshop intro deck. Include slide purpose, key message, recommended evidence, speaker-note intent, and any visual dependencies before generating the final deck.
    </copy>
    ```

## Task 3: Generate the first presentation draft

1. Ask Codex to create the deck only after the outline is accepted.

2. Require the output to include:

    * Slide titles
    * Core talking points
    * Speaker notes
    * Asset recommendations
    * Any unresolved gaps or assumptions

3. Use a refinement prompt:

    ```text
    <copy>
    Revise the presentation so it reads like an Oracle technical enablement asset rather than a generic AI-generated deck. Tighten the narrative, reduce repetition, preserve factual grounding, and keep each slide anchored to a single teaching goal.
    </copy>
    ```

4. Review the draft and note any slides that would need screenshots, diagrams, or additional product evidence before production use.

5. You may now [proceed to the next lab](#next).

## Learn More

* [Prompt engineering guide](https://developers.openai.com/api/docs/guides/prompt-engineering)
* [Introducing Codex](https://openai.com/index/introducing-codex/)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
