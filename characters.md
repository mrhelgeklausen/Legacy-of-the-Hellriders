# Characters


 {% for character in site.characters %}
 
 <div class="character">
 <h3>{{ character.name }} </h3>
 <div class="description">{{ character.description }} </div>

 {% if character.image %}
     <img src="{{ character.image }}" />
   {% endif %}
 
 </div>
 {% endfor %}
