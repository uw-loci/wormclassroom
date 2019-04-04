---
layout: default
permalink: /instructions_catalog
---

## Contents
{% for page in site.pages %}
  {% if page.category == 'dungeonopoly1' %}  
* [{{ page.title }}](#{{ page.url }})
  {% endif %}
  {% if page.category == 'dungeonopoly2' %}  
    * [{{ page.title }}](#{{ page.url }})
  {% endif %}
{% endfor %}

{% for page in site.pages %}
  {% if page.category == 'dungeonopoly1' %}  
<a name="{{ page.url }}"></a>
* * *
## {{ page.title }}
{{ page.content }}
  {% endif %}
  {% if page.category == 'dungeonopoly2' %}  
<a name="{{ page.url }}"></a>
* * *
### {{ page.title }}
{{ page.excerpt }}
  {% endif %}
{% endfor %}

CTR TODO


<div id="projectsbody" class="wrapper" style="background-color: #ffffff;">
    <div class="container">
      <div class="col-md-12" id="project_desc"> 
        {{#projects}}
        <table cellspacing="2" cellpadding="2" border="0" class="project_table">
          <tbody>
            <tr>
              <td style="width: 7.5em;margin: 5px 15px 0 15px;float: left;"><img src="images/{{img_src}}" alt="Thumbnail 1" width="98" height="98"></td>
              <td><a id ="{{heading}}" href="{{url}}" onclick="passProjectName(this.id)"> {{heading}}</a><p></p>
                <p>{{medium_desc}}</p>
                <hr>
              </td>
            </tr>
          </tbody>
        </table>
        {{/projects}}
      </div>
    </div>
  </div>

<!--  <script type="text/javascript">
    function passProjectName(pName) {
      console.log(pName);
      localStorage.setItem('myStorage', JSON.stringify(pName));
    }
    $(function () {
      $.getJSON('data.json',function(data){
        var template  = $('#projectstpl').html();
        var html =  Mustache.to_html(template,  data);
        $('#projectsbody').html(html);
      });
    });
  </script> -->
