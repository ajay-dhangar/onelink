# Onelink

Onelink is an experimental link-in-bio tool, where the data lives in the URL. 

![screencapture-onelink-ajay-vercel-app-2023-02-04-10_40_24](https://user-images.githubusercontent.com/99037494/216749916-8466c034-ec03-4cf0-9b52-279e11bd6f35.png)

<a href="https://www.youtube.com/channel/UCRQBq8dfTEZfIMxmq-Ba9Tw" target="_blank">
<img src=https://img.shields.io/badge/YouTube_Subscriber-1.11K-orange.svg?style=flat-square=behance&logoColor=white alt=youtube style="margin-bottom: 5px;" />
</a> 
  
 <a href="https://bettercodehub.com/" target="_blank">
<img src=https://img.shields.io/badge/Better_Code-8/10-orange.svg?style=flat-square=behance&logoColor=white alt=bettercodehub style="margin-bottom: 5px;" />
</a> 

<a href="https://opencollective.com/twitter-bio" target="_blank">
<img src=https://opencollective.com/twitter-bio/tiers/badge.svg alt=opencollective style="margin-bottom: 5px;" />
</a> 
 
<a href="https://feedingtrends.com/u/ajaydhangar49" target="_blank">
<img src=https://img.shields.io/badge/Feeding_Trends-31-orange.svg?style=flat-square=behance&logoColor=white alt=feedingtrend style="margin-bottom: 5px;" />
</a> 

<a href="https://ajaydhangar49.hashnode.dev/" target="_blank">
<img src=https://img.shields.io/badge/Hashnode-6-orange.svg?style=flat-square=behance&logoColor=white alt=hashnode style="margin-bottom: 5px;" />
</a> 

<a href="https://ajaydhangar49.medium.com/" target="_blank">
<img src=https://img.shields.io/badge/Medium-31-orange.svg?style=flat-square=behance&logoColor=white alt=medium style="margin-bottom: 5px;" />
</a> 


Here's a demo page

[View Demo](https://onelink-ajay.vercel.app/1?data=eyJuIjoiQWpheSBEaGFuZ2FyICIsImQiOiJJIGFtIFdlYiBEZXZlbG9wZXIuIiwiaSI6Imh0dHBzOi8vYXZhdGFycy5naXRodWJ1c2VyY29udGVudC5jb20vdS85OTAzNzQ5ND92PTQiLCJmIjoiaHR0cHM6Ly93d3cuZmFjZWJvb2suY29tL3Byb2ZpbGUucGhwP2lkPTEwMDA3ODMxNjY1NzE1MiIsInQiOiJodHRwczovL3R3aXR0ZXIuY29tL0FKQVlESEEyNzI1MDAxNiIsImlnIjoiQGFqLmVkdS5pbiIsImdoIjoiaHR0cHM6Ly9naXRodWIuY29tL0FqYXktRGhhbmdhciIsInRnIjoiaHR0cHM6Ly90Lm1lL2FqX3plcm9fY29kaW5nIiwibCI6Imh0dHBzOi8vd3d3LmxpbmtlZGluLmNvbS9pbi9hamF5LWRoYW5nYXItYmI4OWI0MjI3LyIsImUiOiJhamF5ZGhhbmdhcjQ5QGdtYWlsLmNvbSIsInciOiI3MDI0NTkyMTA1IiwieSI6Imh0dHBzOi8vd3d3LnlvdXR1YmUuY29tL0BBamF5LURoYW5nYXIiLCJscyI6W3siaSI6ImFudC1kZXNpZ246Z2xvYmFsLW91dGxpbmVkIiwibCI6IlBvcnRmb2xpbyIsInUiOiJodHRwczovL2FqYXktZGhhbmdhci5naXRodWIuaW8vUmVzcG9uc2l2ZS1wb3J0Zm9saW8td2Vic2l0ZS5naXRodWIuaW8vI2hvbWUifSx7ImkiOiJmYS1icmFuZHM6bWVkaXVtLW0iLCJsIjoiTWVkaXVtIiwidSI6Imh0dHBzOi8vYWpheWRoYW5nYXI0OS5tZWRpdW0uY29tLyJ9LHsiaSI6Im1hdGVyaWFsLXN5bWJvbHM6ZWRpdC1kb2N1bWVudCIsImwiOiJSZXN1bWUiLCJ1IjoiaHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2ZpbGUvZC8xYURxN2loTExyTXNzc0JiMUd1d2ltVVJ6dEIxeDkycUMvdmlldyJ9LHsiaSI6ImFyY3RpY29uczpsZXR0ZXItdXBwZXJjYXNlLWgiLCJsIjoiSGFzaG5vZGUiLCJ1IjoiaHR0cHM6Ly9hamF5ZGhhbmdhcjQ5Lmhhc2hub2RlLmRldi8ifV19)

The data is converted to a base 64 string which we onelink uses as a query parameter. I have tried to reduce the json keys to be as small as possible

Roadmap.
1. Templates - make different templates, the `/1` after the host is basically a template here.
2. Refactor code - a lot of repeated boilerplate code is added here - refactor it properly.

## Setup locally

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.
