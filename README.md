<!DOCTYPE html>
<!--
Created using JS Bin
http://jsbin.com

Copyright (c) 2020 by tamasisandor2014 (http://jsbin.com/qinabaw/11/edit)

Released under the MIT license: http://jsbin.mit-license.org
-->
<meta name="robots" content="noindex">
<html>
<head>
  <title>Zoe &amp; Alex</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width initial-scale=1">
  <link rel="shortcut icon" type="image/x-icon" href="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-favicon.png">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.css">
	<link rel="stylesheet" type="text/css" href="css/main.css">
  <link href="https://fonts.googleapis.com/css?family=Great+Vibes%7CLibre+Baskerville:400,400i,700%7CMuli:400,700&display=swap" rel="stylesheet">
<style id="jsbin-css">
/* =============================

    GENERAL STYLES

=============================*/

* {
  box-sizing: border-box;
}

/* Single-direction margin declaration to establish vertical rhythm. */
h1,h2,h3,
ul,ol,
p,
img {
    margin-bottom: 1.5rem;
}

body {
  background: url('https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-background.png') repeat center;
  font-family: 'Libre Baskerville', serif;
  font-size: 1.125rem;
  line-height: 1.5;
  color: #444349;
}

.locations,
.program,
.gifts,
.faq,
.contact {
  width: 95%;
  margin: 1.5rem auto;
  padding: .5rem 1rem;
  text-align: center;
}

h1,
h2 {
  font-family: 'Great Vibes', cursive;
}

h2 {
  font-size: 3rem;
}

h3 {
  font-size: 1.5rem;
}

a {
  text-decoration: none;
  color: #bd806e;
}

a:hover {
  color: #eda087;
  transition: color .15s ease-in-out;
}

/* =============================

    HEADER STYLES

=============================*/

.cover {
  background: url('https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-cover.jpg') no-repeat 70% center/cover;
  display: table;
  text-align: center;
  height: 100vh;
  width: 100vw;
}

@media (min-width: 768px) {

  .cover {
    background: url('https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-cover.jpg') no-repeat center/cover;
  }

}

.hero-text-wrapper {
  display: table-cell;
  vertical-align: middle;
}

.hero-text {
  margin: 0 auto;
  padding: .625rem;
  color: hsla(0,0%,100%,.9);
  background: hsla(100,0%,0%,.5);
}

.hero-text h1 {
  font-size: 3.15rem;
  color: #d2ba87;
  margin-bottom: 0; /* To negate the effect of the single-direction margin declaration. */
}

@media (min-width: 768px) {

  .hero-text {
    padding: 1.25rem;
    border-radius: 4px;
    width: 50%;
  }

  .hero-text h1 {
    font-size: 7rem;
  }

}


.tagline {
  font-size: 1.25rem;
  letter-spacing: .15rem;
}

@media (min-width: 768px) {

  .tagline {
    text-transform: uppercase;
  }

}

.tagline::after {
  display: block;
  content: "";
  background-color: #fff;
  height: 1px;
  width: 12.515625rem;
  margin: .5rem auto;
}

.date {
  font-size: 1.25rem;
  letter-spacing: .15rem;
  vertical-align: middle;
}

.date::before,
.date::after {
  display: inline-block;
  content: "";
  background-color: #fff;
  height: 1px;
  width: 1.5rem;
  vertical-align: middle;
  margin: 0 .5rem;
}

/* =============================

      LOCATIONS STYLES

=============================*/

.blurb img {
  height: 7.5rem;
}

.blurb h3 {
  font-weight: 700;
}

.blurb div {
  font-family: 'Muli', sans-serif;
}


.blurb::after {
  content: "";
  display: block;
  height: .1875rem;
  width: 25vw;
  margin: 1.5rem auto;
  background-color: #444349;
}

@media (min-width: 768px) {

  .blurb {
    display: inline-block;
    width: 30%;
    padding: 1.5rem;
    margin: .5rem;
  }

  .blurb::after {
    display: none;
  }

}

/* =============================

        PROGRAM STYLES

=============================*/

.program {
  width: 100vw;
  text-align: left;
  background: hsla(100,0%,0%,.6);
  color: #d2ba87;
  font-family: 'Muli', sans-serif;
}

.program h2 {
  font-family: 'Great Vibes', cursive;
  margin-top: 1rem; /* To account for the unequal margins compared to the previous section. */
  text-align: center;
}

.program p {
  font-style: italic;
}

.program ul {
  letter-spacing: .025rem;
}

@media (min-width: 768px) {

  .program-wrapper {
    width: 30vw;
    margin: 0 auto;
  }

}

/* =============================

        GIFTS STYLES

=============================*/

.gifts img {
  height: 7.5rem;
}

.gifts p:last-child {   /* To even out the bottom and top margins of this section. */
  margin-bottom: 0;
}

/* =============================

        FAQ STYLES

=============================*/

.faq {
  background: hsla(100,0%,0%,.6);
  color: #d2ba87;
  width: 100vw;
  text-align: center;
}

.faq h2 {
  margin-top: 1rem; /* To even out top and bottom margins. */
}

.faq p {
  font-family: 'Muli', sans-serif;
  text-align: left;
}

.question-group::after {
  content: "";
  display: block;
  height: .1875rem;
  width: 50vw;
  margin: 1.5rem auto;
  background-color: #d2ba87;
}

.question {
  font-weight: 700;
  margin-bottom: .5rem;
}

.answer {
  margin-bottom: 1.5rem;
}

@media (min-width: 768px) {

  .question-group {
    display: inline-block;
    width: 30%;
    vertical-align: top;
    padding: 1.5rem;
    margin: .5rem;
  }

  .question-group::after {
    display: none;
  }

  .question-group h3 {
    text-align: left;
  }

}

/* =============================

        FOOTER STYLES

=============================*/

footer {
  height: 10vh;
  width: 100vw;
  background-color: #606060;
  color: #fff;
  font-family: 'Muli', sans-serif;
  display: table;
  text-align: center;
  font-size: .875rem;
}

.footer-wrapper {
  display: table-cell;
  vertical-align: middle;
  padding: .5rem 1rem;
}

footer p {
  margin-bottom: 0;
}

footer small {
  line-height: 1.5;
}

@media (min-width: 768px) {

  footer {
    min-height: 7vh;
  }

}
</style>
</head>
<body>
  <header class="cover">
      <div class="hero-text-wrapper">
        <div class="hero-text">
          <div class="tagline">We're getting married!</div>
          <h1>Zoe &amp; Alex</h1>
          <span class="date">August 1, 2018</span>
        </div>
      </div>
  </header>
  <main>
    <section class="locations">
      <h2>Locations</h2>
      <div class="blurb">
        <h3>Ceremony</h3>
        <img src="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-ceremony.png" alt="Ceremony">
        <div>St. Nicholas Church</div>
        <div>2 Trinity Square, Budapest</div>
      </div>
      <div class="blurb">
        <h3>Photos</h3>
        <img src="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-photoshoot.png" alt="Photoshoot">
        <div>Liberty Bastion</div>
        <div>23 Wisdom Road, Budapest</div>
      </div>
      <div class="blurb">
        <h3>Party</h3>
        <img src="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-party.png" alt="Party">
        <div>Heaven Lounge</div>
        <div>14 Fairy Street, Budapest</div>
      </div>
    </section>
    <section class="program">
      <h2>Program</h2>
      <div class="program-wrapper">
        <p>"It's going to be somehow, that's for sure."</p>
        <ul>
          <li>13:45 – Wedding ceremony</li>
          <li>14:30 – Photos</li>
          <li>16:00 – Cocktails</li>
          <li>18:00 – Dinner</li>
          <li>22:00 – Cake</li>
          <li>... - 4:00 – Dance until dawn</li>
        </ul>
      </div>
    </section>
    <section class="gifts">
      <h2>Gifts</h2>
      <p>The greatest gift for us is to have you there.</p>
      <img src="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-gifts.png" alt="Gifts">
      <p>Please, just bring yourself and have fun with us.</p>
    </section>
    <section class="faq">
      <h2>Questions &amp; Answers</h2>
        <div class="question-group">
          <h3>Travel and accomodations</h3>
            <p class="question">Will there be some kind of organized transfer?</p>
            <p class="answer">No, we'll just meet at the church at 13:15.</p>
            <p class="question">Where can I park?</p>
            <p class="answer">Parking is free on the weekends in the 1st district. The locations are close to each other so you won't need your car.</p>
            <p class="question">How can I get home at night?</p>
            <p class="answer">The 916 bus is in service all night at the castle and it hits every major traffic hub in the city.</p>
        </div>
        <div class="question-group">
          <h3>Food and festivities</h3>
            <p class="question">I'd like to do some kind of surprise for you guys at the party. To whom should I talk about this?</p>
            <p class="answer">Discuss it with Abigail Smith. Just drop her an email at <a href="mailto:abigail@awesomemail.com">abigail@awesomemail.com</a>.</p>
            <p class="question">What should I wear? Do you have a dress code?</p>
            <p class="answer">Wear what's comfortable to you. If it helps <a href="#" target="_blank">smart casual</a> / <a href="#" target="_blank">business casual</a> for the ladies and <a href="#" target="_blank">smart casual</a> / <a href="#" target="_blank">informal</a> for the gentlemen are perfect options.</p>
            <p class="question">I would like some kind of special food (gluten-free, lactose-free, vegan etc.)</p>
            <p class="answer">Drop us a line <a href="mailto:zoeandalex@awesomemail.com">here</a> and we'll find a way.</p>
        </div>
        <div class="question-group">
          <h3>Other small stuff</h3>
            <p class="question">I have a problem / question on the wedding day. With whom can I speak?</p>
            <p class="answer">Jared Wright on this number: <a href="tel:+36300000000">+36 30 000 0000</a>.</p>
            <p class="question">Can we bring kids?</p>
            <p class="answer">Sure! We planned a whole toy / sweets corner for them.</p>
            <p class="question">How do you feel about dogs? Can I bring mine?</p>
            <p class="answer">We love dogs and you can absolutely bring yours. The Heaven Lounge is a dog-friendly place.</p>
        </div>
    </section>
    <section class="contact">
      <h2>Contact</h2>
      <p>If you have any questions feel free to call / write us.</p>
      <p>Phone: <a href="tel:+36300000000">+36 30 000 0000</a> (Zoe) / <a href="tel:+36300000000">+36 30 000 0000</a> (Alex)</p>
      <p>Email: <a href="mailto:zoeandalex@awesomemail.com">zoeandalex@awesomemail.com</a></p>
    </section>
  </main>
  <footer>
    <div class="footer-wrapper">
      <p><small>Made with  ♥ in Budapest ©2018 | Icons by <a href="http://www.flaticon.com/authors/becris" title="Becris">Becris</a> (<a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a>)</small></p>
    </div>
  </footer>
</body>
</html>
