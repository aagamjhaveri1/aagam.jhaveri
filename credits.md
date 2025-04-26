---
layout: default
title: Credits
section_url: /credits
---

{% if site.data.credits.assets.size > 0 %}
## Assets Used

{% for asset in site.data.credits.assets.images %}
- {{asset.desc}}: [{{ asset.name }}](/assets/img/{{asset.location}}) by [{{ asset.author }}]({{asset.src}})
{% endfor %}
{% endif %}

{% if site.data.credits.people.size > 0 %}
## Support

{% for person in site.data.credits.people %}
- [{{ person.name }}]({{ person.url }}) for {{ person.credit }}
{% endfor %}
{% endif %}

