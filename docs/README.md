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

- **National University of Singapore (2021 - 2025)** <br/>
Degree: Bachelor of Computing in Computer Science (with Honours*) <br/>
CAP: 4.30/5.00



## Projects


[→ Full list](/projects/)

<ProjectCard image="/projects/Zeggle.jpg">

  **Zeggle**

  A Peggle clone made using pure Swift.
  Physics engine and Game engine are hand-crafted in pure Swift.
  Ui with SwiftUI.
  Level storage is done with native Swift SQLite.
  Simple Sound engine through calling Apple's Audio ToolKit and MIDI APIs.

  Features:
  - Level Selector
  - Level Designer
  - Multiple Game modes
  
  [[GitHub](https://github.com/zicotjia/Zeggle)] [[Demo Video](https://arxiv.org)]

</ProjectCard>

<ProjectCard image="/projects/Socmed.jpg">

  **Harry Potter and the Deathly Hallows**
  
  In the epilogue of Deathly Hallows, which is set 19 years after Voldemort's death, Harry and Ginny are a couple and have three children: James Sirius Potter, who has already been at Hogwarts for at least one year, Albus Severus Potter, who is starting his first year there, and Lily Luna Potter, who is two years away from her first year at the school.

  [[Link](https://www.google.com)]

</ProjectCard>


## Awards & Honors

### Contests

- First place in **The Hogwarts House Cup**


<!-- Custom style for this page -->

<style lang="stylus">

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
        max-width 300px
        max-height 300px
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
