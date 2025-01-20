# Tailwind CSS `@apply` Directive in Style Tag Issue

This repository demonstrates a common issue when using Tailwind CSS's `@apply` directive within an inline `<style>` tag.  The `@apply` directive is intended for use within your main CSS file or other imported CSS files.  Placing it directly in a style tag often leads to it being ignored by the Tailwind build process. 

The `bug.html` file shows the problem. The `bugSolution.html` file demonstrates the correct approach.

**Solution:** Avoid using `@apply` within inline `<style>` tags.  Instead, place your styles in your main CSS file or use a standard CSS approach within the `<style>` tag without `@apply`.