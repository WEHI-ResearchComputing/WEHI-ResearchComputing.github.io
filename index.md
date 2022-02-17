## Welcome to the WEHI Research Computing Platform website

The Research Computing Platform is based in the Computational Biology theme.

At Research Computing Platform we are interested in research software engineering and research software support for WEHI researchers. We always appreciate comments and feedback on how we can better support more researchers.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="./{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
