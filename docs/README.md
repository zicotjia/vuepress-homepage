---
pageClass: home-page
# some data for the components

name: Zico
profile: /profile.jpg

socials:
  - title: github
    icon: "/icons/github.svg"
    link: https://github.com/zicotjia
  - title: linkedin
    icon: "/icons/linkedin-mono.svg"
    link: ttps://www.linkedin.com/in/zico-tjia/

cv: https://en.wikipedia.org/wiki/Harry_Potter
bio: Computer Science Undegraduate in NUS
email: Zicotjia@gmail.com
---

<ProfileSection :frontmatter="$page.frontmatter" />

## About Me

I am currently in my final year studying Computer Science in the National University of Singapore. 

I look forward to working with other Software Engineers to work on products that have impacts on others.

Some topics I am interested are Low-Level Computing (C++/Rust), Parallel Computing, Volumetric Video ans Computer Graphics.

I am starting my Final Year Dissertation on Volumetric Video Toolkit in Rust.

## Education

<EducationCard image="/icons/nus_icon.png">
  **National University of Singapore (2021 - 2025)** <br/>
  Degree: Bachelor of Computing in Computer Science (with Honours*) <br/>
  CAP: 4.29/5.00.

  You can find the course I have taken [here](/courses).

</EducationCard>

## Experiences

<EducationCard image="/experiences/autodesk_icon.jpg">

**Software Engineering Intern Autodesk (Jan 2024 - July 2024)** 

Worked within a team within the Licensing Department to create new microservices to allow client-side software to request for Compliance Check and also to push Telemetry data to other microservices.

- Identified a bug in OpenAPI generated HTTP Client causing HTTP connection to delay termination. Refactored the
HTTP Client and improve on the client to utilise connection pooling in thread-safe manner. This lead to 400%
speedup, allowing SLAs to be met with 75% less machines with significantly lower error rate. Furthermore P99 was reduced from 900ms to 420ms. Verified through performance testing.

- Create a new Terraform repo based on legacy shared Terraform repo that utilise Terraform v1.7.3 over the legacy repo
with Terraform v0.x. Designed a new repository structure to be able to exploit newer Terraform feature while being
compatible with how current services are consuming the Terraform modules. All modules are tested with Terratest.

- Designed Terraform Modules to allow microservices to be routed and accesses through HTTPS. Propagate DNS from Autodesk apex domain DNS table to our microservices DNS server.

- Devised and executed an infrastructure migration plan to achieve domain name change with near zero down time in
service through Terraform applied changes and destruction.

- Updated shared Go Docker Image from v1.17 to v1.22.5. Fixed regression caused by changes in how Go handle Modules and Packages in newer Go version.

- Created Taurus scripts to do load and performance testing for new microservice in Blazemeter.

- Won people's choice award (Highest User vote) in an internal Hackathon by adapting an internal ChatGPT-like platform to provide specialised response for project planning queries. 

</EducationCard>

<EducationCard image="/experiences/zuju_icon.jpg">

**Software Engineering Intern ZujuGP (May 2023 - Sep 2023)** 

Contribute in the development of version 2.X of the application/game "Kickoff by Zuju" for the iOS platform. 

- Developed UI in UiKit for the app.

- Implemented some of the gameplay logic that connects with backend such as notification handler and in-game score/leaderboard update. 

- Automate creation of GitHub branch based on transition of Jira Tickets, Automate movement of Jira tickets based on
creation of PR. Streamlining workflow of iOS team.

- Create Bash Scripts to be run in GitHub Actions to trigger Jira webhook for automation.

- Start initiatives to write unit tests for iOS codebase and refactoring codes to be more testable through dependency inversion.

- Refactor legacy codes to iOS 15 UIKit standard and refactor reusable codes into internal Swift package.

- Collaborate with backend team to fix issues of transitioning Amplify V1 into Amplify V2 due to incompatibility with Terraform.

</EducationCard>

<EducationCard image="/experiences/flux_icon.png">

**Software Development Intern Project Flux (May 2022 - Jun 2022)**

Contributed in creating a javascript web extension that lower data and energy consumption of internet browsing through these features:

- Modify images and videos to download and render on-click.

- Delay loading and rendering of side components of web pages such as navbar, header and footer to wait for user prompt.

- Stop gifs and animations from autoplaying.

</EducationCard>

## Projects

[→ Full list](/projects/)

<ProjectVidCard videoSrc="/projects/Zeggle.mov">

  **Zeggle (2023)**

  A Peggle clone made using pure Swift for iPad.
  Physics engine and Game engine are hand-crafted in pure Swift.
  Ui with SwiftUI.
  Level storage is done with native Swift SQLite.
  Simple Sound engine through calling Apple's Audio ToolKit and MIDI APIs.

  Features:
  - Level Selector
  - Level Designer
  - Multiple Game modes

  This project was for me to try design my own game with zero knowledge in game programming. Also to test my software engineering skills by designing everything by hand, using minimal pre-existing library while learning a new language.
  
  [[GitHub](https://github.com/zicotjia/Zeggle)]

</ProjectVidCard>

<ProjectCard image="/projects/Socmed.jpg">

  **Social Media Prototype (2022)**
  
  A simple social media app similar to Instagram. Frontend is made using React with Typescript. Backend is made with Go. MongoDB is used to store post and user profile data. A authentication system is created in Go with simple password encryption using crypto library.

  Features:
  - Make Post, Like a Post, Comment on Post
  - Follow other Account
  - Guest Account

  This project was for me to learn Full Stack Engineering with Typescript, Go and designing Backend to handle CRUD. Also for me to improve my skills in state management.

  [[GitHub (Frontend)](https://github.com/zicotjia/Social-Media-Project-Frontend-)] [[GitHub (Backend)](https://github.com/zicotjia/Social-Media-Project-Frontend-)] [[Project Link](https://www.google.com)]

</ProjectCard>

## Skills

**Programming Language**

<SkillLogo image="/skills/cpp.png" text="C++"/>
<SkillLogo image="/skills/rust.png" text="Rust"/>
<SkillLogo image="/skills/golang.png" text="Go"/>
<SkillLogo image="/skills/java.png" text="Java"/>
<SkillLogo image="/skills/swift.png" text="Swift"/>
<SkillLogo image="/skills/typeScript.png" text="TypeScript"/>
<SkillLogo image="/skills/python.png" text="Python"/>

&nbsp;

**Scripting Language**

<SkillLogo image="/skills/python.png" text="Python"/>
<SkillLogo image="/skills/bash.png" text="Bash"/>

&nbsp;

**Database**

<SkillLogo image="/skills/postgreSQL.png" text="PostgreSQL"/>
<SkillLogo image="/skills/mongoDB.png" text="MongoDB"/>
<SkillLogo image="/skills/dynamoDB.png" text="AWS DynamoDB"/>
<SkillLogo image="/skills/S3.png" text="AWS S3"/>

&nbsp;

**Infrastructure**

<SkillLogo image="/skills/terraform.png" text="Terraform"/>

&nbsp;

**Other AWS Cloud Stacks**

<SkillLogo image="/skills/route53.png" text="Route 53"/>
<SkillLogo image="/skills/acm.png" text="ACM"/>
<SkillLogo image="/skills/elb.svg" text="ELB"/>
<SkillLogo image="/skills/ecs.png" text="ECS"/>
<SkillLogo image="/skills/ecr.png" text="ECR"/>
<SkillLogo image="/skills/ec2.png" text="EC2"/>
<SkillLogo image="/skills/sqs.png" text="SQS"/>
<SkillLogo image="/skills/lambda.png" text="Lambda"/>

**Graphic Programming**

<SkillLogo image="/skills/openGL.png" text="OpenGL"/>

**GPU Programming**

<SkillLogo image="/skills/nvidia.png" text="CUDA"/>

**Asynchronous or Concurrency API**

<SkillLogo image="/skills/openMP.png" text="openMP"/>
<SkillLogo image="/skills/openMPI.png" text="openMPI"/>
<SkillLogo image="/skills/tokio.png" text="Tokio (Rust)"/>

**Frontend Framework**

<SkillLogo image="/skills/react.png" text="React"/>
<SkillLogo image="/skills/vue.png" text="Vue"/>
<SkillLogo image="/skills/uiKit.png" text="UiKit"/>
<SkillLogo image="/skills/swiftUi.png" text="SwiftUI"/>






## Awards

- School Of Computing Dean's List AY21-22 Semester 2. [(Link)](https://credentials.nus.edu.sg/42e40ee9-3cf1-439b-8fa8-b8d01075e392)
- ASEAN Undergraduate Merit Scholarship.
- Various Mathematics Olympiad awards in national level.

## Certification

- Certification Of Distinction (Database Systems Focus Area). [(Link)](https://credentials.nus.edu.sg/31bfa54e-4cfa-488c-9de4-bf9cb470bb3a)
- AWS Solution Architect Associate (SAA-CO3). [(Link)](https://www.credly.com/users/zico/)


<!-- Custom style for this page -->

<style lang="stylus">

.text-with-logo {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.text-content {
  flex: 1;
}

.logo-content {
  margin-right: 20px;
}

.logo {
  max-width: 50px !important; /* Adjust as needed */
  height: auto;
}

.theme-container.home-page .page
  font-size 14px
  font-family "lucida grande", "lucida sans unicode", lucida, "Helvetica Neue", Helvetica, Arial, sans-serif;
  p
    margin 0 0 0.5rem
  p, ul, ol
    line-height normal
  a
    font-weight normal
  .theme-default-content:not(.custom) > h2
    margin-bottom 0.5rem
  .theme-default-content:not(.custom) > h2:first-child + p
    margin-top 0.5rem
  .theme-default-content:not(.custom) > h3
    padding-top 4rem

  /* Override */
  .md-card
    margin-top 0.5em
    .card-image
      padding 0.2rem
      img
        max-width 250px
        max-height 500px
    .card-content p
      -webkit-margin-after 0.2em

  /* Override */
  .md-card
    margin-top 0.5em
    .card-image
      padding 0.2rem
      video
        max-width 250px
        max-height 500px
    .card-content p
      -webkit-margin-after 0.2em

@media (max-width: 419px)
  .theme-container.home-page .page
    p, ul, ol
      line-height 1.5

    .md-card
      .card-image
        img 
          width 100%
          max-width 400px

</style>
