---
layout: categories
permalink: /categories/
title: Theme Changer
search_exclude: true
---

<!-- Define CSS variables for the theme colors -->
<style>
:root {
  --primary-color: #007bff; /* blue */
  --secondary-color: #6c757d; /* gray */
  --accent-color: #28a745; /* green */
}
</style>

<!-- Add a button to toggle the theme -->
<button onclick="toggleTheme()">Toggle Theme</button>

<!-- Define a JavaScript function to toggle the theme -->
<script>
function toggleTheme() {
  // Get the current theme color values
  let primaryColor = getComputedStyle(document.documentElement).getPropertyValue('--primary-color');
  let secondaryColor = getComputedStyle(document.documentElement).getPropertyValue('--secondary-color');
  let accentColor = getComputedStyle(document.documentElement).getPropertyValue('--accent-color');

  // Toggle the theme colors
  if (primaryColor === '#007bff') {
    document.documentElement.style.setProperty('--primary-color', '#dc3545'); /* red */
    document.documentElement.style.setProperty('--secondary-color', '#6c757d'); /* gray */
    document.documentElement.style.setProperty('--accent-color', '#fd7e14'); /* orange */
  } else if (primaryColor === '#dc3545') {
    document.documentElement.style.setProperty('--primary-color', '#28a745'); /* green */
    document.documentElement.style.setProperty('--secondary-color', '#6c757d'); /* gray */
    document.documentElement.style.setProperty('--accent-color', '#ffc107'); /* yellow */
  } else {
    document.documentElement.style.setProperty('--primary-color', '#007bff'); /* blue */
    document.documentElement.style.setProperty('--secondary-color', '#6c757d'); /* gray */
    document.documentElement.style.setProperty('--accent-color', '#28a745'); /* green */
  }
}
</script>
