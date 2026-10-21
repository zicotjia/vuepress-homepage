---
pageClass: projects-page
---

# Work

Here are some of my projects and other work.

## Projects

<ProjectVidCard image="/projects/Ravening.jpg">

  **Ravening (2025)**

  Ravening is a loot-and-scoot game featuring an isometric camera angle, procedurally generated dungeons, and a variety of entities.   The goal is to amass wealth by finding treasure and survive until you find a merchant to sell your loot.

  Features:
  - Procedurally generated levels
  - Multiple enemy types
  - Power-ups and upgrades

  This project was created for the CS3247 Game Development course. I worked on:

  - Level generation blueprint with entities and loot spawning
  - Enemy design and animation (designed and rigged in Blender, then animated in UE5)
  - Loot table blueprint
  - In-game UI elements

  [[GitHub](https://github.com/zicotjia/Ravening)]

</ProjectVidCard>

<ProjectVidCard videoSrc="/projects/Zeggle.mov">

  **Zeggle (2023)**

  A Peggle clone made entirely in Swift for iPad.
  The physics and game engines were handcrafted in Swift.
  The UI was built with SwiftUI.
  Levels are stored in SQLite using Swift's native support.
  A simple sound engine uses Apple's AudioToolbox and MIDI APIs.

  Features:
  - Level selector
  - Level designer
  - Multiple game modes

  I created this project to try designing my own game with no prior game programming experience. It also gave me a chance to test my software engineering skills by designing everything by hand, using as few pre-existing libraries as possible while learning a new language.
  
  [[GitHub](https://github.com/zicotjia/Zeggle)]

</ProjectVidCard>

<ProjectCard image="/projects/Socmed.jpg">

  **Social Media Prototype (2022)**
  
  A simple social media app similar to Instagram. The frontend is built with React and TypeScript, while the backend is written in Go. MongoDB stores posts and user profile data. The app also includes an authentication system written in Go, with basic password encryption using the crypto library.

  Features:
  - Make, like, and comment on posts
  - Follow other accounts
  - Guest account

  I created this project to learn full-stack engineering with TypeScript and Go, and to design a backend that handles CRUD operations. It also helped me improve my state management skills.

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
