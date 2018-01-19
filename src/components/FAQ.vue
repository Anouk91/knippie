<template>

  <div class="faq" style="padding-bottom: 5rem; width: 100%;">
    <h3 style="padding:2rem;">Frequently Asked Questions</h3>
    <div v-b-toggle.collapse1 class="question">
      Don’t your cards easily fall out?
      </div>
    <b-collapse id="collapse1" class="answer">
      <p>
        <span>Nope has never occured to me yet, and I'm using Knippies already for over a year. </span>
        <span>Besides, as people who know me a little know, I'm not the most careful... </span>
        <span>PS Small movie will follow soon!</span>
        </p>
    </b-collapse>
    <div v-b-toggle.collapse2 class="question">
      Doesn’t the elastic gets dirty?
      </div>
    <b-collapse id="collapse2" class="answer">
      <p>
        <span>It does change slightly, but not annoyingly to my opinion. </span>
        <span>PS Photo is on it's way!</span>
        </p>
    </b-collapse>
    <div v-b-toggle.collapse3 class="question">
      How can I get my own Knippie?
      </div>
    <b-collapse id="collapse3" class="answer">
      <p>
        <span>By sending me an email or text message!</span>
        <span> boukema.a@gmail.com</span>
        <span> +31612377790</span>
      </p>
    </b-collapse>





  </div>
  
</template>


<style>
.faq * {
  text-align: left;
}
.question {
  padding-left: 3rem;
  font-weight: bold;
}

.answer {
  padding-left:4rem;
  font-style: italic;
}

p span{
  display: block;
}
</style>
