---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
![Suomipelit Foundation](assets/logo_trans_big.png)

The purpose of this page is to preserve Finnish PC games from roughly 1987 -> 2004. This was the original `golden age` of Finnish indie game development. The resulting idiosyncratic games were nicknamed `Suomipelit` and they quickly gained a cult status.

-

## Notable Genres 
### (Mostly winter) Sports
Ski Jump International 3, ProPilkki, Slicks'n'Slide
### Co-op Shooters
Liero, Wings, Tapan Kaikki 2
### Parody
Beerworm, SpurguX


All the games are freeware or shareware.
Over half of them are in English.
Most of them require DosBox and a Windows 95 Virtual Machine (instructions coming later) to run.

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