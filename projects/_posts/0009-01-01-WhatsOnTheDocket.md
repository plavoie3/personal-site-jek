---
layout: project
title: What's On The Docket?
---

<span class="post-date"> Web App (HTML + CSS + JavaScript + PHP + MySQL) </span>

<div class="message"> 

<p> End of semester final project for Database Design for the Web course. Virtual pantry and meal/recipe suggestion service. </p>

<p> Awarded 2nd Place in UVM CS Fair Web Design Category </p>  

</div>

<div class="slider">
	<div> 
        <img src="{{ '/public/images/docket/docketInitial.png' | relative_url }}" alt="Home"> 
        <div class="slide__caption">Welcome to WOTD.</div>
    </div>
    <div>
        <img src="{{ '/public/images/docket/docketRegister.png' | relative_url }}" alt="">
        <div class="slide__caption">Register with your service preferences.</div>
    </div>
    <div>
        <img src="{{ '/public/images/docket/docketPantry.png' | relative_url }}" alt="">
        <div class="slide__caption"> Keep an inventory of your available ingredients.</div>
    </div>
    <div>
        <img src="{{ '/public/images/docket/docketReady.png' | relative_url }}" alt="">
        <div class="slide__caption"> See identified "ready to cook" recipes based on your preferences and pantry items!</div>
    </div>
    <div>
        <img src="{{ '/public/images/docket/docketAllRecipes.png' | relative_url }}" alt="">
        <div class="slide__caption"> Browse and search the entire recipe cookbook by ingredient, keyword, etc...yum!</div>
    </div>
    <div>
        <img src="{{ '/public/images/docket/docketAdmin.png' | relative_url }}" alt="">
        <div class="slide__caption"> Interface to add new recipes and keep the docket rolling!</div>
    </div>
</div>


<script>

    $(document).ready(function(){

        $('.slider').slick({
            dots: true,
            infinite: true,
            autoplay: true,
            autoplaySpeed: 7000,
            speed: 500,
            fade: true,
            cssEase: 'linear'
          });
    });

</script>

