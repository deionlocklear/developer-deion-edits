# Deploy OCI Resources Through the Console and CLI

## Introduction

In this lab, you will define the OCI environment needed to support the workshop and use prompt engineering to help Codex produce a clean deployment plan. The main value here is careful prompting around scope, sequence, environment assumptions, and the difference between illustrative steps and tenancy-specific execution.

Estimated Time: 25 minutes

### Objectives

In this lab, you will:

* Identify the OCI resources needed for the workshop
* Separate console-based and CLI-based deployment tasks
* Use Codex to draft deployment steps without hiding environmental assumptions

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* A workshop scenario that requires OCI resources
* Basic knowledge of OCI resource dependencies and tenancy boundaries

## Task 1: Define the resource model

1. List the OCI resources your workshop requires. For example:

    * Compartment
    * VCN and subnet
    * Compute instance
    * Database service
    * Object Storage bucket
    * IAM policies

2. Mark each resource as one of the following:

    * Must exist before the workshop
    * Can be created during the workshop
    * Optional or stretch content

3. Ask Codex to create a dependency-aware plan:

    ```text
    <copy>
    Create an OCI deployment plan for this workshop. Separate prerequisites from in-lab steps, show resource dependencies in order, and call out which values must be supplied for a specific tenancy, compartment, region, or naming standard.
    </copy>
    ```

## Task 2: Split console and CLI paths

1. Decide which steps are best taught in the OCI Console and which are better taught in the CLI.

2. Require Codex to produce both tracks when appropriate:

    * Console walkthrough for first-time learners
    * CLI workflow for repeatability and automation

3. Use a prompt that enforces clarity:

    ```text
    <copy>
    For each deployment step, state whether it should be taught in the OCI Console, the OCI CLI, or both. If both are included, explain why each path is valuable to the learner.
    </copy>
    ```

## Task 3: Add validation and failure handling

1. Ask Codex to include validation checkpoints after major resource-creation steps.

2. Record the environment details that the prompt must carry forward in later labs.

3. Add an error-handling prompt:

    ```text
    <copy>
    Include common failure points, such as missing permissions, quota issues, incorrect compartment selection, or network prerequisites. Keep the troubleshooting guidance concise and specific to the affected step.
    </copy>
    ```

4. You may now [proceed to the next lab](#next).

## Learn More

* [Prompt engineering guide](https://developers.openai.com/api/docs/guides/prompt-engineering)
* [Using tools](https://developers.openai.com/api/docs/guides/tools)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
