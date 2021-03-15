<p> My name is Phil, and welcome to my personal site! </p>

<p>This site is updated sporadically as time allows and serves as a place for some general information <a href="./about" title="Go to About me!"> about me </a> and a brief portfolio of some of the shareable <a href="./projects" title="Go to Projects!"> projects / side learnings </a> I've worked on or am currently working on. </p>

<p> It's also a place to show pictures of and talk about my dog, Pinto! </p>

<p> She is an <span id="PintoAge"> </span> month <span id="PintoAgeWeeks"> </span> old Austrailian Shepard who loves exploring the world, frisbees, and wiggling! &#128512; </p>

<img src="{{ '/public/images/pinto.jpg' | relative_url }}" alt="Pinto!">

<div class="pa-gallery-player-widget" style="width:100%; height:480px; display:none;"
  data-link="https://photos.app.goo.gl/8zsNaEpEUetYSquk7"
  data-title="Best of Pinto :D"
  data-description="5 new photos added to shared album">
  <object data="https://lh3.googleusercontent.com/awXAcnUsK9NAso2fRk3zMYBFen9kIw7fCOLjhrCgXS_4ep_vOI9u-hAEKt0quRBsFdbwpm9wD384LqoCKcIgDVMIufQkSIl0Izvra3nozWYCicpqmcC_QGC335W34ProPItiLo-9rQ=w1920-h1080"></object>
  <object data="https://lh3.googleusercontent.com/mR9zRWS7cqrM103m0P9LqnRiZaih61pJHuQhkNQTumhs_vMiwIEju2qCtgUzCbqr3QOBQc91GXuMoZsO99sZYSG4tHvUOTNNgoKKQeeekdt-cCieEFxMVD34zfCHLlSFU_zbs_JCew=w1920-h1080"></object>
  <object data="https://lh3.googleusercontent.com/kCEgsjEAtr523ThTuryQo-RgzRZJuUbUZdAB5QOdOtbjuM-5xV_goAZmL0zch57G87I8aHdrZDZ08OHmgnL5eNtQZrS-lyk31aQm-Wz0z_D0HMcvCoz2xbKRA34Rrddu9XMkjp3Akg=w1920-h1080"></object>
  <object data="https://lh3.googleusercontent.com/hbWnI6VMtJYTxBI7d3YjRer7Sij5HSEPPmGN4no8J_Vtsh30STAMTPSDUTelyegHNgqnr5HeS1Eu4nppG30u6kujfkqpHjVIj2bsmJfQNoyVizrIHrGKssAvUmh6ge7obn6ZM_BPFg=w1920-h1080"></object>
  <object data="https://lh3.googleusercontent.com/Ay34UpTdtm0xsSrSE3on3oX4jgkDmmaB7xBv7opc_5sAkPH-guuJJYj3ojLdTFHoo4QU0xMk73XjzmlfnvznwLff5FTDeNF-Bo877iU9ErN9Z_xsXPW3BGPtUJiZtiMgYnKG4NbF6w=w1920-h1080"></object>
</div>

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