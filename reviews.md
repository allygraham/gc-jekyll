---
title: Reviews
layout: default
---

<div class="box">
  <ul class="timeline">
  </ul>
  <script id="reviewList" type="text/x-handlebars-template">
    {{#each reviews}}
    <li {{#if_even @index}}class="timeline-inverted"{{/if_even}}>
      <div class="timeline-badge"><i class="fa fa-comments-o"></i></div>
      <div class="timeline-panel">
        <div class="timeline-heading">
          <h4 class="timeline-title">{{title}}</h4>
          <p class="stars"><img src="./assets/images/5-star-review.png" /></p>
          <p><small class="text-muted"><i class="fa fa-calendar-o"></i> {{date}}</small></p>
        </div>
        <div class="timeline-body">
          <p>{{{comment}}}</p>
            <p><small class="text-muted">{{name}}</small></p>
        </div>
        <div class="timeline-footer">
          <img src="./assets/images/tripadvisor.png" height="50" />
          <a href="https://www.tripadvisor.co.uk/VacationRentalReview-g551745-d1777377-or9-Garden_Cottage_in_the_heart_of_Crail-Crail_Fife_Scotland.html" target="_blank">Read more reviews on TripAdvisor <span class="fa fa-angle-right fa-lg"></span></a>
        </div>
      </div>
    </li>
    {{/each}}
  </script>
</div>
