# Primary vs Secondary Clarification - Initiative Brief

- [10-10CG Form - product outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/caregivers/10-10CG%20Caregiver%20application%20product-outline.md)
- [Primary vs Secondary - Transition document](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/caregivers/Transition%20hub/In%20progress%20features/Primary%20and%20Secondary%20Caregiver%20selection.md) from April 2022
- [Primary/Secondary Caregiver - Epic](https://app.zenhub.com/workspaces/vsa---10-10-team-5fff0cfd1462b6000e320fc7/issues/department-of-veterans-affairs/va.gov-team/37541)
- [Discovery ticket #35838](https://app.zenhub.com/workspaces/10-10-health-apps-5fff0cfd1462b6000e320fc7/issues/department-of-veterans-affairs/va.gov-team/35838)
- [Research Findings with Feedback on Primary vs Secondary](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/caregivers/1010cg-mvp/Sign-as-a%20Rep-Round3-Oct2021/Usability%20research/research-findings.md#additional-insights)
- Notes from Design story [#22372](https://app.zenhub.com/workspaces/10-10-health-apps-5fff0cfd1462b6000e320fc7/issues/department-of-veterans-affairs/va.gov-team/22372)
>Comment from Shawna
>- One participant explicitly stated that she wanted the questions to be on a single page: "Maybe if there is a way to have primary and secondary together to explain the differences so I know right off the bat what I'm applying for." Another had issues with the placement of the "Learn more" components and thought those components were the actual questions.
>
>Note from the CG program team:
>
>- They have been receiving a higher than usual amount of Secondary CG applications. These are from older Veterans.
>- They feel there is a lack of understanding what a secondary CG is - that it comes with heavy commitments and requirements similar to the primary, such as check-ins, >etc.
>- Lack of understanding of the difference of Primary and Secondary - responsibilities, benefits, etc.
>- Secondary is not just anyone who helps out (such as underage child, etc.)
>- It is unclear whether when applying for secondary, the applicant needs to **reenter** primary CG information
>- Applicants are unclear if they **HAVE** to enter both Primary and Secondary (eg. They see Secondary so they enter one- sometimes same info as Primary)

Historic volume of Primary & Secondary Caregivers submitted
|2022 Month|1 Primary|1 Primary, 1 Secondary|1Primary, 2 Secondaries|1 Secondary|2 Secondaries|Total Applications|Total Primary|Total Secondary|
|------------|------------|------------|------------|------------|------------|------------|------------|------------|
|July|3,999|576|114|37|1|4,727|4,689|843|
|August|4,643|780|141|45|4|5,613|5,564|1,115|
|September|5,775|940|196|46|4|6,961|6,911|1,386|
---

## Problem

Unrelated usability research studies have shown that users are unclear the difference between a Primary and Secondary Caregiver. A big reason for this is that the selection to apply for each of these is separated in the flow. Another reason is that people don't know what the difference between Primary and Secondary is - if there are different requirements (there aren't) and what benefits are different.

OCTO-DE Objectives: This change will help with increasing the accessilibility, reliability and security of Veteran's digital services.  It will also help reduce the time it takes for Veterans to find, use and receive VA services, by making the roles and benefits between the two types of Caregivers clear and easy to understand.

## Outcome Summary

* As a Veteran and Caregiver/s applying for PCAFC, I want to be clear about the difference between a Primary and Secondary Caregiver. I want to know if there are different requirements and what benefits each one receives,  so that we can apply for the correct one.
* Provide clarity between Primary and Secondary Caregiver roles and benefits, reducing duplicate and abandoned applications.

## Desired User Outcomes
* Clear understanding of the Primary and Secondary Caregiver roles and benefits
* Confidence in completing the form accurately
* Trusting that VA processes will provide expected results

## Undesired User Outcomes
* Uncertainty of the difference between Primary and Secondary Caregiver roles and benefits
* Frustration and/or confusion causing application abandonment
* Distrust in VA and its processes

## Desired Business Outcomes
* Reduced duplicate applications
* Reduced application abandonment
* Increased trust and satisfaction

## Undesired Business Outcomes
* no change or increase in duplicate applications
* no change or increased application abandonment
* Distrust in VA and its processes

---
## Measuring Success

### Key Performance Indicators (KPIs)

### Objective: Update the 10-10CG to clarify the roles and benefits of the Primary and Secondary caregivers

#### **Key Result #1:** Reduce drop-off/exit rate for the application

Data source - [Domo Dashboard](https://va-gov.domo.com/page/447193050)

Data source - [Datadog](https://vagov.ddog-gov.com/dashboard/p5g-fys-epz/1010-health-apps?from_ts=1657212129534&to_ts=1657215729534&live=true)

| Product KPI | Baseline | Target | Post-Launch 1 week |Post-Launch 1 month|
|------------- |---------|-------|-------------- |-------------- |
|Application Submissions | TBD  | TBD | TBD|TBD|
|Section Exit rates?? |TBD  | TBD | TBD|TBD|


#### **Key Result #2:** Reduce duplicate applications (Can CG Contact Center (CSP) get us this info?)

| Product KPI | Baseline | Target | Post-Launch 1 week |Post-Launch 1 month|
|------------- |---------|-------|-------------- |-------------- |
|Application duplicates | TBD  | TBD | TBD | TBD |


#### **Key Result #3:** Increased Trust in VA services

Data source - Medalia survey results?
Data source - Contact Center feedback?

| Product KPI | Baseline | Target | Post-Launch 1 week |Post-Launch 1 month|
|------------- |---------|-------|-------------- |-------------- |
|Trust  | TBD  | TBD | TBD | TBD |
---

## Discovery
### Assumptions/Risks

- **Value Risks** (will people use it): 
  - There is a Risk that applicants will still have difficulty determining the difference between the Primary and Secondary Caregiver roles and benefits
- **Usability Risks** (can people figure out how to use it):
  - There is a risk that, due to lack of clarity, applicants may not know how to complete the application accurately
- **[Technical] Feasibility Risks** (can we build it with available tech/data):
  - There is a low risk of technical issues that would be due to this change.  The usual overall VA>gov risks are still applicable, which are focused on service reliability and performance.
- **Organizational Viability Risks/Constraints** (will there be a positive organizational impact):
  - The risk/constraint is that the stakeholders will not have favorable feedback on the changes

### What're you building

In-Scope
- Update content for Primary and Secondary Caregiver roles and benefits

Out of Scope
- Adding questions
- Removing questions

#### Exploratory design
This table includes links to the individual design work products.

| Screens | Links  
| :--- | :--- | 
| Exploratory Mockup designs | [Sketch](https://www.sketch.com/s/5a676881-7aa8-4054-9b6e-34d86ced43d8/p/79BDE8AC-21C9-4FEF-B0FB-DA6E0C3990DD) 
| Future progressive exploratory flow | [Sketch](https://www.sketch.com/s/5a676881-7aa8-4054-9b6e-34d86ced43d8/a/qerZvg2) 
| Future progressive flow exploratory Mockup designs  | [Sketch](https://www.sketch.com/s/5a676881-7aa8-4054-9b6e-34d86ced43d8/p/FDA98FA9-757B-4193-B52F-6C07B035DA59) 


--- 

## Launch Planning
### Collaboration Cycle
> 💡 *Use for any Collab Cycle tracking, questions.*

- Kickoff ticket #..
  - Design Intent
  - Research Review
  - IA Review
  - Midpoint Review
  - Staging Review
  - Privacy & Security
  - Contact Center guide review

### Incident Response Info
- The 1010CG form is currently in production
- We are updating content only. There are no changes to the form's performance, architecture, API enpoints or security.
- 1010CG [Datadog monitoring dashboard](https://app.datadoghq.com/dashboard/8it-wik-f5q/vsa-1010-team)

### Timeline 
- Initiative Kickoff: 
- Discovery: 
- Design: 
- Design Intent: 
- Finalized Design & Midpoint: 
- Usability/Research: 
- Development: 
- Staging: 
- ... 

#### Initiative Launch Dates
- *Target Launch Date*
  - tbd
- *Actual Launch Date* 
  - tbd

---
   
## Screenshots

### Before

Primary Caregiver question with additional info accordion open
- ![image](https://user-images.githubusercontent.com/92328831/194910647-26ace996-bd41-4f1c-a6fc-bd3cb9a24559.png)

Secondary Caregiver question with additional info accordion open
- ![image](https://user-images.githubusercontent.com/92328831/194910771-23cf51cf-1d29-44e8-83c7-f230caac321f.png)


### After

TBD

---

#### Communications
*Where will you discuss this initiative?*

<details>

- Team Name: 10-10 Health Apps team
- GitHub Label(s): 1010 primary/secondary
- Slack channel: #1010-health-apps
- Product POCs: Heather Justice, Mark Fallows

</details>


#### Stakeholders
*What offices/departments are critical to make this initiative successful?*

<details>
  
- Office/Department: OCTO-DE
- Contact(s): Patrick Bateman, Katherine Lawyer, Mark Dewey
 
</details>

---
<sup>1</sup> [VA.gov Analytics - KPI Framework](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/analytics/Analytics%20Playbook/va-gov-platform-analytics-kpi-framework.pdf)\
<sup>2</sup> [SVPG: The Four Big Risks](https://svpg.com/four-big-risks/)

