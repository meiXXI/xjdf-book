# References

{% assign refs = site.data.references %}
<ul>
{% for ref in refs %}
  <li id="{{ ref.id }}">
    {{ ref.author }} ({{ ref.year }}). <em>{{ ref.title }}</em>. Retrieved from <a href="{{ ref.url }}">{{ ref.url }}</a>
  </li>
{% endfor %}
</ul>