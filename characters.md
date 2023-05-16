# Characters

<script>
const queryString = window.location.search;
console.log(queryString);
 const urlParams = new URLSearchParams(queryString);
 const characterParam = urlParams.get('character')
 
 </script>


 {% for character in site.characters %}
 
 <div class="character">
 <h3>{{ character.name }} </h3>
 <div class="description">{{ character.description }} </div>

 {% if character.image %}
     <img src="{{ character.image }}" alt="{{ character.name }}" />
   {% endif %}
 
 </div>
 {% endfor %}
 
 
 {% assign url_substring = page.url | split, '/' | last %}
# url: {{ url_substring }}
 
  
 {% assign url_substring = page.url | split, '?' | last %}
# paraterers: {{ url_substring }}
 
 
 {% assign npc =  site.characters | where_exp: "characters", "characters.name == 'Amrik Vanthampur' "%}
# npc.name: {{ npc.name }}
 
 {% assign npc2 = site.characters | where: 'title', include.title | first %}
 
 
 {% assign theproduct = site.characters | where:"name", "Amrik Vanthampur" | first %}
 
 # npc.name2: {{ theproduct.name }}
  # npc.name2: {{ theproduct }}


