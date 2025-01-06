# References

<a id="ref1"></a> Doe, J. (2023). Understanding Markdown References. Retrieved from https://example.com
<a id="ref2"></a> Smith, A. (2021). Markdown for Beginners. Retrieved from https://anotherexample.com

### References

{% assign refs = site.data.references %}
<ul>
{% for ref in refs %}
  <li id="{{ ref.id }}">
    {{ ref.author }} ({{ ref.year }}). <em>{{ ref.title }}</em>. Retrieved from <a href="{{ ref.url }}">{{ ref.url }}</a>
  </li>
{% endfor %}
</ul>