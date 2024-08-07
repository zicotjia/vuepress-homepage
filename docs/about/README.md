---
pageClass: about-page
description: 'The biography and information about me.'
avatar: /profile.jpg
head: 'Zico'
info: 'Final Year Computer Science Undegraduate in National University of Singapore'
interests: 'Interests: Distributed Systems, Low-Level Programming (Rust/C++), Parallel Computing, Computer Graphics.'
socials:
- title: github
  link: https://github.com/zicotjia
- title: linkedin
  link: https://www.linkedin.com/in/zico-tjia/
- title: email
  link: 'mailto:zicotjia[at]gmail.com'
actions:
- text: Projects
  link: /projects/
- text: Blog
  link: https://github.com/mtobeiyf
- text: CV
  link: /article/
footer: Made with ♥ by Fing. Powered by VuePress
---

<AboutCard :frontmatter="$page.frontmatter" >

I attended [Hogwarts School of Witchcraft and Wizardry](https://en.wikipedia.org/wiki/Hogwarts) to study witchcraft, supervised by **Dumbledore** and other professors. I'm trying my best to battle with Lord Voldemort, the evil Wizard that we all fear. My research area includes Defence Against the Dark Arts and other magic. :dizzy:

</AboutCard>

<style lang="stylus">

.theme-container.about-page .page
  background-color #FFF5E1
  min-height calc(100vh)
  
  .last-updated
    display none

</style>