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

---

## Project R5-P5 — End meso process and automation
**Owner:** Brent
**Objective:** The end meso call structure is agreed and documented, and the automation produces the end meso presentation for a client, reviewed by the coach.

### R5-M17 — Call structure agreed and documented
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M17-t1 | Audit the current end meso deck and call structure on his own: what information coaches have, what decisions they make, what is missing and what is unnecessary. | Bernardo | work | 0.3 | 0 | — |
| R5-M17-t2 | Audit the current end meso deck and call structure on his own, with the same questions. | Brent | work | 1 | 0 | — |
| R5-M17-t3 | Compare both audits and write a proposal for Brent: what Bernardo would not do from Brent's audit and why, and what he would add. | Bernardo | work | 0.3 | 0 | R5-M17-t1, R5-M17-t2 |
| R5-M17-t4 | Talk through the proposal and agree what has to change in the call structure. Bernardo attends. | Brent | meeting | 0.3 | 0 | R5-M17-t3 |
| R5-M17-t5 | Define the data the call needs: program start date, starting weight, measurements and photos, data from about eight weeks ago, the most recent data, the original intake and the client's reason for starting, and the current roadmap with its history. | Brent | work | 0.3 | 0 | R5-M17-t4 |
| R5-M17-t6 | Define the coach's decisions: whether the outcome goal still makes sense or should change, whether training or nutrition needs adjusting, and whether the roadmap changes. | Brent | work | 0.3 | 0 | R5-M17-t4 |
| R5-M17-t7 | Write the agreed call structure into one document: purpose, the conversation, the client data required, the coach decisions required and the outputs afterwards. | Brent | work | 0.2 | 0 | R5-M17-t4 |
| R5-M17-t8 | Define what satisfaction is asked live at end meso and how dissatisfaction reaches the head coach. | Brent | meeting | 0.3 | 0 | R5-M17-t4 |
| R5-M17-t9 | Define the criteria for asking for referrals and a Google review at the second end meso. | Brent | meeting | 0.3 | 0 | R5-M17-t4 |
| R5-M17-t10 | Review the finished call structure document and approve it. | Bernardo | approval | 0.3 | 0 | R5-M17-t5, R5-M17-t6, R5-M17-t7, R5-M17-t8, R5-M17-t9 |

### R5-M18 — End meso automation built and tested
**Depends on:** R5-M17, R5-M5, R5-M6

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M18-t1 | Approve the end meso presentation design in Google Slides, with the agreed call structure in mind. | Bernardo | approval | 0.1 | 0 | — |
| R5-M18-t2 | Confirm that the way data reaches the presentation works: mesocycle 1 fills from the kickoff information, later ones from where the previous mesocycle started, and clients without history can be filled in by hand. | Bernardo | work | 0.5 | 0 | R5-M18-t1 |
| R5-M18-t3 | Build the end meso automation and its presentation template with two paths: with history, it asks for the client's email and reads the rest; without history, it asks for the data each section needs, such as goals. | Bernardo | work | 2 | 0 | R5-M18-t2 |
| R5-M18-t4 | Test the path without history with an existing client, loading the data the builder asks for. | Bernardo | work | 0.1 | 0 | R5-M18-t3 |
| R5-M18-t5 | Wait for the first client whose kickoff call used the new system, plus one week. Elapsed time only. | Bernardo | work | 0 | 9 | R5-M7-t8* |
| R5-M18-t6 | Test the path with history on that client, loading made-up progress data. | Bernardo | work | 0.1 | 0 | R5-M18-t3, R5-M18-t5 |
| R5-M18-t7 | Contingent: fix what the two tests show. | Bernardo | work | 1 | 0 | R5-M18-t4, R5-M18-t6 |
| R5-M18-t8 | Hand the automation to the coaches so they can start using it. | Bernardo | work | 0.1 | 0 | R5-M18-t4, R5-M18-t6 |

### R5-M19 — End meso presentation produced for a real client, coach-reviewed
**Depends on:** R5-M18-t4

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M19-t1 | Review the end meso presentation produced for the existing client, before the call, as the coach would. | Brent | work | 0.1 | 0 | R5-M18-t4 |

---

## Project R5-P6 — Transfer the running responsibilities to Brent
**Owner:** Brent
**Objective:** Each running responsibility is walked through, written into the SOP and run once by Brent.

### R5-M20 — Weekly team rhythm
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M20-t1 | Record a Loom explaining to Brent how the Pulse and coaching calls are run today, with the tools and the data. | Bernardo | work | 0.1 | 0 | — |
| R5-M20-t2 | Write or confirm the SOP section for the Pulse and coaching calls. | Brent | work | 0.3 | 0 | R5-M20-t1, R5-M1* |
| R5-M20-t3 | Brent runs the Pulse and coaching call for the first time. Bernardo attends. | Brent | meeting | 0.1 | 5 | R5-M20-t2 |
| R5-M20-t4 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M20-t3 |
| R5-M20-t5 | Write the SOP section for coach training, meaning the office hours. This is a new responsibility. | Brent | work | 0.3 | 0 | R5-M1* |
| R5-M20-t6 | Brent runs the office hours for the first time. Bernardo attends. | Brent | meeting | 0.2 | 5 | R5-M20-t5 |
| R5-M20-t7 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M20-t6 |
| R5-M20-t8 | Give Brent the existing recorded retention training videos, with a note on which to watch and in what order. | Bernardo | work | 0.2 | 0 | — |
| R5-M20-t9 | Watch the retention training videos and build a live training on the retention pillars that can be repeated with all the coaches. | Brent | work | 0.5 | 0 | R5-M20-t8 |
| R5-M20-t10 | Write the SOP section for retention training. | Brent | work | 0.3 | 0 | R5-M20-t9, R5-M1* |
| R5-M20-t11 | Brent runs the retention training live with all the coaches for the first time. Bernardo attends. | Brent | meeting | 0.2 | 20 | R5-M20-t10 |
| R5-M20-t12 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M20-t11 |

### R5-M21 — Weekly client oversight
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M21-t1 | Record a Loom explaining how the flag system review is done today: how often, what each flag requires, when leadership gets involved, the two weekly satisfaction questions and early detection of a coach and client mismatch. | Bernardo | work | 0.3 | 0 | — |
| R5-M21-t2 | Write or confirm the SOP section for the flag system review. | Brent | work | 0.3 | 0 | R5-M21-t1, R5-M1* |
| R5-M21-t3 | Brent runs the flag system review for the first time. Bernardo attends. | Brent | meeting | 0.3 | 5 | R5-M21-t2 |
| R5-M21-t4 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M21-t3 |
| R5-M21-t5 | Write the SOP section for cadence monitoring (weekly, monthly, quarterly) using the cadence tracking document. This is a new responsibility. | Brent | work | 0.3 | 0 | R5-M1*, R5-M4* |
| R5-M21-t6 | Brent runs cadence monitoring for the first time. Bernardo attends. | Brent | meeting | 0.2 | 5 | R5-M21-t5 |
| R5-M21-t7 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M21-t6 |
| R5-M21-t8 | Record a Loom explaining how the review of the coaches' kickoff and end meso calls is done today. | Bernardo | work | 0.1 | 0 | — |
| R5-M21-t9 | Write or confirm the SOP section for the review of kickoff and end meso calls. | Brent | work | 0.3 | 0 | R5-M21-t8, R5-M1*, R5-M10*, R5-M11*, R5-M17* |
| R5-M21-t10 | Brent runs the review of kickoff and end meso calls for the first time. Bernardo attends. | Brent | meeting | 0.4 | 5 | R5-M21-t9 |
| R5-M21-t11 | Correct the SOP section with what the first run showed. | Brent | work | 0.3 | 0 | R5-M21-t10 |

### R5-M22 — Community
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M22-t1 | One-hour meeting with Brent: Bernardo explains what the community calls must achieve and how the day is managed so Brent can organise them his way, and they decide that Gaby takes over posting the schedules. Brent attends. | Bernardo | meeting | 0.2 | 0 | — |
| R5-M22-t2 | Write the SOP section for organising the community calls. | Brent | work | 0.3 | 0 | R5-M22-t1, R5-M1* |
| R5-M22-t3 | Brent organises the first community calls his own way, with Gaby handling the posting. | Brent | work | 0.2 | 7 | R5-M22-t2 |
| R5-M22-t4 | One-hour meeting with Brent to decide how community engagement works: where the post comes from with Gaby, who sends the birthday gifts and what the gift is. Brent attends. | Bernardo | meeting | 0.2 | 0 | — |
| R5-M22-t5 | Prepare what the process needs: message templates for Gaby, how the information is collected, and the systems behind it. | Bernardo | work | 0.5 | 0 | R5-M22-t4 |
| R5-M22-t6 | Write the SOP section for community engagement: birthday gifts and posts, and celebrating every client who renews. | Brent | work | 0.3 | 0 | R5-M22-t5, R5-M1* |
| R5-M22-t7 | Brent runs community engagement for the first time. | Brent | work | 0.2 | 7 | R5-M22-t6 |

### R5-M23 — Quarterly audit and reporting
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M23-t1 | Do this quarter's coach audit and send it to Brent in a Loom, so Brent sees how it is done. | Bernardo | work | 1 | 0 | — |
| R5-M23-t2 | Write the SOP section for the quarterly coach audit. | Brent | work | 0.3 | 0 | R5-M23-t1 |
| R5-M23-t3 | Correct the SOP section with what the audit showed. | Brent | work | 0.2 | 0 | R5-M23-t2 |
| R5-M23-t4 | Write the SOP section for reporting to Joey and Bernardo: systemic issues such as pricing and offer gaps, client and coach trends, and how the coaching system is evolving. | Brent | work | 0.1 | 0 | R5-M1* |
| R5-M23-t5 | Brent gives the first report. Bernardo attends. | Brent | meeting | 0.3 | 20 | R5-M23-t4 |
| R5-M23-t6 | Correct the SOP section with what the first report showed. | Brent | work | 0.2 | 0 | R5-M23-t5 |

---

## Project R5-P7 — SOPs and hand-off
**Owner:** Brent
**Objective:** The head coach SOP is complete, everything points to Brent, and the coaching SOP is reviewed and updated.

### R5-M24 — Head coach SOP complete
**Depends on:** none (but its first task reaches into R5-P1)

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M24-t1 | Start from Brent's first SOP draft and align it with the agreed role definition. | Brent | work | 0.2 | 0 | R5-M1* |
| R5-M24-t2 | Put the outcomes of the end meso call, the flag review and the calibration into the SOP. | Brent | work | 0.3 | 0 | R5-M9*, R5-M17*, R5-M21* |
| R5-M24-t3 | Read the whole SOP from start to finish for contradictions, unclear expectations and steps that do not exist in practice. | Brent | work | 0.5 | 0 | R5-M24-t1, R5-M24-t2, R5-M20*, R5-M21*, R5-M22*, R5-M23* |
| R5-M24-t4 | Write Bernardo's role after the transfer into the SOP: support and escalation, not operator. | Brent | work | 0.2 | 0 | R5-M24-t3 |
| R5-M24-t5 | Make the final corrections, load the SOP into NotebookLM and confirm it references the right version. | Brent | work | 0.4 | 0 | R5-M24-t4 |

### R5-M25 — Everything points to Brent
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M25-t1 | Tell the coaching team that Brent is taking the role. | Brent | work | 0.1 | 0 | — |
| R5-M25-t2 | List every system, channel, meeting and document the role touches, such as the Clients shared drive, GHL, Everfit, Slack and the roadmap builder project, and note what access Brent is missing. | Brent | work | 0.1 | 0 | R5-M1* |
| R5-M25-t3 | Give Brent the access and admin rights he needs. | Bernardo | approval | 0.2 | 0 | R5-M25-t2 |
| R5-M25-t4 | Redirect what Gaby handles on the head coach's behalf so it points to Brent. | Brent | work | 0.2 | 0 | R5-M1* |
| R5-M25-t5 | Decide what Bernardo stops doing and from when: from the day after the sprint closes he performs no head coach task and is escalation support. Bernardo attends. | Brent | meeting | 0.2 | 0 | R5-M1* |
| R5-M25-t6 | Tell the coaching team who to go to for what, everywhere they currently go to Bernardo. | Brent | work | 0.2 | 0 | R5-M25-t5, R5-M20*, R5-M21*, R5-M22*, R5-M23* |
| R5-M25-t7 | Check whether anything client-facing still names Bernardo in the role. | Brent | work | 0.3 | 0 | R5-M25-t5 |

### R5-M26 — Coaching SOP reviewed, sections marked, changes agreed
**Depends on:** none

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M26-t1 | Read the existing coaching SOP from start to finish and compare it with how coaching actually runs. | Brent | work | 0.5 | 0 | — |
| R5-M26-t2 | Mark every section KEEP, UPDATE, DELETE or ADD. | Brent | work | 0.5 | 0 | R5-M26-t1 |
| R5-M26-t3 | Write the findings: what is unclear, outdated, incomplete, redundant or wrong. | Brent | work | 0.5 | 0 | R5-M26-t2 |
| R5-M26-t4 | Review the findings together and agree what changes; settle disagreements before anyone edits. Bernardo attends. | Brent | meeting | 0.2 | 0 | R5-M26-t3 |
| R5-M26-t5 | List the processes that still need to be defined before they can be written down. | Brent | work | 0.3 | 0 | R5-M26-t4 |

### R5-M27 — Coaching SOP updated and in NotebookLM
**Depends on:** R5-M26

| Task | What gets done | Owner | Type | Work | Wait | Depends on |
|---|---|---|---|---|---|---|
| R5-M27-t1 | Update the coaching SOP: rewrite outdated sections, remove what is obsolete, add missing processes and clarify expectations. | Brent | work | 0.3 | 0 | — |
| R5-M27-t2 | Update the onboarding and kickoff sections of the coaching SOP once the new system exists. | Brent | work | 0.3 | 0 | R5-M27-t1, R5-M8* |
| R5-M27-t3 | Update the training section of the coaching SOP with the SOP on how and why training is structured. | Brent | work | 0.2 | 0 | R5-M27-t1, R5-M14-t4* |
| R5-M27-t4 | Read the new SOP from start to finish for contradictions. | Brent | work | 0.5 | 0 | R5-M27-t2, R5-M27-t3 |
| R5-M27-t5 | Load the new SOP into NotebookLM, replacing what is out of date, and confirm the knowledge base points to the right version. | Brent | work | 0.3 | 0 | R5-M27-t4 |

---

## Execution order per person
Order and dependencies only. The dashboard computes when each of these lands, using both people's capacity across all their Rocks.

### Bernardo
1. **Role definition (R5-M1):** t1, then t2. This unblocks more of the Rock than anything else, so it goes first. Later: t6, approving the agreed definition after Brent's meeting.
2. **Dashboard metrics (R5-M2):** t1, the inventory of where retention and churn data lives. Then t3 and t4 after the metrics meeting, so Brent can validate in t5.
3. **Kickoff chain (R5-M6, R5-M7):** M6-t1 finishes the kickoff presentation builder, then M7-t1 creates the fictional clients, then M7-t2 tests it. M7-t3 hands to Brent, which is what releases the whole SOP and calibration chain. After that M7-t4, t5, t6, and finally t8, the cutover.
4. **Roadmap builder (R5-M5):** t1, the production run with a test client, pilot from Brent's account. Needed before M7-t4 and before the end meso build.
5. **Transfer Looms (R5-M20-t1, R5-M20-t8, R5-M21-t1, R5-M21-t8, R5-M23-t1):** all free of dependencies and all gating Brent's SOP writing. Cheap to do, expensive to delay.
6. **Community meetings (R5-M22-t1, R5-M22-t4):** schedule both with Brent, then t5 prepares the templates and systems.
7. **Shipment dashboard (R5-M12-t1):** three days of build, feeding t3 and t4.
8. **Current onboarding reviewed (R5-M13-t1):** his own review of the current coach onboarding, which feeds the comparison meeting with Brent in t3.
9. **End meso (R5-M17-t1, R5-M17-t3):** his own audit of the current deck and call structure, then the proposal to Brent. Later, M17-t10 approves the finished document.
10. **End meso build (R5-M18):** t1 approves the design, then t2, t3, t4, then t5's wait on the cutover, then t6, t7 if needed, t8 hands it to the coaches.
11. **Head coach dashboard (R5-M4-t1)** after the metrics are defined, and **R5-M14-t7** approving the coach onboarding changes before Mikari starts.
12. **Access (R5-M25-t3)** once Brent has listed what he is missing. **R5-M12-t6** if the first shipment shows problems.

### Brent
1. **Role definition (R5-M1):** t3 merges the lists, t4 marks each responsibility, t5 is the agreement meeting with Bernardo. Everything in projects P6 and P7 waits on this.
2. **Startable immediately in parallel:** the kickoff call audit (R5-M10-t1 onward), the upsell meeting (R5-M11-t1), confirming the shirts arrived (R5-M12-t2), his own coach onboarding review (R5-M13-t2), his own end meso audit (R5-M17-t2), telling the team he is taking the role (R5-M25-t1), and reading the coaching SOP (R5-M26-t1).
3. **Metrics and KPIs:** R5-M2-t2 meeting, R5-M2-t5 validation, then R5-M3-t1, t2, t3 once the role definition and the metrics are both done. R5-M4-t2 confirms the dashboard.
4. **Kickoff standard (R5-M7-t3, R5-M8, R5-M9):** test the builder from his own account, write the competency questionnaire, update the onboarding and kickoff SOP, load it into NotebookLM, then run the calibration call and record who passed. R5-M7-t7 waits for the coaches' mock-call Looms.
5. **Coach onboarding (R5-M13-t3, R5-M14, R5-M15, R5-M16):** the comparison meeting, then the two scoping meetings, the training materials, the training SOP, the rest of the changes and the learning path. Then start Mikari, work her problems as they appear, close the run, and get her a first client.
6. **End meso (R5-M17):** t4 agrees the changes, then t5, t6, t7 in parallel, plus the t8 and t9 meetings. R5-M19-t1 reviews the first produced presentation.
7. **Transfer (R5-M20, R5-M21, R5-M22, R5-M23):** for each responsibility the pattern is the same: write the SOP section, run it once with Bernardo present, correct the section. The two longest waits sit here, in R5-M20-t11 and R5-M23-t5.
8. **SOPs and hand-off (R5-M24, R5-M25, R5-M26, R5-M27):** the head coach SOP draws on the transfer work and closes last. R5-M25-t5 decides what Bernardo stops doing, which gates telling the team who to go to for what. The coaching SOP review and update run their own line, with R5-M27-t2 and t3 waiting on the new onboarding SOP and the training SOP.

## Cut order if capacity slips
**Proposed, not confirmed.** Sprint Commitments marks the cut order as "Proposed, to be confirmed together with every Rock visible side by side." Nothing in this section is settled, and it is tracked as an open decision in the Project Brain.

Proposed order: first the shipment dashboard and first batch (R5-M12), then the end meso automation (R5-M18, R5-M19), keeping the agreed call structure (R5-M17), then the parts of the coaching SOP review beyond the onboarding and kickoff SOP (R5-M26, R5-M27).

Proposed as not cuttable under any circumstance: the role definition (R5-M1), the head coach SOP (R5-M24), running every responsibility once (R5-M20 to R5-M23), pointing everything at Brent (R5-M25), and the kickoff automation (R5-M6, R5-M7).

What IS settled: the Rock itself cannot be cut (see D-002).

## Deferred / post-sprint (do not lose)
No milestone in this Rock is flagged deferred.

Two things the plan routes to a later sprint rather than deferring outright, and they must not be lost:
- **R5-M14-t1:** the coach onboarding changes that are not required before Mikari starts go to the next sprint's list.
- **R5-M15-t4:** closing Mikari's run produces a list of what goes to the next sprint.

Four tasks are contingent and only run if something goes wrong. They keep their estimates so the plan stays honest: R5-M9-t4 (repeat practice with a coach who did not pass), R5-M10-t5 (update the SOP if an audit problem is systemic), R5-M12-t6 (adjust the shipment process after the first batch), R5-M18-t7 (fix what the end meso tests show).
