# Characters




 {% for character in site.characters %}
 
 <div class="character">
   {% if character.image %}
       <img class="character-image" src="{{ character.image }}" alt="{{ character.name }}" />
   {% endif %}
  
   <div class="character-info">
       <h3>{{ character.name }}</h3>
       <div class="character-tagline">{{ character.tagline }}</div>
       <div class="description">{{ character.description }} </div>    
    </div>
 </div>
 {% endfor %}
 



