<script setup lang="ts">
import { useDark, useToggle, useTitle } from "@vueuse/core";
const isDark = useDark()
</script>

<template>
  <h1>🇺🇦 IT Спільнота</h1>
  <p>Привіт, друже!</p>

  <p>Ми раді вітати тебе на сайті спільноти присвяченої українському IT 🇺🇦</p>

  <p>
    У нас в <img src="/discord.png" class="icon" />, ти знайдеш усе що побажаєш,
    від цікавого та корисного контенту, до відпочинку після робочого дня.
  </p>

  <div class="list-and-widget">
    <div>
      <ul>
        <li>Актуальні новини зі світу IT. 📰</li>
        <li>Свіжі та круті вакансії. 👨🏻‍💻</li>
        <li>Цікаві meetup-и на будь-яку тему. 🎙</li>
        <li>Допомога на підтримку на будь-яке твоє запитання. 🛟</li>
        <li>Публічні holywar-и. 🎤</li>
        <li>Експерти у своїй галузі, які завжди онлайн у чаті. 🧑🏼‍🔬</li>
        <li>Поради про кар'єрний розвиток, та life-work баланс. 👨🏼‍⚕️</li>
        <li>
          Та багато розважального контенту, у голосових та текстових чатах.
        </li>
      </ul>

      <h3 class="join">
        Долучайся!<br />
        <a href="https://discord.gg/BWXC9KB9Gs"
          >https://discord.gg/BWXC9KB9Gs</a
        >
      </h3>
      <h5></h5>
    </div>
    <iframe
      v-if="isDark"
      src="https://discord.com/widget?id=932734827545903104&theme=dark"
      width="250"
      height="300"
      allowtransparency="true"
      frameborder="0"
      sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
    ></iframe>
    <iframe
      v-else
      src="https://discord.com/widget?id=932734827545903104&theme=light"
      width="250"
      height="300"
      allowtransparency="true"
      frameborder="0"
      sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
    ></iframe>
  </div>
</template>
