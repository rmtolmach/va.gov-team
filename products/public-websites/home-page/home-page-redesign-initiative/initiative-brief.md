## Home page redesign initiative brief 

[Overview](#overview)

[Problems to solve](#problems-to-solve)

[Desired outcomes](#desired-outcomes)

[Approach](#approach)

[Measuring success](#measuring-success)

[Assumptions and risks](#assumptions-and-risks)

[Summary of changes](#summary-of-changes)
 - [March 2022 iteration](#march-2022-iteration)
 - [Round 2 design iteration](#round-2-design-iteration--october-2022)
 - [Next steps](#next-steps)

[Ongoing efforts](#ongoing-efforts)
- [Cross-team collaboration](cross-team-collaboration)
- [Connection to authenticated experience](#connection-to-authenticated-experience)
- [Discussions with stakeholders](#discussions-with-stakeholders)

[Launch planning](#launch-planning)

- [Collaboration cycle](#collaboration-cycle)

- [Timeline](#timeline) 

[Screenshots](#screenshots)

## Overview
In the nearly three years since the site's launch, the range of VA benefits and programs has grown and evolved, with new valuable offerings. The VA.gov authenticated experience has expanded to include MyVA, MyProfile, eBenefits migration, and soon MyHealthevet integration. 

Veterans have evolved too - from never logging in to understanding that some tasks are possible online _only when logged in_. This redesign initative was undertaken because the VA.gov homepage needs to reflect the evolution of our Veterans and the benefit landscape. 

## Problems to solve

**1. The text-heavy current experience increases cognitive load and discourages engagement.**
- The volume of content causes Veterans to focus on a single area of the homepage, usually the top 4 boxes. 
- Some tasks are easier than others to complete. 
- A few tasks in the top four boxes get most of the traffic.

**2. The row of Veteran portraits acts as a false bottom which negatively affects engagement with content displayed below the images.**

**3. Search and login**
- ~15% of users logged in to VA.gov, which means the majority of users do not benefit from the personalized experience.
- ~ 586K unique searches initiated from the homepage Jan-Jun 2022 - second only to Find a VA Form but still only 12% of all unique searches. 

**4. The current homepage does not meet organizational and stakeholder needs.**
- We need to help Veterans discover changes in products, services, or eligibility that affect them so they can take action.
- We need to empower Veterans to receive information, rather than to actively seek it out (i.e. subscirbe for email updates).
- We need to direct non-Veteran/beneficiary audiences where to go for the information and tasks appropriate to their needs
- The current UX design was optimized for viewability across Desktop and Mobile, limiting the number of links to five in each of the four top task boxes. This limitation has made it difficult to respond to the expanding benefit and program landscape and stakeholder requests. 

## Desired Outcomes

**Desired user outcomes**
- As a Veteran I want to be able to access tools and processes quickly and easily so that I can manage my own VA benefits 
- As a Veteran, caregiver, family member, etc, I want to be able to learn about the different benefits available to me including eligibility etc. so that I can apply to these benefits.
- As a secondary audience to VA.gov (VSO, Member of Congress, News) I need to understand where on VA.gov I should go to manage and learn activities appropriate to my needs 
- Veterans have increased access to self-service tools through an elevated login funnel 

**Undesired User Outcomes**
- Decrease in engagement with the most popular Top Tasks might be concerning, but would have to be viewed in context of overal engagement patterns.
- Search behavior should be monitored for signs that prominent placement of Search in the page is attracting users for use cases that would be better served by some other path/product.

**Desired Business Outcomes**
- Stakeholders can promote and give visibility to new products and services
- More traffic from the home page to the VAntage Point blog
- More logins

## Approach
The redesign was originally planned as [a series of smaller changes](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/design/phased-design-plan.md) but it was decided to go straight to the planned Step 3 design for the first build, given the strong evidence for change and experimental nature of our work. Further refinement will be informed by Veteran research before changes are moved to production.

So that users of assistive technology can participate in usability testing of the new design, the nital iteration will be built as functional code with functional links, header and footer, in a subdomain on staging. Because the page will not receive visitor traffic outside of user testing, no data layer will be applied. See [March 2022 iteration](#march-2022-iteration) for a summary of changes. 

We will use findings from Veteran research, quantitative user data and benefit utilization to inform design iterations before moving the changes to production or replacing the existing homepage. 

Iterations should support the following goals:
- make it easier for Veterans to navigate the page, engage with relevant information and complete their tasks
- increase the use of the authenticated experience
- intuitively empower Veterans to find and take action on less common tasks
- provide and avenue for Veterans to receive updates and information

## Measuring Success

**Key Performance Indicators (KPIs)**
- Increased clickthrough rates
- Decreased time on page before taking action
- Increased login from homepage
- Increased Veteran satisfaction scores
- Increased subscriptions to email updates

**Baseline values**
- [Baseline event data](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/analytics/baseline-event-data.md)
  > includes traffic to the homepage and log-in rates, events on the header, mega menu, top 4 box tasks, benefit hubs/"explore section", VAntage Point navigation, main page buttons and data visualizations
- [Homepage login data](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/analytics/homepage-login.md)

## Assumptions and risks

**Value Risks** (will people use it): 
  - The use of the home page itself is a given.
  - The case for change is very strong, given engagement gaps with the current design.

**Usability Risks** (can people figure out how to use it):
  - It may be unclear that "Search" is searching content on VA.gov. The list of other search tools below complicates what exactly they're searching when they type something into that section.
  - The "Popular" heading may be unclear as to what exactly this list is for. (Popular what?)
  - The "other search tools" may be unclear as to where someone would actually be going when they click on those links, and what information they would find there.
  - There is a lot of copy in the "Browse benefits..." section. Users are likely just scanning the headings and not reading the copy. It could be generally overwhelming and create too much cognitive load to some users and they may ignore the section.

**Feasibility Risks** (can we build it with available tech/data):
  - The idea of creating a “parallel” home page experience seems pretty straightforward but has not been tried before in recent memory. There are potential challenges to our ideas, including Analytics setup and Search API integration. Future CMS integration has not yet been explored for feasibility or level of effort.
  - Changes to the codebase are small and localized. The only external dependency relates to the Search component, but the implementation and functionality will be identical to the search that already exists in the header. 

**Organizational Viability Risks/Constraints** (will there be a positive organizational impact):
  - We may need the support of teams outside of OCTO-DE to get our experiment live on a va.gov subdomain.

## Summary of changes

### March 2022 iteration

<details>
<summary> First build - March 2022 </summary>
 
![First build design](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/images/va-home-page-first-build.png)

</details>

 - A randomized, rotating set of Veteran portraits has been added to the top of the page
 - Sign in/Sign up CTA has elevated visibility and top placement
 - Four top task boxes have been replaced with a data-driven list of links to 5 Veteran-facing pages where actions can be taken 
 - A visible search option which mimics the site search is available, followed by a  list of other search tools not available through Search (such as Yellow Ribbon, Education benefits, Find a VA form, Facility Locator)
 - VAntage blog article appears in prominent location

**Value proposition**
- Veteran portraits humanize VA and remind stakeholders who VA.gov is intended to serve
- By using analytics to determine search tools and task lists, we can ensure optimal use of space
- Delivers simplified, easy to read design 

**Out of scope**
- Initial scope will not include the header and footer as these are shared across VA.gov and developing consensus on their use will be significantly more complicated. 
- The “Other VA resources” section (which contains links to other VA resources such as Choose VA, Resources and Support, VSO websites, VA offices and Programs) is found in the design but not implemented in the testing version as the links are not Veteran-facing. 

This design was validated with usability testing in August 2022 and findings informed Round 2 design iteration.
- [Usability research findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-findings.md)

### Round 2 design iteration | October 2022

<details>
<summary> Round 2 design iteration | October 2022 </summary>
 
 ![Home-R2-D-1_ PROMO-h1](https://user-images.githubusercontent.com/55411834/195213208-f3590773-b6af-49b7-8e13-4ad5d08edaf6.png)

</details>

- Making information on changes to benefits and services more readily available should result in higher engagement with fresh and timely featured content, measured by increases in clickthrough rates
- Adding context and clearer link labels for news promo spotlight	should improve comprehension and engagement Participants in usability research sessions weren't able to easily distinguish news content from ads or information about benefit changes because of context and unclear link language.	Higher engagement with fresh and timely featured content, measured y increases in clickthrough rates
- Changing button from "sign up/sign in" to "create account" only	should increase use of the logged in experience and account creation originating on homepage
- Increased number of links will improved discoverability and findability of information and improved task completion for common tasks and those which are difficult to find by browsing or frequently searched from the homepage
- Changes to "Other search tools"	will improve task completion and Veteran understanding 
- Adding Resources and support link	will improve task completion and result in traffic to Resources and Support page originating from homepage
- Adding email sign up	will provide an avenue to Veterans to receive updates and information 
- addition of Addition of "Welcome to VA.gov H1	will improve experience for those using screenreaders or keyboard navigation by giving context to landing page

### Next steps

1. Conduct Veteran research to identify top tasks, informing the list of "most popular" links which replace the 4 top task boxes in the new iteration
   > Status: Complete - June 2022 | [Unmoderated top task finding](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/public-websites/research/Veteran-tasks/unmoderated/research-findings.md)

2. Validate design changes with Veterans
   > Status: Complete - August 2022 | [Usability research findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-findings.md)

3. Share research findings broadly 
   > Status: Complete. Top task and usability findings have been presented broadly, including to Public Websites, Authenticated Experience and Health Apartment teams. 

4. Continue to refine objectives and key results 
   > Status: Ongoing
   
5. Develop a rubric for delivering menaingful Veteran-facing content 
   > Status: In progress. Initial rubric was used to determine list of links for design iteration, round 2.

6. Design iterations, informed by analytics and research findings 
   > Status: Round 2 complete - [Description of changes](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/design/round-2-design-iteration.md)

7. Validate design changes with Veterans
   > Status: _Planned - October 2022_ | [Round 2 Usability research plan](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/2022-09-redesign-usability-round2/research-plan.md)

8. Present to Web Governance Board and Digital Modernization Council stakeholders
   > Status: _Scheduled for October 20-21, 2022_

9. Share research findings broadly 
   > Status: _Pending_

10. Drupalize homepage content
    > Status: _In progress_


## Ongoing efforts

### Cross-team collaboration
- Tight collaboration/communication/research readouts with relevant teams (Public Websites, Apartment, Auth Experience)

### Connection to authenticated experience
- Explore routed queries - direct Veterans to a deep link rather than the search results page
- Determine expected behavior for logged in users
  - should sign in/sign up CTA still be present? 
  - user flow when My VA becomes the logged in home page (expected Summer 2022)

### Discussions with stakeholders
- June 22, 2022 Review of redesign and research plan with Dave Conlon, Chris Johnston, and Jeff Barnes
- July 12, 2022 [Deep dive presentation](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/VA.gov%20homepage%20deep%20dive%20-%20July%202022.pdf) to Digital Modernization Council
- October 20-21, 2022 Presentations to Digital Modernization Council and Web Governance Board [_link to presentation pending_]
--- 

## Launch Planning
### Collaboration Cycle
> 💡 *Use for any Collab Cycle tracking, questions.*


| Collab cycle milestone |	Date	|	Issue	|	Notes |
---	|	---	|	---	|	---
| | | Epic: [VA.gov Home page redesign #40845](https://github.com/department-of-veterans-affairs/va.gov-team/issues/40845)| |
| Design intent | 03/29/2022 | [CMS-Offices team - VA.gov Home Page #39038](https://github.com/department-of-veterans-affairs/va.gov-team/issues/39038) | |
| Research | 5/2022 - 6/2022| [Epic: Veteran Top Task Research (moderated and unmoderated) #40857](https://github.com/department-of-veterans-affairs/va.gov-team/issues/39038) | [Unmoderated research findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/public-websites/research/Veteran-tasks/unmoderated/research-findings.md) |
| Research | 8/2022 | [Research epic:  VA.gov homepage redesign iteration - usability#46652](https://github.com/department-of-veterans-affairs/va.gov-team/issues/46652) | [Research findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-plan.md](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-findings.md) |
| Research | _planned 10/2022_ | [Epic: Usability of redesigned home page #41578](https://github.com/department-of-veterans-affairs/va.gov-team/issues/39038) | [Research plan]([https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-plan.md](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/2022-09-redesign-usability-round2/research-plan.md) |
| Analytics | _requested 5/2022_ | <ul><li> [Search DOMO #41512](https://github.com/department-of-veterans-affairs/va.gov-team/issues/41512) </li><li> [Content DOMO #41503](https://github.com/department-of-veterans-affairs/va.gov-team/issues/41503) </li></ui>  | <ul><li> Search DOMO / complete </li><li> Content DOMO / pending </li></ui> |
| Accessibility | _requested 6/2022_| [Accessibility spot check review for redesigned VA.gov home page #42860](https://github.com/department-of-veterans-affairs/va.gov-team/issues/42860)| <ul><li> [SCREENREADER: Alt attributes need to be more descriptive #43898](https://app.zenhub.com/workspace/o/department-of-veterans-affairs/va.gov-team/issues/43898) / pending </li><li> [AXE-CORE Change some of the H2s to H3s #9722](https://app.zenhub.com/workspace/o/department-of-veterans-affairs/va.gov-cms/issues/9722) / closed </li><li> [SCREENREADER: No h1 heading on page #9721](https://app.zenhub.com/workspace/o/department-of-veterans-affairs/va.gov-cms/issues/9721) / closed </li></ul>
| Mid-cycle review | 10/21/2022 | [Sitewide Homepage, VA.gov homepage redesign #48041](https://github.com/department-of-veterans-affairs/va.gov-team/issues/48041)

### Timeline 
> *Describe any major milestones for this initiative including organizational, legislative, etc. constraints.*

| Date | Milestone|
|---|---|
| November 11, 2018 | VA.gov launch
| April 2021 | Baseline Wayfinding Research | 
| March 39, 2022 | [Design intent](https://github.com/department-of-veterans-affairs/va.gov-team/issues/39038)|
| June 3, 2022 | Moderated Top Task research/[findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/public-websites/research/Veteran-tasks/moderated/research-findings.md) |
| June 3, 2022 | First build deployed to [Staging](https://staging.va.gov/homepage-test/) |  
| June 2022 | Unmoderated Top Task research/[findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/public-websites/research/Veteran-tasks/unmoderated/research-findings.md)|
| July 22, 2022 | [Deep dive presentation](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/VA.gov%20homepage%20deep%20dive%20-%20July%202022.pdf) to Digital Modernization Council 2022 
| August 2022 | Usability research/[findings](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/redesign-usability/research-findings.md)| 
| September 2022 | Design iteration v2 deployeded to staging
| October 2022 | Usability of redesigned homepage /[plan](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/research/2022-09-redesign-usability-round2/research-plan.md)
| October 2022 | Presentations to Digital Modernization Council and Web Governance Board
| October 2022 | Drupalization of homepage content

---
   
## Screenshots

### Before (Current)
<details>
<summary> VA.gov home page as of 3/1/2022 </summary>

![Current homepage](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/images/va-home-page-current.png)
</details>

### After (Still on VA.gov subdomain)

[Staging url](https://staging.va.gov/homepage-test/)

<details>
<summary> First build - June 2022 </summary>
 
![First build design](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/images/va-home-page-first-build.png)

</details>

<details>
<summary> Round 2 design iteration | October 2022 </summary>
 
 ![Home-R2-D-1_ PROMO-h1](https://user-images.githubusercontent.com/55411834/195213208-f3590773-b6af-49b7-8e13-4ad5d08edaf6.png)

</details>



