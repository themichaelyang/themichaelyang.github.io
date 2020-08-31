---
layout: default
---

Howdy! I’m Michael, a software engineer at Stripe. 

I studied CS and Math at NYU. Previously, I was a hackNY Fellow at BuzzFeed. I have also worked at Yelp, the Collaborative Social Systems Lab, and Mapkin. Check out some of my projects below, or read my blog.

You can contact me at yangmichael@nyu.edu. I’m also on Github as @themichaelyang.

<div class="Home__Featured">
  <ul class="Home__Projects">
    <h1 class="Home__Heading">Projects</h1>
    {% assign projects = site.projects | reverse %}
    {% for project in projects %}
      <li>
        <a class="project-name" href="{{ project.link }}">{{ project.name }}</a>
        <p class="project-description">{{ project.description }}</p>
      </li>
      {% endfor %}
  </ul>

  <ul class="Home__Posts">
    <h1 class="Home__Heading">Latest posts</h1>
    {% for post in site.posts limit:3%}
      <li>
        <a class="post-name" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <p class="post-description">{{ post.description }}</p>
      </li>
    {% endfor %}
    <p><em>Read more from the <a href='/blog'>blog</a></em>    ➡️</p>
  </ul>
<div>
