<template>
  <article class="card">
    <ul class="options">
      <li>
        <label class="btn-language">
          <input type="radio" name="translated" value="english" checked />
          English
        </label>
      </li>
      <li>
        <label class="btn-language">
          <input type="radio" name="translated" value="french" />
          French
        </label>
      </li>
      <li>
        <label class="btn-language">
          <input type="radio" name="translated" value="spanish" />
          Spanish
        </label>
      </li>
    </ul>
    <p class="content"></p>
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
    </div>
  </article>
</template>
