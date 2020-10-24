---
layout: project
title: StentTrack
permalink: projects/StentTrack
---

<span class="post-date"> iOS App (Swift + Xcode) </span>

<div class="message"> 

<p> A pain tracking and medication scheduling/notification app to improve patient compliance and pain management while allowing researchers to study the effectiveness of medication plans following stent placement. </p>

<p> Ultimately designed to help researchers demonstrate the feasibility of implementing a nonopioid protocols to manage postoperative pain after ureteroscopy with stent placement. </p>  

</div>

<div class="slider">
	<div> 
        <img src="{{ '/public/images/stent_setup.png' | relative_url }}" alt="Minimum required attributes"> 
        <div class="slide__caption">
        First app launch open with notifications opt-in / opt-out.
        </div>
    </div>
        <div>
        <img src="{{ '/public/images/stent_setup2.png' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption">
            First dose day / time is set (administered in post-op care before patient is sent home). <br>
            Follow up day / time is also set.
        </div>
    </div>
        <div>
        <img src="{{ '/public/images/stent_notifications.jpg' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption"> At home, patient is notified when it is time to take next dose <br> 
        Opening notification draws user into app to submit a pain/symptoms and medication status update.</div>
    </div>
    <div>
        <img src="{{ 'public/images/stent_ready_meds.png' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption">Patient sets pain level and indicates which "ready for next does / green" medicines they have taken. </div>
    </div>
    <div>
        <img src="{{ '/public/images/stent_symptoms.png' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption"> Patient indicates which (if any) symptoms they are experiencing.</div>
    </div>
    <div>
        <img src="{{ 'public/images/stent_submit.png' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption">Log submission sent! </div>
    </div>
    <div>
        <img src="{{ 'public/images/stent_log_meds.png' | relative_url }}" alt="Minimum required attributes">
        <div class="slide__caption"> Medicine log view when it is not time for a prescription's next dose</div>
    </div>
</div>


<script>

    $(document).ready(function(){

        $('.slider').slick({
            dots: true,
            infinite: true,
            autoplay: false,
            autoplaySpeed: 7000,
            speed: 500,
            fade: true,
            cssEase: 'linear'
          });
    });

</script>



