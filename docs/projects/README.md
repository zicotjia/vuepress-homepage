---
pageClass: projects-page
---

# Work

Here are some of my projects and other works

## Projects

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

## Publications
*TBA

<style lang="stylus">

.projects-page
  background-color #FFF5E1

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

</style>

