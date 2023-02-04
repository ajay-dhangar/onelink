<template>
  <div class="h-screen grid grid-cols-3 divide-x">
    <div class="col-span-2 h-screen flex flex-col bg-slate-100">
      <div class="flex-1 overflow-y-auto p-8">
        <app-form-profile
          v-model:name="data.n"
          v-model:desc="data.d"
          v-model:image="data.i"
        />
        <app-form-hr />
        <app-form-social-links
          v-model:facebook="data.f"
          v-model:twitter="data.t"
          v-model:instagram="data.ig"
          v-model:github="data.gh"
          v-model:telegram="data.tg"
          v-model:linkedin="data.l"
          v-model:email="data.e"
          v-model:whatsapp="data.w"
          v-model:youtube="data.y"
        />
        <app-form-hr />
        <app-form-links v-model="data.ls" />
      </div>
      <div class="border-t bg-white flex items-center">
        <button
          @click="prefillDemoData"
          class="h-12 flex items-center space-x-2 px-4 border-r text-xs font-medium bg-white text-slate-700"
        >
          <span> Add demo data </span>
          <icon name="mdi:code-json" class="h-4 w-4" />
        </button>
        <button
          @click="publish"
          class="h-12 flex items-center space-x-2 px-4 border-r text-xs font-medium bg-white text-slate-700"
        >
          <span> Publish </span>
          <icon name="ph:paper-plane-tilt-bold" class="h-4 w-4" />
        </button>
        <a
          href="https://github.com/Ajay-Dhangar/onelink"
          target="_blank"
          class="h-12 flex items-center space-x-2 px-4 border-r text-xs font-medium bg-white text-slate-700"
        >
          <span> Github </span>
          <icon name="mdi:github" class="h-4 w-4" />
        </a>
      </div>
    </div>
    <app-form-preview :data="data" />
    <a
      href="https://www.linkedin.com/in/ajay-dhangar-bb89b4227/"
      target="_blank"
      class="absolute bottom-0 right-0 bg-white rounded-tl-lg shadow px-4 py-1 font-medium text-sm text-gray-500"
    >
      Made by Ajay Dhangar 
    </a>
  </div>
</template>

<script setup>
import { encodeData } from "../utils/transformer";
const data = ref({
  n: "",
  d: "",
  i: "",
  f: "",
  t: "",
  ig: "",
  gh: "",
  tg: "",
  l: "",
  e: "",
  w: "",
  y: "",
  ls: [],
});

const prefillDemoData = () => {
  data.value = {
    n: "Ajay Dhangar",
    d: "I’m Web Developer, YouTuber, and Learner.",
    i: "https://avatars.githubusercontent.com/u/99037494?v=4",
    f: "https://www.facebook.com/profile.php?id=100078316657152",
    t: "https://twitter.com/AJAYDHA27250016",
    ig: "https://www.instagram.com/aj.edu.in/",
    e: "ajaydhangar49@gmail.com",
    gh: "https://github.com/Ajay-Dhangar",
    tg: "https://t.me/aj_zero_coding",
    w: "+91 7024592105",
    y: "https://www.youtube.com/@Ajay-Dhangar",
    l: "https://www.linkedin.com/in/ajay-dhangar-bb89b4227/",
    ls: [
      {
        l: "My Website",
        i: "ph:globe-duotone",
        u: "https://ajay-dhangar.github.io/Responsive-portfolio-website.github.io/#home",
      },
      {
        l: "Medium",
        i: "ant-design:medium-outlined",
        u: "https://ajaydhangar49.medium.com/",
      },
      {
        l: "CSS course",
        i: "grommet-icons:css3",
        u: "https://github.com/Ajay-Dhangar/CSS3-Mastery",
      },
      {
        l: "Donate for our cause",
        i: "iconoir:donate",
        u: "https://topmate.io/ajay_dhangar/132375",
      },
      {
        l: "Download my resume",
        i: "ph:file-pdf",
        u: "https://drive.google.com/file/d/1aDq7ihLLrMsssBb1GuwimURztB1x92qC/view",
      },
    ],
  };
};

const publish = () => {
  const url = `${window.location.origin}/1?data=${encodeData(data.value)}`;
  navigator.clipboard.writeText(url).then(() => {
    alert("Link copied to clipboard");
  });
};
</script>
