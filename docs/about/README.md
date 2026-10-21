---
pageClass: about-page
description: 'A short biography and information about me.'
avatar: /profile.jpg
head: 'Zico'
info: 'Final-year Computer Science undergraduate at the National University of Singapore'
interests: 'Interests: Distributed systems, low-level programming (Rust/C++), parallel computing, computer games, and graphics.'
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

I studied Computer Science at the [National University of Singapore](https://www.comp.nus.edu.sg), where I have greatly enjoyed the subject as a whole. So far, I have broadened my knowledge across many areas of computer science, including niche fields such as parallel programming, GPU programming, and graphics programming. I have work experience in backend engineering, iOS programming, and DevOps.

I am also interested in game programming and Rust.


</AboutCard>

<style lang="stylus">

.theme-container.about-page .page
  background-color #FFF5E1
  min-height calc(100vh)
  
  .last-updated
    display none

</style>