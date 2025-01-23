# Tailwind---play

An advanced online playground for Tailwind CSS, including support for things like:

Customizing your theme with @theme

Adding custom utilities with @utility

Adding custom variants with @variant

Code completion with instant preview

Perfect for learning how the framework works, prototyping a new idea, or creating a demo to share online.


# Tailwind CSS Setup with Vite

This repository demonstrates how to integrate **Tailwind CSS** with **Vite** for seamless styling. Tailwind CSS is a utility-first CSS framework that works by scanning your HTML, JavaScript, and template files for class names, generating the corresponding styles, and writing them to a static CSS file.

It’s fast, flexible, and reliable — with **zero-runtime**.

## Installation

### Prerequisites
Ensure you have [Node.js](https://nodejs.org/) installed on your machine.

### Getting Started

Follow these steps to set up Tailwind CSS with Vite.

### 1. Install Tailwind CSS and Vite Plugin

In your project directory, run the following command to install `tailwindcss` and the Vite plugin for Tailwind CSS:

```bash
npm install tailwindcss @tailwindcss/vite
``` 
2. Configure Vite Plugin
Next, configure the @tailwindcss/vite plugin in your vite.config.ts file:

typescript
Copy
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
3. Import Tailwind CSS in Your CSS File
In your main CSS file, add the @import directive to include Tailwind CSS:

css
Copy
@import "tailwindcss";
4. Start Your Build Process
To start the build process, run the following command:

bash
Copy
npm run dev
This will start the development server and compile your Tailwind CSS.

5. Using Tailwind in Your HTML
Once the CSS is compiled, make sure to include the generated CSS in your HTML file. You can do this by adding the link to the compiled CSS in the <head> section of your HTML file:

html
Copy
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/styles.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
Now you can start using Tailwind CSS utility classes to style your HTML elements!

Additional Resources
Tailwind CSS Documentation
Vite Documentation
Happy coding! ✨
