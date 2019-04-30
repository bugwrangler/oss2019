---
title        : Dealing with Security Findings in the Enterprise
type         : working-session
track        : Security Automation
topics       : ["SDL"]
technology   : Dependency Check, FindSecBugs, ZAP, Defect Dojo, Selenium, Jira
categories   :                      # GDPR, Juice Shop, etc.
featured     : yes                  # review with summit team "yes"
when_day     : Tue
when_time    : PM-1, PM-2
room_layout  :                    #
room_id      : room-5
session_slack: 
status       : review-content              # draft, review-content, done
organizers   : Claudio Camerino
participants : 
description  : How to deal with the security findings generated by automated security testing tools

---

Security testing is vital to validate the correct implementation of controls and that security requirements, gathered during the design phase, have been properly implemented. To scale securty testing to  often huyndreds of different software products, many organisations have now started automating static testing as part of the build process or by driving runtime testing through the QA process. 

## Why

Thanks to the proliferation of autonated security scanning tools we are generating a phenomenal amount of security findings. As part of the this session we tackle the following goals.

1. Visibility - Can't secure what you don't see. Why is important to test early in the SDL and map tests to business flows.
2. Accountability - Creating a feedback loop. Why is important to flag findings to their respective owners.
3. Noise Removal - Accuracy drives credibility. Developers are more likely to triage and action reputable findings, starting with tigther scan policies.
4. Scalability - Running tools and managing processes manually is not an aption when dealing with hundreds of products. How to scale generation, collection and triaging of security findings.

## What

- What tools and test types should be used to generate security findings? What's a good toolset to start from?
- The automated testing workflow: generate, collect, consolidate, sanitise, allocate, triage, accept/reject/fix and track security findings.
- Reccomended security testing approaches for:
-- Srontend and backend applications
-- Static vs runtime
- AppSec testing integration with QA - user stories vs abuse cases and how to leverage QA processes to drive ZAP.
- Integration with Jira - how to raise and populate SEC type tickets and track their lifecycle.
- Continous improvement - is it possible to tune scan policies as part of the triage process?

## Outcomes
- Generates/amend scripts to automate generation, collection and allocation of findings.
- Define ruleset for programmatic removal of noise (i.e. duplicates, transitive dependencies and easy to spot FPs)
- Adapt/hack OSS tools like ZAP, findsecbugs, dependency check and Defect Dojo for enterprise level automation.
- Define roles and responsibilities for these activities based on common industry roles (QA, Del Svcs, Engineering etc.)
- Generation of ZAP scan policies and SAST quality profiles (for Sonarqube) for common technologies and frameworks.
- Build a POC for the system.

## Who

The target audience for this Working Session is:

 - Developers
 - Security professionals
 - DevSecOps
 - Security champions
 - AppSec leaders

## Working materials

Here are the current materials for this session:

- [The Security Development Lifecycle](https://www.owasp.org/images/7/78/OWASP_AppSec_Research_2010_Keynote_2_by_Lipner.pdf)
- [SDL in Practice](https://www.owasp.org/images/4/45/SDL_in_practice.pdf)
- [Defect Dojo](https://github.com/DefectDojo/django-DefectDojo)
- [OWASP ZAP](https://github.com/zaproxy/zaproxy)
- [Dependency Check](https://github.com/jeremylong/DependencyCheck)
- [Selenium](https://www.seleniumhq.org/projects/webdriver)

## Previous Summit Working Session