<p> My name is Phil, and welcome to my personal site! </p>

<p>This site is updated sporadically as time allows and serves as a place for some general information <a href="./about" title="Go to About me!"> about me </a> and a brief portfolio of some of the shareable <a href="./projects" title="Go to Projects!"> projects / side learnings </a> I've worked on or am currently working on. </p>

<p> It's also a place to show pictures of and talk about my dog, Pinto! </p>

<p> She is an <span id="PintoAge"> </span> month <span id="PintoAgeWeeks"> </span> old Austrailian Shepard who loves exploring the world, frisbees, and wiggling! &#128512; </p>

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