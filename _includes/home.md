<p> My name is Phil - thanks for checking out my personal site! </p>

<p>This site is still being put together but it's underway with some general information <a href="./about" title="Go to About me!"> about me </a> and some of the <a href="./projects" title="Go to Projects!"> projects </a> I've worked on or am currently working on :) </p>

<p> Below is a picture of my dog, Pinto! </p>

<p> She is <span id="PintoAge"> </span> months old and loves exploring the world, her frisbee, and wiggling! </p>

<img src="{{ '/public/images/pinto.jpg' | relative_url }}" alt="Pinto!">

<script>

$( document ).ready(function() {

    $today = new Date($.now());

    // months are zero-based! But days and years are one-based ... ;)
    $birthday = new Date(2020, 03, 26);

    console.log($today);
    console.log($birthday);

    $('#PintoAge').text(differenceInMonths($birthday, $today));

});

function differenceInMonths(dateFrom, dateTo) {

    return dateTo.getMonth() - dateFrom.getMonth() + 
    (12 * (dateTo.getFullYear() - dateFrom.getFullYear()))
    
}

</script>