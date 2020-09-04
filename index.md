# Welcome to my dev related website

This is my page

[<img align="center" src="https://avatars1.githubusercontent.com/u/16356506?s=460&u=93215fa537fc220158e03c88653ea25fa5f68de5&v=4" alt="github profile photo" width="50px" />][github]

## Posts

Here are my posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## Tags

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

## Categproes

{% for cat in site.categories %}
  <h3>{{ cat[0] }}</h3>
  <ul>
    {% for post in cat[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

[website]: https://talesofwanders.com
[github]: https://github.com/vmarmin
[twitter]: https://twitter.com/vmarmin
[youtube]: https://youtube.com/vmarmin
[instagram]: https://instagram.com/valentin.mrmn
[linkedin]: https://linkedin.com/in/valentin-marmin
