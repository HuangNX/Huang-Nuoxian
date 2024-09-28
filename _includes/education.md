<h2 id="education" style="margin: 2px 0px -15px;">Educations</h2>

<div class="publications">
<ol class="bibliography">

{% for edu in site.data.education.main %}

<li style="margin-bottom: 10px;">

<div class="pub-row" style="display: flex; align-items: flex-start;">
  <div class="col-sm-3 abbr" style="position: relative; padding-right: 15px; padding-left: 15px; padding-top: 10px">
    {% if edu.icon %} 
    <img src="{{ edu.icon }}" style="width: 70px; height: auto;">
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative; padding-right: 15px; padding-left: 20px;">
    <div style="display: flex; justify-content: space-between; width: 100%;">
      {% if edu.title %} 
      <div class="title"><a href="#">{{ edu.title }}</a></div>
      {% endif %}
      {% if edu.duration %} 
      <div class="duration" style="color: gray;">{{ edu.duration }}</div>
      {% endif %}
    </div>
    {% if edu.school %} 
    <div class="school">{{ edu.school }}</div>
    {% endif %}
    {% if edu.location %} 
    <div class="location">{{ edu.location }}</div>
    {% endif %}
    {% if edu.notes %}
    <div class="notes">   
      {{ edu.notes | safe }}
    </div>
    {% endif %}
  </div>
</div>

</li>
<br>

{% endfor %}

</ol>
</div>
