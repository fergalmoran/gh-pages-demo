---
layout: default
---


<h1>{{ site.github.project_tagline }}</h1>

<p>
    This is a demonstration of some of the cool integrations with GitHub that
    GitHub Pages provides.
</p>

<h2>Contributors</h2>
<p>These lovely people have contributed a change to this repository</p>
<ul>
{% for contributor in site.github.contributors %}
  <li>
    <img src="{{ contributor.avatar_url }}" width="32" height="32" /> {{ contributor.login }}
  </li>
{% endfor %}
</ul>

<p>
The code for generating that list is:
</p>

```
{% raw %}
<ul>
{% for contributor in site.github.contributors %}
  <li>
    <img src="{{ contributor.avatar_url }}" width="32" height="32" /> {{ contributor.login }}
  </li>
{% endfor %}
</ul>
{% endraw %}
```


<h2>Repositories</h2>
<p>This is a list of my public repositories</p>
<ul>
{% for repository in site.github.owner_repositories %}
  <li>
    <span>{{ repository.name }} </span>
  </li>
{% endfor %}
</ul>
