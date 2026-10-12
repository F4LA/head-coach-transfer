# Master Plan — R5 Head coach role defined, improved and transferred to Brent
**Company:** Strong Standard   **Rock owner:** Brent   **Support:** Bernardo (owns tasks in this Rock)   **Sprint:** S4-2026   **Go-live:** none stated

## What this is
The full task layout for this Rock: every project, milestone and task, its owner, type, dependencies, and execution order per person. Source of truth for *why* is the Decision Log. Source of truth for *where the work stands and when it lands* is the Operations Dashboard — this file holds no status and no dates.

Rules: one task = one chat; specs approved before building.

Durations are carried here as work days and wait days exactly as the Rock Plan states them. They are inputs the dashboard schedules from, not dates. The Operations Dashboard rounds every work-day value up to the nearest 0.25 (decision D-105 in the dashboard repo), so the numbers it schedules from can be slightly higher than the ones below. This Rock has no milestone deadlines and no go-live date.

An asterisk on a dependency means it reaches into another Project inside this Rock. No dependency in this Rock crosses into another Rock.

**Changing this file takes three steps, and none of them is optional.** The plan changes only when (1) a Decision Log row records the change, (2) this file is edited to match, and (3) the Rock's JSON fragment is regenerated in the Rock Planner and handed to the Sprint project so the dashboard sees the same plan. A change that stops after step 2 leaves the dashboard scheduling work that no longer exists.

## Definition of Done
Verbatim from Sprint Commitments.

This Rock is complete when:
1. The head coach role is defined in one document: every responsibility the role owns, with its cadence (weekly, monthly, quarterly), reviewed against what Bernardo does today and marked kept, improved, dropped or added. Agreed by Bernardo and Brent.
2. The head coach SOP is written from that definition: for each responsibility, what gets done, how, and with what.
3. The role's KPIs are defined with the source of each number named, and every KPI that can be measured today is being measured.
4. The client onboarding carryover from S3 is finished:
   4a. The kickoff presentation automation is live and validated.
   4b. The onboarding and kickoff SOP is updated, including the coach competency questionnaire.
   4c. All four coaches are calibrated on the new kickoff and roadmap process and have passed competency.
   4d. The audit of coach kickoff calls is done and its findings are written down.
   4e. The inventory and shipment dashboard is built and the first batch is shipped.
5. The new coach onboarding process is rebuilt and Mikari is taking clients:
   5a. The current coach onboarding process has been reviewed, and every element is marked kept, improved, deleted or added.
   5b. Every change that Bernardo and Brent mark as required before Mikari starts is implemented, including the exercise training materials and the SOP on how and why training is structured. Everything else goes to the S5 list.
   5c. Mikari has gone through the updated process from start to finish.
   5d. Mikari is coaching at least one client.
6. The end meso process is defined and automated: Brent and Bernardo have agreed and documented the call structure, and the automation has produced the end meso presentation for at least one real client, reviewed by the coach before the call.
7. Brent has run every weekly, monthly and per-client responsibility in the SOP at least once, with Bernardo present.
8. The coaching team, the clients and the systems point to Brent: he has the accesses, and the team has been told who to go to for what.
9. Bernardo and Brent have agreed the metrics the head coach needs, and Bernardo has built the head coach dashboard showing all of them. Brent has confirmed each number is calculated correctly.
10. The coaching SOP has been reviewed section by section, each section marked kept, updated, deleted or added, updated to match, and loaded into NotebookLM.

---

## Project R5-P1 — Define the role, KPIs and dashboard
**Owner:** Brent
**Objective:** Role, KPIs and head coach dashboard are agreed and measurable.

### R5-M1 — Role definition agreed by Bernardo and Brent
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M1-t1 | Write down everything Bernardo does today as head coach, including what he does only occasionally, such as the quarterly coach audit. | Bernardo | work | 0.3 | 0 | — |
| R5-M1-t2 | Add what the role should be doing and is not getting done today for lack of time. | Bernardo | work | 0.3 | 0 | R5-M1-t1 |
| R5-M1-t3 | Merge Bernardo's list with Brent's four areas and the operational list, remove duplicates, and add what came up on the September 22 call. | Brent | work | 0.5 | 0 | R5-M1-t2 |
| R5-M1-t4 | For each responsibility decide kept, improved, dropped or added, give it a cadence, say who owns it and who executes it, and review Brent's Overview draft against the list. | Brent | work | 0.5 | 0 | R5-M1-t3 |
| R5-M1-t5 | Brent and Bernardo agree the final list of responsibilities. Bernardo attends. | Brent | meeting | 0.1 | 0 | R5-M1-t3, R5-M1-t4 |
| R5-M1-t6 | Bernardo reviews the agreed role definition and approves it. | Bernardo | approval | 0.3 | 0 | R5-M1-t5 |

### R5-M2 — Dashboard metrics agreed and defined
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M2-t1 | List every place where retention and churn data lives today. | Bernardo | work | 0.2 | 0 | — |
| R5-M2-t2 | Decide the metrics the head coach needs. Bernardo attends. | Brent | meeting | 0.2 | 0 | R5-M2-t1 |
| R5-M2-t3 | Define each agreed metric: what it counts and where the data comes from. | Bernardo | work | 0.3 | 0 | R5-M2-t2 |
| R5-M2-t4 | Check how each metric is calculated today and whether the numbers are correct. | Bernardo | work | 0.5 | 0 | R5-M2-t3 |
| R5-M2-t5 | Validate Bernardo's check of the calculations. | Brent | work | 1 | 0 | R5-M2-t4 |

### R5-M3 — KPIs defined, measurable ones measured
**Depends on:** R5-M1, R5-M2

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M3-t1 | Go through the proposed KPIs by area, name where each number comes from, and mark each one: measurable today, needs a source built, or cannot be measured yet. | Brent | work | 0.5 | 0 | — |
| R5-M3-t2 | Decide the KPIs Brent is unsure about and add the kickoff upsell rate. Bernardo attends. | Brent | meeting | 0.2 | 0 | R5-M3-t1 |
| R5-M3-t3 | Start measuring every KPI that can be measured today and take the first reading. No targets yet. | Brent | work | 1 | 0 | R5-M3-t2 |

### R5-M4 — Head coach dashboard built and confirmed
**Depends on:** R5-M2

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M4-t1 | Build the head coach dashboard with the agreed and defined metrics. | Bernardo | work | 2 | 0 | — |
| R5-M4-t2 | Review the dashboard and confirm it shows what Brent needs and that each number is right. | Brent | approval | 0.5 | 0 | R5-M4-t1 |

---

## Project R5-P2 — Kickoff and roadmap automation
**Owner:** Bernardo
**Objective:** Kickoff and roadmap builders are tested, released to the coaches and live.

### R5-M5 — Roadmap builder released to coaches
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M5-t1 | Run the roadmap builder end to end in production with a test client, and pilot it from Brent's own account. | Bernardo | work | 3 | 0 | — |
| R5-M5-t2 | Record a Loom and send the Slack message asking Ceci, Jackie and Miguel to test the roadmap builder with their test client and DM Brent the files. | Brent | work | 0.1 | 0 | R5-M5-t1 |
| R5-M5-t3 | Wait while Ceci, Jackie and Miguel test the roadmap builder and send their files to Brent. Elapsed time only. | Brent | work | 0 | 2 | R5-M5-t2 |

### R5-M6 — Kickoff presentation builder built
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M6-t1 | Finish the kickoff presentation builder: create the project from the template, verify what the readers of the roadmap data file do, build the fixed template for the overview image, and define how the 38 placeholders get filled. | Bernardo | work | 2 | 0 | — |

### R5-M7 — Automation live and validated
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M7-t1 | Create the fictional clients used to test the builder and later to calibrate the coaches. | Bernardo | work | 0.3 | 0 | — |
| R5-M7-t2 | Test the kickoff builder with a fictional client until it works. | Bernardo | work | 0.5 | 0 | R5-M6, R5-M7-t1 |
| R5-M7-t3 | Brent tests the kickoff builder from his own account. | Brent | work | 0.3 | 0 | R5-M7-t2 |
| R5-M7-t4 | Record and send a video to the coaches showing how the kickoff builder works, and ask them to test it with their fictional client. | Bernardo | work | 0.1 | 0 | R5-M7-t3, R5-M5 |
| R5-M7-t5 | Wait while the coaches run the kickoff builder and send their presentations to Bernardo. Elapsed time only. | Bernardo | work | 0 | 1 | R5-M7-t4 |
| R5-M7-t6 | Review the presentations the coaches sent and confirm the kickoff builder works. | Bernardo | work | 0.3 | 0 | R5-M7-t5 |
| R5-M7-t7 | Wait while each coach records a Loom of a mock kickoff call with a fictional client, using the presentation, and sends it to Brent. Elapsed time only. | Brent | work | 0 | 2 | R5-M9-t1* |
| R5-M7-t8 | Cutover: switch the client-facing onboarding to the new system in one go, on a set night. | Bernardo | work | 1 | 0 | R5-M7-t6, R5-M7-t7 |

---

## Project R5-P3 — Kickoff standard: SOP, calibration, audit, shipment
**Owner:** Brent
**Objective:** Onboarding and kickoff SOP updated, coaches calibrated, kickoff calls audited, and the shipment system built with its first batch shipped.

### R5-M8 — Onboarding and kickoff SOP updated, including the coach competency questionnaire
**Depends on:** none (but its first task reaches into R5-P2)

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M8-t1 | Write the coach competency questionnaire, completed by each coach after the calibration call. | Brent | work | 0.3 | 0 | R5-M7-t3* |
| R5-M8-t2 | Update the onboarding and kickoff SOP for the new structure, including the questionnaire. | Brent | work | 1.5 | 0 | R5-M8-t1 |
| R5-M8-t3 | Load the updated SOP into NotebookLM. | Brent | work | 0.3 | 0 | R5-M8-t2 |

### R5-M9 — Four coaches calibrated and passed
**Depends on:** R5-M8

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M9-t1 | One training call with Ceci, Miguel and Jackie on how to guide the kickoff call with the new presentation. Brent is considered calibrated and passed. | Brent | meeting | 0.3 | 0 | — |
| R5-M9-t2 | Wait while the three coaches complete the competency questionnaire. Elapsed time only. | Brent | work | 0 | 2 | R5-M9-t1 |
| R5-M9-t3 | Record who passed. | Brent | work | 0.2 | 0 | R5-M9-t2 |
| R5-M9-t4 | Contingent: repeat the practice with any coach who did not pass. | Brent | work | 1 | 0 | R5-M9-t3 |

### R5-M10 — Kickoff call audit done, findings written
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M10-t1 | Choose the kickoff calls to audit from each coach. | Brent | work | 0.2 | 0 | — |
| R5-M10-t2 | Audit the chosen calls against the defined kickoff standard. | Brent | work | 0.5 | 0 | R5-M10-t1 |
| R5-M10-t3 | Write the findings, separating what is one coach from what is the whole team. | Brent | work | 0.2 | 0 | R5-M10-t2 |
| R5-M10-t4 | Give feedback to each coach. | Brent | work | 0.4 | 0 | R5-M10-t3 |
| R5-M10-t5 | Contingent: update the SOP or the training materials if a problem is systemic. | Brent | work | 0.3 | 0 | R5-M10-t3 |
| R5-M10-t6 | Decide how often the head coach audits, how calls are picked and how feedback is recorded. | Brent | meeting | 0.2 | 0 | R5-M10-t3 |

### R5-M11 — Kickoff upsell standard and feedback loop
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M11-t1 | Meet with the coaches about how the upsell is presented at the kickoff. | Brent | meeting | 0.2 | 0 | — |
| R5-M11-t2 | Standardize how the upsell is presented and set up a feedback loop for the coaches. | Brent | work | 1 | 0 | R5-M11-t1 |

### R5-M12 — Shipment dashboard built, first batch shipped
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M12-t1 | Build the inventory and shipment dashboard as one system: weekly shipment trigger, mark shipped and size, inventory counts and restock notification. It pulls address and shirt size from the new intake form. | Bernardo | work | 3 | 0 | — |
| R5-M12-t2 | Confirm that the first order of about 50 shirts arrived. | Brent | work | 0.2 | 0 | — |
| R5-M12-t3 | Define who operates the shipment system. | Brent | work | 0.5 | 0 | R5-M12-t1 |
| R5-M12-t4 | Ship the first batch, shirt and note, to the next cohort of new clients, batched weekly and after the grace period. | Brent | work | 0.5 | 10 | R5-M12-t1, R5-M12-t2, R5-M7-t8* |
| R5-M12-t5 | Message the clients who received it to confirm arrival and wait for their replies. | Brent | work | 0.2 | 2 | R5-M12-t4 |
| R5-M12-t6 | Contingent: adjust the dashboard and the shipping process from what the first shipment shows. | Bernardo | work | 0.3 | 0 | R5-M12-t5 |

---

## Project R5-P4 — Rebuild coach onboarding and start Mikari
**Owner:** Brent
**Objective:** The current coach onboarding is reviewed, the required changes are implemented, and Mikari goes through it and starts coaching a client.

### R5-M13 — Current onboarding reviewed, every element marked
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M13-t1 | Review the current coach onboarding on his own: what works, what is unclear, what is missing and what is unnecessary. | Bernardo | work | 0.3 | 0 | — |
| R5-M13-t2 | Review the current coach onboarding on his own, with the same four questions. | Brent | work | 1 | 0 | — |
| R5-M13-t3 | Compare both reviews, agree the major gaps and mark every element kept, improved, deleted or added. Bernardo attends. | Brent | meeting | 0.3 | 0 | R5-M13-t1, R5-M13-t2 |

### R5-M14 — Required changes implemented
**Depends on:** R5-M13

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M14-t1 | Decide which changes are required before Mikari starts. The rest goes to the next sprint's list. | Brent | meeting | 0.3 | 0 | — |
| R5-M14-t2 | Define what a new coach must learn, in what order, and what to demonstrate before coaching clients alone. | Brent | meeting | 0.3 | 0 | R5-M14-t1 |
| R5-M14-t3 | Build the training materials the required changes need: exercise selection, progression, volume, intensity, substitutions and modifications. | Brent | work | 1 | 0 | R5-M14-t1 |
| R5-M14-t4 | Write the SOP on how and why Strong Standard structures training. | Brent | work | 1 | 0 | R5-M14-t3 |
| R5-M14-t5 | Implement the rest of the required changes to the coach onboarding. | Brent | work | 3 | 0 | R5-M14-t1 |
| R5-M14-t6 | Write the learning path into the onboarding: what to read, watch and practise, in order. | Brent | work | 0.5 | 0 | R5-M14-t2 |
| R5-M14-t7 | Review the implemented changes, including the training materials and the training SOP, and approve them before Mikari starts. | Bernardo | approval | 0.3 | 0 | R5-M14-t2, R5-M14-t3, R5-M14-t4, R5-M14-t5, R5-M14-t6 |

### R5-M15 — Mikari through the updated process
**Depends on:** R5-M14

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M15-t1 | Start Mikari on the updated coach onboarding and give her what she needs to go through it from start to finish. | Brent | work | 0.2 | 0 | — |
| R5-M15-t2 | Wait while Mikari goes through the updated process from start to finish. Elapsed time only. | Brent | work | 0 | 10 | R5-M15-t1 |
| R5-M15-t3 | Write down the problems that appear during Mikari's run and adjust the process as they appear. | Brent | work | 1 | 0 | R5-M15-t1 |
| R5-M15-t4 | Close the run: confirm the adjusted process holds from start to finish and list what goes to the next sprint's list. | Brent | work | 1 | 0 | R5-M15-t2, R5-M15-t3 |

### R5-M16 — Mikari coaching a client
**Depends on:** R5-M15

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M16-t1 | Define what "ready to take clients" means and confirm Mikari meets it. | Brent | work | 1 | 0 | — |
| R5-M16-t2 | Assign Mikari her first client and confirm she is coaching. | Brent | work | 0.5 | 0 | R5-M16-t1 |
