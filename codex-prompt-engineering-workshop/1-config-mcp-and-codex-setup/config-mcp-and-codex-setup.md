# Configure Codex, MCP, and Local Access

## Introduction

In this lab, you will establish the working foundation for the rest of the workshop. The goal is to make Codex usable as a repeatable engineering partner by defining configuration expectations, downloading or connecting the appropriate Codex surface, and enabling MCP-backed tools that improve context quality and task execution.

Estimated Time: 20 minutes

### Objectives

In this lab, you will:

* Identify the Codex surface you plan to use for workshop work
* Define the minimum local configuration required for reliable prompting
* Understand when MCP is useful and what kinds of tools it should expose

### Prerequisites

This lab assumes you have:

* Completed the previous labs in this workshop
* Access to the environment where you plan to run Codex
* Access to any repository, files, or source systems needed for workshop work

## Task 1: Choose the Codex operating model

1. Decide which Codex experience is best for your workflow:

    * Desktop app for day-to-day workshop building
    * CLI for local repository workflows
    * Web or shared workspace environment for lightweight collaboration

2. Record why that choice fits your team. Focus on repository access, review needs, and whether the work is primarily content-oriented, code-oriented, or both.

3. Write a setup prompt you can reuse:

    ```text
    <copy>
    Help me configure Codex for Oracle workshop development. Assume I need stable output structure, clear file organization, and prompts optimized for documentation, presentations, and lab authoring.
    </copy>
    ```

    > **NOTE:** In a production LiveLab, this step would usually be paired with environment-specific screenshots or a sample configuration file.

## Task 2: Define your baseline configuration

1. Review the areas you want Codex configuration to control:

    * Permissions and approval behavior
    * Preferred tools
    * Output formatting expectations
    * Testing and verification expectations
    * Team conventions for filenames, folders, and artifact reviews

2. Write down the rules that matter most in your environment.

3. Create a short prompt that turns those expectations into instructions:

    ```text
    <copy>
    Work in a workshop-authoring mode. Prefer structured markdown, preserve Oracle branding constraints, explain assumptions briefly, and leave artifacts in a LiveLabs-friendly folder structure.
    </copy>
    ```

## Task 3: Plan MCP usage

1. List the categories of tools you want available through MCP or equivalent integrations:

    * Documentation lookup
    * File or repository access
    * Presentation or document generation
    * Browser interaction
    * OCI or internal system actions

2. For each category, note the risk of giving the tool too much scope. This is where prompt engineering and tool boundaries meet.

3. Write one prompt that deliberately constrains tool use:

    ```text
    <copy>
    Use MCP-backed tools only when they materially improve accuracy or speed. Prefer primary documentation sources, summarize findings before acting, and avoid broad changes when a targeted edit is enough.
    </copy>
    ```

4. Review the prompt and confirm it reflects the environment you chose in Task 1.

5. You may now [proceed to the next lab](#next).

## Learn More

* [Config basics for Codex](https://developers.openai.com/codex/config-basic)
* [Model Context Protocol in Codex](https://developers.openai.com/codex/mcp)
* [Import to Codex](https://developers.openai.com/codex/import)
* [Introducing Codex](https://openai.com/index/introducing-codex/)

## Acknowledgements

* **Author** - OpenAI Codex
* **Last Updated By/Date** - OpenAI Codex, July 2026
