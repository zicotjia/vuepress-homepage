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

## Education & Experiences

<EducationCard image="/icons/nus_icon.png">
  - **National University of Singapore (2021 - 2025)** <br/>
  Degree: Bachelor of Computing in Computer Science (with Honours*) <br/>
  CAP: 4.30/5.00

</EducationCard>

## Projects


[→ Full list](/projects/)

<ProjectVidCard videoSrc="/projects/Zeggle.mov">

  **Zeggle**

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

  **Social Media**
  
  A simple social media app similar to Instagram. Frontend is made using React with Typescript. Backend is made with Go. MongoDB is used to store post and user profile data. A authentication system is created in Go with simple password encryption using crypto library.

  Features:
  - Make Post, Like a Post, Comment on Post
  - Follow other Account
  - Guest Account

  This project was for me to learn Full Stack Engineering with Typescript, Go and designing Backend to handle CRUD. Also for me to improve my skills in state management.

  [[GitHub (Frontend)](https://github.com/zicotjia/Social-Media-Project-Frontend-)] [[GitHub (Backend)](https://github.com/zicotjia/Social-Media-Project-Frontend-)] [[Project Link](https://www.google.com)]

</ProjectCard>


## Awards & Honors

### Contests

- First place in **The Hogwarts House Cup**


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
