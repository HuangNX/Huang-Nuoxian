<h2 id="education" style="margin: 2px 0px -15px;">Educations</h2>

<div class="publications">
<ol class="bibliography">

{% for edu in site.data.education.main %}

<li>

<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative; padding-right: 15px; padding-left: 15px;">
    {% if edu.icon %} 
    <img src="{{ edu.icon }}" class="teaser img-fluid z-depth-1" style="width: 70; height: auto;">
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative; padding-right: 15px; padding-left: 20px;">
    {% if edu.title %} 
    <div class="title"><a href="#">{{ edu.title }}</a></div>
    {% endif %}
    {% if edu.school %} 
    <div class="school">{{ edu.school }}</div>
    {% endif %}
    {% if edu.duration %} 
    <div class="duration">{{ edu.duration }}</div>
    {% endif %}
    {% if edu.location %} 
    <div class="location">{{ edu.location }}</div>
    {% endif %}
    {% if edu.notes %}
    <div class="notes">   
      <strong><i style="color:#e74d3c">{{ edu.notes }}</i></strong>
    </div>
    {% endif %}
  </div>
</div>

</li>
<br>

{% endfor %}

</ol>
</div>
