---
layout: Page
permalink: /Theme Changer/
title: Theme Changer
---

Toggle Theme <script> const toggleButton = document.querySelector('#theme-toggle'); const themeLink = document.querySelector('#theme-link'); toggleButton.addEventListener('click', () => { if (themeLink.getAttribute('href') === '../assets/css/dark-mode.css') { themeLink.setAttribute('href', '../assets/css/light-mode1.css'); } else { themeLink.setAttribute('href', '../assets/css/dark-mode.css'); } }); </script>