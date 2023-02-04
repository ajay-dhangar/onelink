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

[View Demo](https://onelink-ajay.vercel.app/1?data=eyJuIjoiQWpheSBEaGFuZ2FyIiwiZCI6IknigJltIFdlYiBEZXZlbG9wZXIsIFlvdVR1YmVyLCBhbmQgTGVhcm5lci4iLCJpIjoiaHR0cHM6Ly9hdmF0YXJzLmdpdGh1YnVzZXJjb250ZW50LmNvbS91Lzk5MDM3NDk0P3Y9NCIsImYiOiJodHRwczovL3d3dy5mYWNlYm9vay5jb20vcHJvZmlsZS5waHA/aWQ9MTAwMDc4MzE2NjU3MTUyIiwidCI6Imh0dHBzOi8vdHdpdHRlci5jb20vQUpBWURIQTI3MjUwMDE2IiwiaWciOiJodHRwczovL3d3dy5pbnN0YWdyYW0uY29tL2FqLmVkdS5pbi8iLCJlIjoiYWpheWRoYW5nYXI0OUBnbWFpbC5jb20iLCJnaCI6Imh0dHBzOi8vZ2l0aHViLmNvbS9BamF5LURoYW5nYXIiLCJ0ZyI6Imh0dHBzOi8vdC5tZS9hal96ZXJvX2NvZGluZyIsInciOiIrOTEgNzAyNDU5MjEwNSIsInkiOiJodHRwczovL3d3dy55b3V0dWJlLmNvbS9AQWpheS1EaGFuZ2FyIiwibCI6Imh0dHBzOi8vd3d3LmxpbmtlZGluLmNvbS9pbi9hamF5LWRoYW5nYXItYmI4OWI0MjI3LyIsImxzIjpbeyJsIjoiTXkgV2Vic2l0ZSIsImkiOiJwaDpnbG9iZS1kdW90b25lIiwidSI6Imh0dHBzOi8vYWpheS1kaGFuZ2FyLmdpdGh1Yi5pby9SZXNwb25zaXZlLXBvcnRmb2xpby13ZWJzaXRlLmdpdGh1Yi5pby8jaG9tZSJ9LHsibCI6Ik1lZGl1bSIsImkiOiJhbnQtZGVzaWduOm1lZGl1bS1vdXRsaW5lZCIsInUiOiJodHRwczovL2FqYXlkaGFuZ2FyNDkubWVkaXVtLmNvbS8ifSx7ImwiOiJDU1MgY291cnNlIiwiaSI6Imdyb21tZXQtaWNvbnM6Y3NzMyIsInUiOiJodHRwczovL2dpdGh1Yi5jb20vQWpheS1EaGFuZ2FyL0NTUzMtTWFzdGVyeSJ9LHsibCI6IkRvbmF0ZSBmb3Igb3VyIGNhdXNlIiwiaSI6Imljb25vaXI6ZG9uYXRlIiwidSI6Imh0dHBzOi8vdG9wbWF0ZS5pby9hamF5X2RoYW5nYXIvMTMyMzc1In0seyJsIjoiRG93bmxvYWQgbXkgcmVzdW1lIiwiaSI6InBoOmZpbGUtcGRmIiwidSI6Imh0dHBzOi8vZHJpdmUuZ29vZ2xlLmNvbS9maWxlL2QvMWFEcTdpaExMck1zc3NCYjFHdXdpbVVSenRCMXg5MnFDL3ZpZXcifV19)

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
