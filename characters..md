# Characters


 {% for character in site.characters %}
 - {{ character.name }}, role: {{ character.description }}
 - {% if character.image %}
     {{ character.image }}
   {% endif %}
 {% endfor %}
