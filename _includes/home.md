<p> My name is Phil - thanks for checking out my personal site! </p>

<p>This site is still being put together but it's underway with some general information <a href="./about" title="Go to About me!"> about me </a> and some of the <a href="./projects" title="Go to Projects!"> projects </a> I've worked on or am currently working on :) </p>

<p> Below is a picture of my dog, Pinto! </p>

<p> She is <span id="PintoAge"> </span> months <span id="PintoAgeWeeks"> </span> old and loves exploring the world, her frisbee, and wiggling! </p>

<img src="{{ '/public/images/pinto.jpg' | relative_url }}" alt="Pinto!">

<script>

$( document ).ready(function() {

    $today = new Date($.now());

    // months are zero-based! But days and years are one-based ... ;)
    $birthday = new Date(2020, 03, 26);

    let weeksDays = differenceInWeeks($birthday, $today);

    const weeks = weeksDays[0];
    const days = weeksDays[1];

    $('#PintoAge').text(differenceInMonths($birthday, $today));
    $('#PintoAgeWeeks').text('('+ weeks + ' weeks and ' + days + ' days)');

});

function differenceInMonths(dateFrom, dateTo) {

    return dateTo.getMonth() - dateFrom.getMonth() + 
    (12 * (dateTo.getFullYear() - dateFrom.getFullYear()))
    
}

function differenceInWeeks(dt2, dt1) {

  // for weeks
  var diff =(dt2.getTime() - dt1.getTime()) / 1000;
  diff /= (60 * 60 * 24 * 7);


  // for days
  n = Math.abs(diff); 
  var decimal = n - Math.floor(n)

  var weeks = Math.abs(Math.round(diff));
  var days = Math.round(decimal * 7);

  return [weeks, days];
  
 }

</script>