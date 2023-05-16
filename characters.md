# Characters


 {% for character in site.characters %}
 
 <div class="character">
 <h3>{{ character.name }} </h3>
 <div class="description">{{ character.description }} </div>

 {% if character.image %}
     <img src="{{ character.image }}" alt="{{ character.name }}" />
   {% endif %}
 
 </div>
 {% endfor %}
 
 
 {% assign npc =  site.characters | where_exp: "item", "item.name == 'Amrik Vanthampur' "%}
 # npc.name
 
 {% assign npc2 = site.characters | where: 'title', include.title | first %}
