---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{{ site.games }}

{% for game in site.games %}
{% if game.top_pick %}
One game
  <h2>{{ game.name }}</h2>
  ```yaml
  Year: {{ game.year }}
  Genre: {{ game.genre }}
  Language: {{ game.language }}
  Download: {{ game.asset_id }}.zip
  ```
{% endif %}
{% endfor %}

I guess this is the index innit