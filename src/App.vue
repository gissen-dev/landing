<script setup lang="ts">
import logo from '/favicon.svg'

const CONTACT = 'hello@gissen.dev'
const GITHUB = 'https://github.com/gissen-dev'
</script>

<template>
  <div class="shell">
    <header class="topbar">
      <div class="brand">
        <img :src="logo" alt="Gissen logo" width="30" height="30" />
        <span class="word">gissen</span>
      </div>
      <span class="badge"><span class="dot" aria-hidden="true"></span>COMING SOON</span>
    </header>

    <main class="hero">
      <p class="eyebrow">Open source · MIT · Self-hosted</p>

      <h1>The headless visual<br />editor for <span class="grad">Vue</span>.</h1>

      <p class="sub">
        Drag and drop your existing Vue components to build pages, marketing sites,
        or your own CMS. Open source, MIT-licensed, self-hosted — and agent-ready.
      </p>

      <p class="launch">
        <span class="bar" aria-hidden="true"></span>
        Launching late 2026
      </p>

      <div class="actions">
        <a class="ghbtn" :href="GITHUB" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true">
            <path
              fill-rule="evenodd"
              d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8Z"
            />
          </svg>
          GitHub
        </a>
      </div>
    </main>
  </div>

  <footer>
    <div class="foot-inner">
      <span>© 2026 Gissen — MIT licensed</span>
      <a :href="`mailto:${CONTACT}`">{{ CONTACT }}</a>
    </div>
  </footer>
</template>
