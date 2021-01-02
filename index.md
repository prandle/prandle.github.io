{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %}

{% for page in site.pages %}
  <article>
    <h2>
      <a href="{{ page.url }}">
        {{ page.title }}
      </a>
    </h2>
  </article>
{% endfor %}
