---
pageClass: about-page
description: 'The biography and information about me.'
avatar: /profile.jpg
head: 'Zico'
info: 'Final Year Computer Science Undegraduate in National University of Singapore'
interests: 'Interests: Distributed Systems, Low-Level Programming (Rust/C++), Parallel Computing, Computer Games & Graphics.'
socials:
- title: github
  link: https://github.com/zicotjia
- title: linkedin
  link: https://www.linkedin.com/in/zico-tjia/
- title: email
  link: 'mailto:zicotjia@gmail.com'
# actions:
# - text: Projects
#   link: /projects/
# - text: Blog
#   link: https://github.com/zicotjia
# - text: CV
#   link: /article/
footer: Powered by VuePress
---

<AboutCard :frontmatter="$page.frontmatter" >

I attended [National University of Singapore](https://www.comp.nus.edu.sg) to study Computer Science. I have greatly enjoyed Computer Science as a whole. Using my time in college to increase the breadth of my knowledge in many different fields of Computer Science including niches such as Parallel Programming, GPU Programming and Graphic Programming. I have work experience in Backend, iOS Programming and DevOps. 

Some other domains of Computer Science that I am interested in but have little exposures are Game Programming and Low-Level Programming.

I am starting a Final Year dissertation on making improvement to a Volumetric Video Toolkit written in Rust.

</AboutCard>

<style lang="stylus">

.theme-container.about-page .page
  background-color #FFF5E1
  min-height calc(100vh)
  
  .last-updated
    display none

</style>