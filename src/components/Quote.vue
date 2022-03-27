<template>
    <button @click="generate" :style="{ background: 'green'}" class='btn'>Generate Quote</button>
    <div class="quote">
    <p><i>{{ quote.quote }}</i></p> 
    <p><b>{{ quote.cite }}</b></p> </div>
</template>

<script>

const quotes = [
  {
    quote:
      "The purpose of our lives is to be happy.",
    cite: "Dalai Lama",
  },
  {
    quote:
      "Get busy living or get busy dying.",
    cite: "Stephen King",
  },
  {
    quote: "Many of life’s failures are people who did not realize how close they were to success when they gave up.",
    cite: "Thomas A. Edison",
  },
  {
    quote: "If you want to live a happy life, tie it to a goal, not to people or things.",
    cite: "Albert Einstein",
  },
  {
    quote:
      "Curiosity about life in all of its aspects, I think, is still the secret of great creative people.",
    cite: "Leo Burnett",
  },
  {
    quote:
      "Most good programmers do programming not because they expect to get paid or get adulation by the public, but because it is fun to program.",
    cite: "Linus Torvalds",
  },
  {
    quote:
      "The unexamined life is not worth living.",
    cite: "Socrates",
  },
  {
    quote:
      "Don’t settle for what life gives you; make life better and build something.",
    cite: "Ashton Kutcher",
  },
  {
    quote:
      "Life imposes things on you that you can’t control, but you still have the choice of how you’re going to live through this.",
    cite: "Celine Dion",
  },
  {
      quote:"Life is never easy. There is work to be done and obligations to be met – obligations to truth, to justice, and to liberty.",
      cite : "John F. Kennedy"
  },
  {
      quote:"Live for each second without hesitation.",
      cite : "Elton John"
  },{
      quote:"Life is like riding a bicycle. To keep your balance, you must keep moving.",
      cite : "Albert Einstein"
  },
  {
      quote:"My mama always said, life is like a box of chocolates. You never know what you’re gonna get",
      cite : "Forrest Gump "
  },
  {
      quote:"When we do the best we can, we never know what miracle is wrought in our life or the life of another.",
      cite : "Helen Keller"
  }
];

export default {
    name: 'Quote',
    data() {
    return { quote: {} };
  },
    components:{
        
    },
    methods: {
        generate() {
      const index = Math.floor(Math.random() * quotes.length);
      this.quote = quotes[index];
    },
    }

}
</script>

<style scoped>

.quote {
  max-width: 500px;
  margin: 10px auto;
  overflow: auto;
  min-height: 50px;
  border: 1px solid rgb(29, 167, 221);
  padding: 30px;
  border-radius: 10px;
}

</style>
