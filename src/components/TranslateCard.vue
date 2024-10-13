<script setup>
import { ref } from 'vue'

const text = ref('Hello, how are you?')
</script>

<template>
  <article class="card">
    <ul class="options">
      <li>
        <label class="btn-language" for="language">
          Detect Language
          <input type="radio" name="language" value="detect" checked />
        </label>
      </li>
      <li>
        <label class="btn-language">
          <input type="radio" name="language" value="english" />
          English
        </label>
      </li>
      <li>
        <label class="btn-language">
          <input type="radio" name="language" value="french" />
          French
        </label>
      </li>
      <li>
        <label class="btn-language">
          <input type="radio" name="language" value="spanish" />
          Spanish
        </label>
      </li>
    </ul>
    <textarea
      class="content"
      name="textToTranslate"
      id="translate"
      maxlength="500"
      v-model="text"
    ></textarea>
    <span class="character-count">{{ text.length }} / 500 </span>
    <div class="extra">
      <ul class="buttons">
        <li>
          <button>
            <img src="/src/assets/resources/Copy.svg" alt="Copy" />
          </button>
        </li>
        <li>
          <button>
            <img src="/src/assets/resources/sound_max_fill.svg" alt="Copy" />
          </button>
        </li>
      </ul>

      <button class="btn-translate">
        <img src="/src/assets/resources/Sort_alfa.svg" alt="" />
        Translate
      </button>
    </div>
  </article>
</template>

<style scoped></style>
