---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

I guess this is the index
{% for game in site.games %}
  <h2>{{ game.name }}</h2>
  <p>Year: {{ game.year }}</p>
  <p>Genre: {{ game.genre }}</p>
  <p>Language: {{ game.language }}</p>
  <p>Download: {{ game.asset_id }}.zip</p>
{% endfor %}
