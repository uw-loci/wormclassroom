---
layout: default
---



<div id = "indexbody" class="wrapper" style="background-color: #ffffff;">
   <div class="container">
      <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 hidden-xs">
         <div id="carousel-299058" class="carousel slide">
            <div class="carousel-inner">
               <div class="item">
                  <img  class="img-responsive" src="images/slider1.jpg" alt="thumb">
                  <div class="carousel-caption">  
                  </div>
               </div>
               <div class="item active"> <img class="img-responsive" src="images/slider2.jpg" alt="thumb">
               </div>
               <div class="item">
                  <img class="img-responsive" src="images/slider3.jpg" alt="thumb">
                  <div class="carousel-caption"> 
                  </div>
               </div>
               <div class="item">
                  <img class="img-responsive" src="images/slider4.jpg" alt="thumb">
                  <div class="carousel-caption"> 
                  </div>
               </div>
            </div>
            <a class="left carousel-control" href="#carousel-299058" data-slide="prev"><span class="icon-prev"></span></a> <a class="right carousel-control" href="#carousel-299058" data-slide="next"><span class="icon-next"></span></a>
         </div>
      </div>
   </div>
   <div class="container" id="projects">
      <div class="col-md-12 project-container" style="max-height: {{MaxHeightForProjectsContainer}};" >
         {{#projects}}
         <div class="col-lg-4 col-md-4 col-sm-6 col-xs-6 project-item ">
            <a id ="{{heading}}" href="{{url}}" onclick="passProjectName(this.id)">
               <div class="thumbnail">
                  <img src="images/{{img_src}}" alt="Thumbnail Image 1" class="img-responsive" >
                  <div class="caption">
                     <h4>{{heading}}</h4>
                     <p>{{short_des}}</p>
                  </div>
            </a>
            </div>
         </div>
         {{/projects}}
         <div class="col-lg-4 col-md-4 col-sm-6 col-xs-6 project-item ">
            <a id ="{{events.0.heading}}">
               <div class="thumbnail">
                  <div class="caption">
                     <h4>{{events.0.heading}}</h4>
                     <p>{{events.0.date_time}}</p>
                     <p>{{events.0.location}}</p>
                     <p>{{events.0.short_des}}</p>
                  </div>
            </a>
            </div>
         </div>
      </div>
   </div>
</div>
<!-- 
  <script type="text/javascript">
    function passProjectName(pName) {
      console.log(pName);
      localStorage.setItem('myStorage', JSON.stringify(pName));
    }
    $(function () {
      $.getJSON('data.json',function(data){
        data.projects.sort(function (a, b) {return Math.random() - 0.5;});
        data.projects=data.projects.slice(0,5);
        var template  = $('#indextpl').html();
        var html =  Mustache.to_html(template,  data);
        $('#indexbody').html(html);
      });
    });
  </script>
 -->