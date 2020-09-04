# Welcome to my dev related website

This is my page

[<img aligh="center" src="https://avatars1.githubusercontent.com/u/16356506?s=460&u=93215fa537fc220158e03c88653ea25fa5f68de5&v=4" alt="github profile photo" width="50px" />][https://github.com/vmarmin]

## Posts

Here are my posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

