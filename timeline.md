

<section id="timeline">
<h3>Beta Timeline</h3>
<div class="colour_key">
  <p class="colour_key_heading">KEY</p>
  <p><span style="background-color: #f5c44b">&nbsp;&nbsp;&nbsp;&nbsp;</span> Accessibility</p>
  <p><span style="background-color: #3ee9d1">&nbsp;&nbsp;&nbsp;&nbsp;</span> Other</p>
  <p><span style="background-color: #ce43eb">&nbsp;&nbsp;&nbsp;&nbsp;</span> Lab research</p>
  <p><span style="background-color: #4d92eb">&nbsp;&nbsp;&nbsp;&nbsp;</span> Online research</p>
  <p><span style="background-color: #935300">&nbsp;&nbsp;&nbsp;&nbsp;</span> Partners collaboration - co-design</p>
</div>

<ul class="timeline_ul">
  {% for post in site.posts reversed %}
      <div class="timeline_card">
        <div class="timeline_head {{post.type}}">
          <div class="date_{{post.type}}" > {{ post.display_date }} </div>
          <!-- <br>  -->
          <div class="type_{{post.type}}" > </div>  
        </div>
        <div class="timeline_body">
          {{ post.excerpt }}
        </div>
        <!-- <span class="initials">{{ post.initials }}</span> -->

      </div>
  {% endfor %}
</ul>


</section>
