<ul>
  {% for post in site.posts %}
    <p>
    <li>
      {% if post.external_url %}
        {{ post.date | date: "%Y-%m-%d" }} <a href="{{ post.external_url }}" target="_blank">{{ post.title }} (link)</a>
      {% else %}
        {{ post.date | date: "%Y-%m-%d" }} <a href="{{ post.url }}">{{ post.title }}</a>
      {% endif %}
      <br>
    </li>
    </p>
  {% endfor %}
</ul>
