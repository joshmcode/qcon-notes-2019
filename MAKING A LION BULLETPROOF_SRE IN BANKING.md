# Making a Lion Bulletproof
Robin van Zijll & Janna Brummel

## Introduction
Mobile banking serves 4.5 million customers (100+ TPS).

Availability requirements from regulators: 
Internet Banking = 99.77% 
Mobile is even more stringent

Customer expectations is: 
99.63% and mobile is 99.78%

## SRE
> What happens when you have a software engineer work on operations. - Ben Traynor for Google. 

## The ING Organization
- Organized into "tribes"
- 1700 engineers across 340 squads. 
- They try to avoid the "tribe" dangers by being horizontal on their teams via use of squads inside of a engineering tribe. 

### The Team
- 7 engineers (4 devs, 3 ops)
- 2 more joining soon
- 1 product owner
- 1 chapter lead

They tend to stay. Lots of stability. 

### Hiring
- Grow incrementally, not all at once. 
- Heavy focus on non-technical skills
- Someone who is passionate about reliability, problems, DevOps, and open source. 
- OK with failure
- Insensitive to hierarchy
- Willing to teach and advise engineers about reliability
- Experienced in on-call duties and 1+ languages in our stack. 
- Still excited to work with us after meeting half our team

### How they structured their team
- Service ownership is with product engineering. They partner with team. 
 
 TODO: Read the SRE book by O'Reilly (2016)

 ## Time Spent
 - 80% of time is spent  
 - Not on-call for product engineering (what does this mean?)
 - Prometheus workshops

 ## Principles
 - Work with industry standards
 - Work with open source products and practices
 - Automate toil wherever and whenever we can

 ## Technology
 80% software engineering

* Mean time to repair was too long. Wasted time finding incident owners. 
* Lack of insight into application health for teams
* High-level of technology diversity makes implementing monitoring difficult

### How does the Reliability Toolkit work
- Centered around Prometheus

```
                        Grafana
                        /
Applications <- Prometheus  -> Alert Manager -> Communication
                    \\
                    Model Builder
```                  

Idea: Send our alerts to Mattermost with tags

### How do they provision the Toolkit?

### Pipelines
- Before, teams would own and use a full pipeline
    - Version control
    - Combine configurations (Jinja)
    - Build
    - Publish
    - Deploy
    - Reliability toolkit
- Now, they only own and update config

### Increasing and improving usage of Reliability Toolkit
- Include client libraries in engineering frameworks
- Ensure a good feedback loop either in person or in tooling
- Educate others during onboarding and workshops
- Template team dashboards and make other dashboards accessible to all
