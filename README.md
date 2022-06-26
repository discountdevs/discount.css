
<h1 align="center">Discount.css</h1>
<p align="center">A drop-in collection of CSS styles to make simple websites just a little nicer</p>


<br>

## Goals

- Responsive
- Themeable
- Good browser support (works on my old kindle's browser :P)
- Tiny size
- Beautiful
- No classes

## Why?

Discount.css is a CSS framework that doesn't require any classes. You just include it in your `<head>` and forget about it, while it silently makes everything nicer.

## Who?

You might want to use Discount.css if you're making a simple static page or demo website that you don't want to spend time styling.

Although it originally wasn't built for more complex websites, many developers have used Discount.css as a base stylesheet and creatively applied custom styles to build out an entire app. Nothing is stopping you from doing the same!

## How?

Just stick this in your `<head>`:

### 🌙/☀ Automatic Theme:

`<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/discountdevs/discount.css@master/out/discount.min.css">`

### 🌙 Dark Theme:

`<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/discountdevs/discount.css@master/out/dark.min.css">`

### ☀ Light Theme:

`<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/discountdevs/discount.css@master/out/light.min.css">`

<br>

A **preview** of the different themes is available [on the **demo page**]([https://watercss.kognise.dev/#installation](https://discountdevs.github.io/discount.css/out/docs/#installation))! ⚡

#### How the "Automatic Theme" works

The main `water.css` file automatically switches between light and dark mode depending on the system preferences of a user's device. This detection is made possible through a CSS media query called [`prefers-color-scheme`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme). In browsers where the preference can't be detected, `water.css` will stick to the light theme.

If you want to avoid this behavior, use either `dark.css` or `light.css`.

#### Supporting Internet Explorer

All three distributions of Discount.css support Internet Explorer 11, but the main `water.css` file **doesn't respect the user's color scheme** and will be locked to light mode due to lack of `prefers-color-scheme` support.

Be aware that IE also doesn't support [runtime theming](#theming), and fixed fallback values will be used. If you want to override the Discount.css theme in a way that's compatible with IE, we recommend that you [compile your own theme](#compiling-your-own-theme).

#### Unminified builds

All versions are also available as unminified stylesheets, which can be handy during development.  
Simply remove the `.min` from the file name.

## Theming

Do you want to make some adjustments or build your own theme completely different from the official dark or light themes? Since Discount.css is built with CSS variables this is super easy to do! Here's a list list of all the variables you can change to your liking:

- `--background-body`
- `--background`
- `--background-alt`
- `--selection`
- `--text-main`
- `--text-bright`
- `--text-muted`
- `--links`
- `--focus`
- `--border`
- `--code`
- `--animation-duration`
- `--button-hover`
- `--scrollbar-thumb`
- `--scrollbar-thumb-hover`
- `--form-placeholder`
- `--form-text`
- `--variable`
- `--highlight`
- `--select-arrow`
