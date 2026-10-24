PLACEMENTHUB

WORKFLOW INVESTIGATION & REDESIGN

TASK 1  |  ROUND 2 RECRUITMENT ASSESSMENT

A structured review of placement-opportunity publishing, student notifications,
external application redirection and faculty-facing activity statistics.

# 1. Executive Summary

PlacementHub is a placement-opportunity management concept intended to make campus recruitment information easier for students to discover and easier for faculty to monitor. The placement cell uploads an opportunity with its deadline, registration link, eligibility criteria and other relevant details. Students receive a notification, review the listing and select Apply, which redirects them to an external destination such as a Google Form or company application page.

Faculty-facing statistics can provide visibility into placement activity, but each metric must reflect what the system can actually observe or verify. An Apply click is not proof of a completed application, and eligibility figures depend on the criteria and student information available.

This report maps the described workflow, defines reporting statuses, proposes five synthetic acceptance tests, identifies risks and recommends an evaluation plan. ATS-style resume-to-job-description compatibility feedback is treated as a proposed enhancement unless confirmed in the working prototype. The report distinguishes the workflow design, proposed enhancements and items for future validation.

## Report scope and evidence discipline

The workflow description is based on the PlacementHub project information provided for this assessment.

Student conversations and notes informed the understanding of the workflow. The report focuses on the process information available and identifies opportunities for further validation.

Proposed controls and acceptance tests describe behaviours to validate; they are not claims that every control already exists in the prototype.

Any numerical impact example is clearly identified as an illustrative estimate.

# 2. Project Context and Objectives

## 2.1 Workflow need

Placement opportunities contain several details students need to act on: role information, eligibility criteria, deadline, registration link and application instructions. PlacementHub brings these details into a consistent listing and provides a path from notification to the employer’s external application destination.

Students: find opportunity details, review deadlines and eligibility, receive notifications and reach the correct application destination.

Placement cell: publish and maintain opportunity information consistently.

Faculty: review placement activity statistics, with clear distinctions between clicks, reported applications, verified applications and eligibility counts.

## 2.2 Objectives

Define a consistent opportunity record containing the deadline, registration link, eligibility criteria and other relevant details.

Make new opportunities visible to students through notifications.

Provide an Apply action that redirects to the configured external form or company page.

Present faculty-facing activity statistics with explicit definitions and data sources.

Evaluate workflow reliability through controlled, synthetic test scenarios.

Consider AI-assisted resume/JD compatibility feedback as an advisory student-preparation feature.

# 3. PlacementHub Workflow

The following process reflects the workflow described for this project.

## 3.1 End-to-end flow

The external application destination is a key workflow boundary. PlacementHub can record an Apply click when that event is tracked, but an external page opening alone does not prove that a student completed and submitted the application.

# 4. Roles, Responsibilities and Data Boundaries

# 5. Status Definitions and Reporting Logic

Clear labels help faculty interpret statistics correctly. A status should describe the event actually observed rather than imply a stronger level of confirmation.

## 5.1 Interpreting faculty statistics

Apply clicks can be measured from PlacementHub activity if the event is tracked. Completed external applications may require student-reported status, submission confirmation or an authorized data connection. Eligibility statistics depend on the criteria and student information available to the system. The interface should make these distinctions visible

.

# 6. Proposed AI Enhancement: Resume/JD Compatibility

A proposed AI add-on could help students prepare for a specific placement by comparing their resume with the job description attached to that opportunity. The purpose is to identify requirements clearly supported by the resume and areas that may be missing or insufficiently evidenced.

## 6.1 Proposed student journey

The student selects a placement opportunity and reviews its job description.

The student voluntarily provides a resume for comparison.

The feature identifies relevant requirements supported by the resume and requirements that appear missing or unclear.

The student receives a compatibility estimate and practical suggestions for improving clarity or relevance.

The student decides whether to revise the resume and proceeds to the employer’s application page independently.

## 6.2 Responsible design principles

Label the result as an ATS-style compatibility estimate, not the employer’s actual ATS score.

Show the job requirements and resume evidence behind the feedback where possible.

Do not guarantee shortlisting, hiring or selection based on a score.

Keep the feature advisory; do not automatically reject or rank students for employers.

Explain how resume data is used, restrict access and apply a clear retention policy.

Evaluate the feature with synthetic resumes and fictional job descriptions before relying on it with real users.

Implementation status: this feature is presented as a proposed enhancement for evaluation.

# 7. Evidence and Validation Plan

The workflow map is based on the project information provided. The candidate has indicated that student conversations and note-taking informed their understanding of the process. To keep the report evidence-based, no participant counts, direct quotations, formal survey results or measured outcomes are asserted without records supporting them.

Where additional discovery notes or test results are available, they can be incorporated to strengthen the evidence base.

# 8. Five Synthetic Acceptance Tests

The following acceptance tests provide a practical validation plan. They can be run with fictional opportunity details and synthetic student accounts.

## 8.1 Additional proposed AI checks

Use a synthetic resume and fictional job description with both matching and missing skills; check that feedback distinguishes evidence from gaps.

Change the selected job description and confirm that the comparison reflects the selected role.

Check that the output is labelled as an estimate and does not claim to be an employer ATS result.

Test unsupported or malformed resume files and confirm safe handling.

For each test run, record the date, environment/version, synthetic data used, steps performed, expected and actual results, and outcome (Pass, Fail, Blocked or Not Tested).

# 9. Illustrative Impact Model (Assumptions Only)

This illustrative model demonstrates one way to estimate staff-effort impact. Its assumptions can be replaced with baseline and pilot measurements when those data become available.

Under these assumptions, the illustrative difference is 140 minutes per month. The result is highly sensitive to request volume, handling time, exceptions and ongoing support. No payback-period claim is included because the implementation effort and savings are not measured; a real payback calculation should be made only after validating these inputs.

## 9.1 Sensitivity to request volume

These scenarios use the assumptions above to show how request volume can affect the estimated time difference. A pilot can refine the estimate using observed review, exception and support effort.

# 10. Risks and Practical Controls

# 11. Recommended Implementation and Evaluation Plan

1. Confirm the required opportunity fields and check that the placement cell can create or update listings consistently.

2. Check notification and Apply-redirection behaviour using fictional opportunities and a safe test account.

3. Confirm the definition and source of each faculty statistic, especially application completion and eligibility counts.

4. Run the five synthetic workflow tests and record actual outcomes; mark untested cases as Not Tested.

5. Review access permissions and student-data handling before expanding use.

6. Evaluate the AI resume/JD feature separately with synthetic data before describing its results or relying on it for student decisions.

7. If an authorized pilot is possible, compare baseline and pilot measures using the same definitions and include review, exception and support effort.

# 12. Conclusion

PlacementHub connects placement-cell opportunity publishing, student notifications, direct application redirection and faculty-facing placement statistics in one workflow. Its intended value is to give students a clearer path from opportunity discovery to the external application page while giving faculty more structured visibility into activity.

The workflow depends on precise status definitions: a notification being issued is not proof it was read, an Apply click is not proof of submission, and an eligibility figure is only as reliable as the criteria and data behind it. These distinctions support more trustworthy reporting.

The proposed ATS-style resume/JD compatibility feature may support student preparation if it remains explainable, privacy-conscious and advisory. The next step is to validate the actual prototype against the acceptance scenarios, clarify metric sources and use measured evidence before making performance claims.



| Candidate | YZ. Maahi Shayada Khanam |

| Enrollment number | 23STUCHH010059 |

| Programme | B.Tech - Data Science & Artificial Intelligence |

| Institution | ICFAI Foundation for Higher Education (IFHE) |

| Assessment | HKAIVERSE × Leanova Opex |

|---|---|





| Stage | Actor | Activity | Expected result |

| 1. Create opportunity | Placement cell | Uploads the opportunity announcement, deadline, registration link, eligibility criteria and other relevant details. | An opportunity record is created or updated. |

| 2. Notify students | PlacementHub | Makes a notification available to students for the opportunity. | Students are alerted to review the listing; issuance does not prove the notification was read. |

| 3. Review details | Student | Opens the opportunity and checks role information, deadline and eligibility criteria. | Student can decide whether to proceed. |

| 4. Select Apply | Student / PlacementHub | Apply redirects to the configured Google Form or company application page. | The external destination opens, subject to link availability. |

| 5. Record activity | PlacementHub / student | Apply-click activity may be recorded; completion is determined from whatever evidence is available. | Activity metrics use accurate, defined labels. |

| 6. Review statistics | Faculty | Views available statistics such as Apply clicks, application counts and eligibility-related figures. | Faculty gains visibility into opportunity activity, within the limits of available data. |

| 7. AI enhancement (proposed) | Student / AI feature | Compares resume content with a selected job description and offers compatibility feedback. | Student receives preparation guidance, not an employer decision. |

|---|---|---|---|





| Role | Primary responsibility | Boundary / control to validate |

| Placement cell | Create and maintain opportunity details, including deadlines, links and eligibility criteria. | Opportunity information should be complete and current before publication; the responsible editor should be clear. |

| Student | Review the opportunity, assess eligibility and select Apply when ready. | The student completes the application on the external destination and follows the employer’s instructions. |

| PlacementHub | Display listings, make notifications available, redirect Apply actions and present supported activity statistics. | Statistics should describe only what the system captures or can reliably confirm. |

| Faculty | Review placement activity and eligibility-related statistics. | Access should be limited to information required for the faculty role. |

| AI resume/JD feature (proposed) | Compare resume evidence with job requirements and provide preparation suggestions. | Advisory only; it should not make hiring decisions or claim to reproduce a proprietary ATS. |

|---|---|---|





| Metric / status | Meaning | Reporting rule |

| Opportunity published | Opportunity information is available to students. | Use for a listing that is available to students. |

| Notification issued | The system initiated or made a notification available. | Do not describe it as read unless that can be observed. |

| Apply clicked | A student selected Apply or the tracked event was recorded. | Measures an action, not a completed application. |

| External page opened | The configured Google Form or company page opened. | Does not prove that the form was submitted. |

| Application reported | Completion is reported through an available source or student confirmation. | Label the source; do not imply independent verification. |

| Application verified | Reliable confirmation or an authorized integration supports submission. | Use only when supporting evidence exists. |

| Eligibility count | Students identified as meeting listed criteria based on available data and stated rules. | Explain the criteria, data source and limitations. |

|---|---|---|





| Evidence area | What to record | Why it matters |

| Student discovery | Summarize the actual themes in the candidate’s notes; include counts or quotations only if recorded and appropriate to share. | Makes the user-discovery basis visible without overstating the method. |

| Prototype review | Record which functions were personally checked: opportunity listing, notification behaviour, Apply redirection and available statistics. | Keeps implementation claims aligned with observed behaviour. |

| Workflow tests | Run the synthetic scenarios and record the date, environment, actual result and any defect. | Shows what has and has not been validated. |

| Metric definitions | Confirm how clicks, reported applications, verified applications and eligibility figures are counted. | Prevents misleading faculty statistics. |

| Impact baseline | If access and permission allow, measure a baseline and compare it with a pilot using the same definitions. | Supports credible impact estimates. |

|---|---|---|





| Test | Scenario | Expected behaviour to validate | Evidence to capture |

| TC-01: Normal flow | Placement cell creates a complete fictional listing with deadline, registration link and eligibility criteria. | Listing becomes available as intended; notification behaviour is observed; selecting Apply opens the correct external destination. | Listing state, notification result, click event and destination. |

| TC-02: Missing information | A listing is submitted without a required deadline or registration link. | If required-field validation exists or is implemented, missing information is flagged and the listing is not treated as complete until corrected. | Missing field, observed response and correction path. |

| TC-03: Duplicate opportunity | Two similar fictional listings are entered for the same role and deadline. | If duplicate detection is implemented, a possible duplicate is flagged for review; records are not silently merged or deleted. | Records, warning/review behaviour and final decision. |

| TC-04: Unauthorized publication/edit | A test account without the relevant authority attempts to publish or change a listing. | Role-based permission controls should block the action if implemented; unauthorized changes must not be accepted. | Account role, attempted action, result and any defect. |

| TC-05: External application/status uncertainty | A student clicks Apply and opens an external page, but no submission confirmation returns to PlacementHub. | The click is recorded as a click; the application is not labelled verified solely because the page opened. | Click event and status shown in faculty statistics. |

|---|---|---|---|





| Input | Illustrative assumption |

| Placement-related requests per month | 20 |

| Current routine handling effort | 25 minutes per request |

| Current rework | 20% of requests × 15 additional minutes |

| Proposed routine effort | 12 minutes per request |

| Human review in proposed process | 5 minutes per request |

| Proposed exception handling | 10% of requests × 10 additional minutes |

| Ongoing support | 60 minutes per month |

| One-time implementation effort | 8 hours |

|---|---|





| Measure | Calculation | Illustrative result |

| Current routine effort | 20 × 25 | 500 min/month |

| Current rework | 20 × 20% × 15 | 60 min/month |

| Current total | 500 + 60 | 560 min/month (9.33 hours) |

| Proposed routine + review | 20 × (12 + 5) | 340 min/month |

| Proposed exception handling | 20 × 10% × 10 | 20 min/month |

| Proposed total incl. support | 340 + 20 + 60 | 420 min/month (7 hours) |

| Illustrative net time difference |  | 140 min/month (2.33 hours) |

|---|---|---|





| Requests/month | Current effort | Proposed effort | Difference |

| 10 | 280 min | 240 min | 40 min (0.67 h) |

| 20 | 560 min | 420 min | 140 min (2.33 h) |

| 40 | 1,120 min | 780 min | 340 min (5.67 h) |

|---|---|---|---|





| Risk | Practical control / validation |

| Outdated deadline or eligibility details | Keep opportunity details consistent and current; make the responsible editor clear and review material changes. |

| Notification not noticed or delivered | Use accurate notification wording and a visible opportunity listing; do not treat issuance as proof it was read. |

| Apply click mistaken for completed application | Report Apply clicks separately from reported and verified applications. |

| Incorrect eligibility statistics | State the eligibility criteria and data source; distinguish an estimate from a verified count. |

| Unauthorized listing change | Limit publication/editing privileges to appropriate roles and test permission behaviour. |

| Resume privacy or exposure | Make resume upload voluntary, restrict access, explain its purpose and apply reasonable retention limits. |

| Misleading AI score | Show evidence and gaps, label the score advisory and do not use it as an automated hiring decision. |

| System or external-link failure | Where supported, show a clear failure state and a practical way to retry or revisit the opportunity. |

| Illustrative estimates mistaken for results | Label assumptions and use measured baseline/pilot data before making claims. |

|---|---|
