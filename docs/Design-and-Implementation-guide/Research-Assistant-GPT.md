# Research Assistant GPT

## Table of Contents

* [Preface](#preface)
* [Introduction](#introduction)
* [Build a Research Assistant GPT](#build-a-research-assistant-gpt)
  * [1. Define the Research Architecture](#1-define-the-research-architecture)
    * [Establish the Scope and Requirements](#establish-the-scope-and-requirements)
    * [Establish a Source Hierarchy](#establish-a-source-hierarchy)
    * [Map Sources to Technical Requirements](#map-sources-to-technical-requirements)
  * [2. Research and Verify Information](#2-research-and-verify-information)
    * [Conduct Research and Extract Evidence](#conduct-research-and-extract-evidence)
    * [Evaluate Research and Evidence](#evaluate-research-and-evidence)
    * [Define Conflict-Resolution Rules](#define-conflict-resolution-rules)
    * [Define Information Gaps and Verification Records](#define-information-gaps-and-verification-records)
  * [3. Standardize the Research Output](#3-standardize-the-research-output)
  * [4. Build, Test, and Improve the GPT](#4-build-test-and-improve-the-gpt)
    * [Define the System Instructions](#define-the-system-instructions)
    * [Create the GPT Prompt](#create-the-gpt-prompt)
    * [Configure the Custom GPT](#configure-the-custom-gpt)
    * [Test the GPT](#test-the-gpt)
* [Conclusion](#conclusion)

---

## Preface

Technical writers spend significant time researching, verifying, and organizing product information before creating documentation. This project addresses that challenge by using a **Research Assistant GPT** to standardize and automate repetitive research tasks.

This guide explains the research methodology, GPT configuration, output structure, and testing process.

## Introduction

Technical writing involves creating, revising, and maintaining documentation for technical products, systems, and processes. The documentation development process consists of multiple phases, including research.

Research requires technical writers to locate relevant information, evaluate sources, verify technical details, and identify information gaps before creating documentation.

A Research Assistant GPT can support this process by automating repetitive research and analysis tasks. The GPT collects relevant information, evaluates evidence, identifies conflicts and information gaps, and organizes findings into a structured research report.

## Build a Research Assistant GPT

The Research Assistant GPT is a custom GPT designed to support technical writers during the research and analysis phase of documentation development.

The GPT follows a standardized research process that can be adapted to different documentation types. It produces a structured research report that writers can review and use as an input for creating an initial documentation draft.

The following sections describe how to design and configure the GPT.

### 1. Define the Research Architecture

The research architecture defines the research scope, information requirements, source hierarchy, and relationship between technical requirements and information sources.

#### Establish the Scope and Requirements

Define the documentation types that the GPT will support and identify the technical information required for each type.

Create a common research process with documentation-specific information requirements.

For example:

* An **Installation Guide** may require prerequisites, system requirements, installation procedures, configuration steps, and verification procedures.
* **Release Notes** may require information about the previous version, changes in the current version, resolved issues, known issues, and upgrade considerations.

This approach allows the GPT to follow a consistent research process while adapting its findings to the requirements of each documentation type.

#### Establish a Source Hierarchy

Define which sources the GPT should prioritize during research.

The source hierarchy should prioritize authoritative and current information, such as:

1. Official product documentation
2. Official product specifications
3. Official technical references
4. Approved internal documentation
5. Other reliable sources, when appropriate

The GPT should distinguish verified information from assumptions and should not present unsupported information as fact.

A defined source hierarchy improves the consistency and reliability of research findings.

#### Map Sources to Technical Requirements

Map each technical requirement to the sources that are most likely to contain the required information.

For example:

| Technical Requirement | Preferred Source |
| --- | --- |
| Installation prerequisites | Installation documentation |
| System requirements | Product documentation or specification |
| Configuration parameters | Configuration reference |
| Known issues | Release notes or support documentation |
| API behavior | API reference |

This mapping helps the GPT identify where to search for specific information and reduces unnecessary research across irrelevant sources.

### 2. Research and Verify Information

The GPT should extract findings from available sources and associate each finding with supporting evidence.

It should not present assumptions, interpretations, or unverified information as established facts.

#### Conduct Research and Extract Evidence

The GPT should:

* Research the identified sources.
* Extract information relevant to the defined requirements.
* Associate each finding with its supporting evidence and source.
* Distinguish between information explicitly stated in a source and conclusions derived from that information.
* Record the source used to support each significant finding.

This creates a traceable relationship between each research finding and its source.

#### Evaluate Research and Evidence

Evaluate each source using criteria such as:

* **Authority** — Is the source published by an authoritative organization or subject-matter expert?
* **Relevance** — Does the source directly address the research requirement?
* **Version** — Does the information apply to the required product or version?
* **Evidence strength** — Does the source provide sufficient evidence to support the finding?

Classify findings using a consistent verification status:

* **Verified** — Supported by sufficient evidence from an authoritative source.
* **Partially verified** — Some supporting information is available, but additional verification is required.
* **Unverified** — Required evidence is not available.
* **Conflicting** — Reliable sources provide different information.

This classification helps writers determine which findings can be used directly and which require additional verification.

#### Define Conflict-Resolution Rules

When multiple sources provide conflicting information, the GPT should compare the sources using the defined source hierarchy.

The GPT should not combine conflicting information or select an answer based solely on inference.

If the conflict cannot be resolved using the available evidence, the GPT should:

1. Identify the conflicting information.
2. Identify the sources involved.
3. Explain the conflict.
4. Mark the finding as **Conflicting**.
5. Create a verification question for the writer or appropriate subject-matter expert (SME).

This prevents unsupported conclusions from entering the documentation.

#### Define Information Gaps and Verification Records

The GPT should identify required technical information that cannot be verified using the available sources.

Missing information must be marked as **Unverified** rather than being assumed or generated.

For each significant information gap, the GPT should create a specific verification question that can be:

* Answered by the technical writer.
* Sent to an appropriate SME.
* Resolved by locating an authoritative source.

This converts missing information into a defined follow-up task.

### 3. Standardize the Research Output

Define a consistent output format so that research findings are presented in a predictable structure.

The research report should contain:

1. **Research Scope** — Defines what was investigated.
2. **Validated Findings** — Lists findings supported by evidence.
3. **Evidence and Sources** — Identifies the evidence and sources supporting each finding.
4. **Conflicts** — Documents conflicting information that requires resolution.
5. **Information Gaps** — Identifies required information that could not be verified.
6. **Follow-up Questions** — Provides questions for the writer or SME.

The output structure should remain consistent across documentation types, while the actual research requirements and findings vary according to the documentation type.

A standardized output makes research easier for technical writers to review, validate, and use during documentation development.

### 4. Build, Test, and Improve the GPT

After defining the research methodology, convert the methodology into instructions that the GPT can follow.

#### Define the System Instructions

Convert the following elements into the GPT's system instructions:

* Research methodology
* Documentation-specific requirements
* Source hierarchy
* Evidence evaluation criteria
* Verification statuses
* Conflict-resolution rules
* Information-gap rules
* Research output structure

The instructions should clearly define what the GPT should do, what it should avoid, and how it should present research findings.

#### Create the GPT Prompt

Use an AI tool to convert the research methodology into a structured prompt for the custom GPT.

Review the generated prompt before using it. The prompt should accurately represent the research methodology and verification rules defined in this guide.

Copy the finalized prompt for use when configuring the GPT.

#### Configure the Custom GPT

> **Assumption:** You have opened ChatGPT and signed in with an account that has access to GPT creation.

Follow these steps:

1. Open the **sidebar**.
2. Select **GPTs**.
3. Select **Create**.
4. Enter the prepared prompt in the GPT builder.
5. Select **Configure**.
6. Enter the GPT name in the **Name** field.
7. Enter a concise description in the **Description** field.
8. Enter the research methodology and behavioral rules in the **Instructions** field.
9. In **Knowledge**, upload approved reference material and representative research-output samples.
10. In **Capabilities**, enable the capabilities required by the research workflow, such as **Code Interpreter & Data Analysis** or **Image Generation**, when applicable.
11. Enable **Web Search** only if the research workflow requires the GPT to retrieve information from current external sources.
12. Create the GPT.
13. Test the GPT using representative research scenarios.

#### Test the GPT

Test the GPT using different documentation types and research scenarios.

The test should verify whether the GPT:

* Follows the defined research scope.
* Uses the required source hierarchy.
* Provides evidence for findings.
* Correctly identifies verification status.
* Detects conflicting information.
* Identifies information gaps.
* Generates useful follow-up questions.
* Follows the standardized output structure.
* Avoids presenting assumptions as facts.

Record the test results and update the GPT instructions when deficiencies are identified.

Repeat the test-and-improve cycle until the GPT consistently produces research reports that meet the defined requirements.

## Conclusion

A Research Assistant GPT can standardize repetitive research and analysis activities in the technical writing workflow.

The effectiveness of the GPT depends primarily on the quality of its research methodology, source hierarchy, verification rules, instructions, and testing process.

A well-defined workflow allows the GPT to produce traceable research findings while clearly identifying conflicts, information gaps, and items that require SME verification.

The resulting research report can provide technical writers with a structured and evidence-based starting point for developing documentation.
