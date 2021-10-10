<template>
  <form @submit.prevent spellcheck="false" class="my-4">
    <label for="text"><h4>Enter your text in latin characters:</h4></label>
    <textarea
      class="form-control"
      id="text"
      v-model="text"
      @input="translate()"
      spellcheck="false"
      required
    ></textarea>
    <br />
    <label for="result"><h4>Result in Linear B:</h4></label>
    <textarea
      class="form-control"
      id="result"
      v-model="result"
      readonly
    ></textarea>
    <br />
    <button
      type="button"
      class="btn btn-outline-danger"
      style="margin-right: 0.5em"
      @click="clearForm()"
    >
      Clear All
    </button>
  </form>
</template>

<script>
export default {
  name: "Translator",
  data() {
    return {
      text: "",
      result: "",
    };
  },
  methods: {
    translate: function () {
      this.result = this.text
        .replace(/tu/g, "𐀶")
        .replace(/su/g, "𐀱")
        .replace(/ru/g, "𐀬")
        .replace(/pu/g, "𐀢")
        .replace(/nu/g, "𐀝")
        .replace(/mu/g, "𐀘")
        .replace(/ku/g, "𐀓")
        .replace(/du/g, "𐀉")
        .replace(/u/g, "𐀄")
        .replace(/zo/g, "𐀿")
        .replace(/wo/g, "𐀺")
        .replace(/to/g, "𐀵")
        .replace(/so/g, "𐀰")
        .replace(/ro/g, "𐀫")
        .replace(/qo/g, "𐀦")
        .replace(/po/g, "𐀡")
        .replace(/no/g, "𐀜")
        .replace(/mo/g, "𐀗")
        .replace(/ko/g, "𐀒")
        .replace(/jo/g, "𐀍")
        .replace(/do/g, "𐀈")
        .replace(/o/g, "𐀃")
        .replace(/wi/g, "𐀹")
        .replace(/ti/g, "𐀴")
        .replace(/si/g, "𐀯")
        .replace(/ri/g, "𐀪")
        .replace(/qi/g, "𐀥")
        .replace(/pi/g, "𐀠")
        .replace(/ni/g, "𐀛")
        .replace(/mi/g, "𐀖")
        .replace(/ki/g, "𐀑")
        .replace(/di/g, "𐀇")
        .replace(/i/g, "𐀂")
        .replace(/ze/g, "𐀽")
        .replace(/we/g, "𐀸")
        .replace(/te/g, "𐀳")
        .replace(/se/g, "𐀮")
        .replace(/re/g, "𐀩")
        .replace(/qe/g, "𐀤")
        .replace(/pe/g, "𐀟")
        .replace(/ne/g, "𐀚")
        .replace(/me/g, "𐀕")
        .replace(/ke/g, "𐀐")
        .replace(/je/g, "𐀋")
        .replace(/de/g, "𐀆")
        .replace(/e/g, "𐀁")
        .replace(/za/g, "𐀼")
        .replace(/wa/g, "𐀷")
        .replace(/ta/g, "𐀲")
        .replace(/sa/g, "𐀭")
        .replace(/ra/g, "𐀨")
        .replace(/qa/g, "𐀣")
        .replace(/pa/g, "𐀞")
        .replace(/na/g, "𐀙")
        .replace(/ma/g, "𐀔")
        .replace(/ka/g, "𐀏")
        .replace(/ja/g, "𐀊")
        .replace(/da/g, "𐀅")
        .replace(/a/g, "𐀀")
        .replace(/10/g, "𐄐")
        .replace(/1/g, "𐄇")
        .replace(/2/g, "𐄈")
        .replace(/3/g, "𐄉")
        .replace(/4/g, "𐄊")
        .replace(/5/g, "𐄋")
        .replace(/6/g, "𐄌")
        .replace(/7/g, "𐄍")
        .replace(/8/g, "𐄎")
        .replace(/9/g, "𐄏");
    },
    clearForm: function () {
      this.text = "";
      this.result = "";
    },
  },
};
</script>