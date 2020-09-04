# Welcome to my dev website!

[<img align="center" src="https://avatars1.githubusercontent.com/u/16356506?s=460&u=93215fa537fc220158e03c88653ea25fa5f68de5&v=4" alt="github profile photo" width="50px" />][github]

Hi there! My name's Valentin and I'm a Software / Test developer.

* From france 🇫🇷
* I’m currently living in Montréal, CA 📍🇨🇦
* I’m currently learning Django 🌱
* 2020 Goals: learn front end development 🥅
* Fun fact: I am a photography and travel enthusiast 📷🌎

<br />

## Connect with me

[<img align="left" alt="vmarmin | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
[<img align="left" alt="www.talesofwanders.com" width="22px" src="https://raw.githubusercontent.com/iconic/open-iconic/master/svg/globe.svg" />][website]
[<img align="left" alt="vmarmin | Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" />][twitter]
[<img align="left" alt="vmarmin | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]

<br />


## Languages and Tools

[<img align="left" alt="neovim" height="26px" src="https://cdn.svgporn.com/logos/neovim.svg" />][linkedin]
[<img align="left" alt="vim" height="26px" src="https://cdn.svgporn.com/logos/vim.svg" />][linkedin]
[<img align="left" alt="python" height="26px" src="https://cdn.svgporn.com/logos/python.svg" />][linkedin]
[<img align="left" alt="pytest" height="26px" src="https://camo.githubusercontent.com/c6c27ccbb35cbbc24cf1431b5e0e084f73e07373/68747470733a2f2f646f63732e7079746573742e6f72672f656e2f737461626c652f5f7374617469632f707974657374312e706e67" />][linkedin]
[<img align="left" alt="c" height="26px" src="https://cdn.svgporn.com/logos/c.svg" />][linkedin]
[<img align="left" alt="Visual Studio Code" height="26px" src="https://cdn.svgporn.com/logos/visual-studio-code.svg" />][linkedin]
[<img align="left" alt="Git" height="26px" src="https://cdn.svgporn.com/logos/git-icon.svg" />][linkedin]
[<img align="left" alt="GitHub" height="26px" src="https://cdn.svgporn.com/logos/github-icon.svg" />][linkedin]
[<img align="left" alt="terminal" height="26px" src="https://cdn.svgporn.com/logos/terminal.svg" />][linkedin]

<br />

## OS and distribution

[<img align="left" alt="linux" height="26px" src="https://cdn.svgporn.com/logos/linux-tux.svg" />](https://www.linux.org/)
[<img align="left" alt="macos" height="26px" src="https://cdn.svgporn.com/logos/macOS.svg" />](https://www.apple.com/macos/catalina/)
[<img align="left" alt="windows" height="26px" src="https://cdn.svgporn.com/logos/microsoft-windows.svg" />](https://www.microsoft.com/en-us/windows)
[<img align="left" alt="ubuntu" height="26px" src="https://cdn.svgporn.com/logos/ubuntu.svg" />](https://ubuntu.com/)
[<img align="left" alt="manjaro" height="26px" src="https://manjaro.org/img/logo.svg" />](https://manjaro.org/)
[<img align="left" alt="raspberry pi" height="26px" src="https://cdn.svgporn.com/logos/raspberry-pi.svg" />](https://www.raspberrypi.org/)

<br />
<br />

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
<p>
    {% for post in tag[1] %}
    <a href="{{ post.url }}">{{ post.title }}</a><br/>
    {% endfor %}
</p>
{% endfor %}

[website]: https://talesofwanders.com
[github]: https://github.com/vmarmin
[twitter]: https://twitter.com/vmarmin
[youtube]: https://youtube.com/vmarmin
[instagram]: https://instagram.com/valentin.mrmn
[linkedin]: https://linkedin.com/in/valentin-marmin
