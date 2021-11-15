<p> My name is Phil, and welcome to my personal site! </p>

<p>This site is updated sporadically and serves as a place for some general information <a href="./about" title="Go to About me!"> about me </a> and a brief portfolio of some of the <a href="./projects" title="Go to Projects!"> projects and side things </a> I've worked on or am currently working on. </p>

<p> It's also a place to show pictures of and talk about my dog, Pinto! </p>

<p> She is a <span id="PintoAge"> </span> old Australian Shepard who loves exploring, playing frisbee, and of course...wiggling! &#128512; </p>

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

    today = new Date()
    
    // April 26, 2020
    birthday = new Date(2020,03,26)

    a = calcDate(today, birthday)
    console.log(a)


    $('#PintoAge').text(a);

});

function calcDate(date1,date2) {

    var diff = Math.floor(date1.getTime() - date2.getTime());
    var day = 1000 * 60 * 60 * 24;

    var days = Math.floor(diff/day);
    var months = Math.floor(days/31);
    var years = Math.floor(months/12);

    var monthsThisYear = months - (years * 12);

    var combined;

    if (monthsThisYear === 0) {

      combined = years + " year ";

    } else {
      
      combined = years + " year and " + monthsThisYear + " month ";
    }
    return combined;

}

</script>
