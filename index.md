# Welcome to my website!

Here, you can find information about me, projects I have done, and my résumé.

[About Me](about.md)

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date }}</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>