<script setup lang="ts">
import logo from '/favicon.svg'

const CONTACT = 'hello@gissen.dev'
const GITHUB = 'https://github.com/gissen-dev'
const X = 'https://x.com/gissen_dev'
const BSKY = 'https://bsky.app/profile/gissen-dev.bsky.social'
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
        <a class="ghbtn" :href="X" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true">
            <path
              d="M9.52 6.77 15.48 0h-1.41L8.9 5.88 4.77 0H0l6.25 8.9L0 16h1.41l5.46-6.2L11.23 16H16L9.52 6.77ZM7.59 8.97l-.63-.89L1.92 1.04h2.17l4.06 5.69.63.89 5.28 7.39h-2.17L7.59 8.97Z"
            />
          </svg>
          X
        </a>
        <a class="ghbtn" :href="BSKY" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true">
            <path
              d="M3.47 1.4C5.31 2.78 7.29 5.58 8 7.08c.71-1.5 2.69-4.3 4.53-5.68C13.86.4 16 -.36 16 2.08c0 .49-.28 4.1-.44 4.69-.58 2.04-2.66 2.56-4.51 2.24 3.23.55 4.05 2.37 2.28 4.19-3.36 3.45-4.83-.87-5.21-1.97-.07-.2-.1-.3-.12-.22-.02-.08-.05.02-.12.22-.38 1.1-1.85 5.42-5.21 1.97-1.77-1.82-.95-3.64 2.28-4.19-1.85.32-3.93-.2-4.51-2.24C.28 6.18 0 2.57 0 2.08 0-.36 2.14.4 3.47 1.4Z"
            />
          </svg>
          Bluesky
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
