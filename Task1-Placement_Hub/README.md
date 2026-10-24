# Task 1 --- PlacementHub Workflow Investigation and Redesign

## Candidate Details

-   **Name:** YZ. Maahi Shayada Khanam
-   **Programme:** B.Tech in Artificial Intelligence and Data Science
-   **Institution:** ICFAI Foundation for Higher Education (IFHE),
    Hyderabad
-   **Admission Batch:** 2023--2027
-   **Assessment:** HKAIVERSE × LEANOVA OPEX --- Round 2

## 1. Task Overview

This task investigates a placement-related workflow referred to as
PlacementHub. The report maps how an opportunity moves through the
placement process, identifies responsibilities and status definitions,
and proposes a more reliable workflow with clearer evidence of outcomes.

The central design principle is that a user action should not be
confused with a verified real-world outcome. For example, clicking
**Apply** or opening an external application page does not by itself
prove that the student completed the employer's application.

## 2. Problem Context

A placement workflow can involve several hand-offs: the placement cell
publishes an opportunity, students receive or discover the listing,
students review the eligibility and role details, and students proceed
to an external application destination. Faculty may also view summary
statistics.

These steps can create ambiguity if the system does not clearly
distinguish between: - An opportunity being published or updated. - A
student viewing a listing. - A student clicking an Apply link or opening
an external page. - An application being completed and independently
verified. - A faculty statistic being derived from a clearly defined
source.

The report therefore emphasizes explicit statuses, clear ownership, and
careful reporting rather than treating incomplete evidence as proof of
completion.

## 3. Workflow and Responsibilities

The report documents the workflow steps and the roles involved. It
proposes clearer responsibility boundaries for the placement cell,
students, faculty, and the system. The intent is to make hand-offs
easier to understand, reduce status ambiguity, and establish what each
role is allowed to view or change.

Status definitions and reporting logic are included so that statistics
can be interpreted consistently. Application completion should only be
reported when the available evidence supports that claim.

## 4. Proposed Improvement: Advisory AI Support

The report proposes an AI-assisted resume/job-description compatibility
feature as an advisory aid. It is intended to help students compare
their resume with a role description and identify potentially relevant
skills or gaps.

The feature is not presented as an employer ATS score, a hiring
prediction, or a guarantee of eligibility. Its output should be
explainable and treated as guidance rather than as a consequential
decision. The proposal should be evaluated separately from the core
workflow and tested with synthetic data before any broader use.

## 5. Evidence and Validation

The report distinguishes observed facts, estimates, assumptions, and
proposals. It includes synthetic acceptance tests for scenarios such
as: - A normal workflow. - Missing information. - A duplicate
opportunity. - An unauthorized edit. - Uncertainty about whether an
external application was completed.

Synthetic cases are a validation plan, not evidence that a live system
has passed the tests. Actual outcomes should be recorded only after
tests are executed, with untested cases labelled accordingly.

## 6. Impact Model, Risks, and Controls

An illustrative impact model is used to explain how process changes
could be evaluated. Its assumptions should remain visible and should not
be presented as measured results. The report also identifies risks and
practical controls, including access boundaries, reliable status
definitions, privacy-conscious handling of student information, and
human oversight for AI-assisted suggestions.

## 7. Implementation Approach

The implementation plan sequences workflow clarification, confirmation
of required opportunity fields, notification and Apply-redirection
checks, definition of faculty statistics, synthetic workflow testing,
review of access permissions, and separate evaluation of the AI-assisted
feature. If an authorized pilot is possible, baseline and pilot measures
should use the same definitions.

## 8. Expected Deliverables

The Task 1 folder should contain the final report and the supporting
artifacts actually prepared for the assessment, such as: - Workflow
diagram or process map. - Evidence log that labels observations,
estimates, and assumptions. - Calculations and assumptions behind the
illustrative impact model. - Synthetic test cases and a test-results
record, clearly distinguishing planned tests from executed tests. - Any
supporting notes required by the assessment instructions.

## 9. Key Limitations and Responsible Reporting

-   An Apply click or external page opening is not proof of a completed
    application.
-   Synthetic acceptance tests must not be described as live-system
    results.
-   Illustrative impact estimates must not be described as measured
    improvements.
-   The AI compatibility feature is proposed and advisory; it should not
    replace human judgment or determine hiring outcomes.
-   Any pilot or data collection must follow the applicable
    authorization and privacy safeguards.

## Submission Metadata

-   **Repository path:** `Task1-Placement_Hub/`
-   **Report file:** Task1_PlacementHub.docx.
