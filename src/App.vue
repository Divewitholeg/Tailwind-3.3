<template>
  <div class="wheelsBackground">
    <h1>Tailwind 3.3 - more colors, TypeScript friendly</h1>
    <p>
      Get ready to spice up your web development game with the latest release of Tailwind CSS v3.3!
      This update brings a deliciously extended color palette to satisfy even the most discerning
      designer's cravings. But that's not all - feast your eyes on the new ESM/TS support that'll
      make your workflow smoother than butter. And, as if that weren't enough, you can now indulge
      in the savory goodness of logical properties and other mouth-watering features that'll take
      your website to the next level. Don't miss out on this delectable upgrade - your taste buds
      (and clients) will thank you!
    </p>
    <p>First thing let's upgrade the existing version of Tailwind for the latest one:</p>
    <pre>npm install -D tailwindcss@latest</pre>
    <p>
      Darker <span class="font-bold text-slate-950">-950 shades</span> are now added for every
      color:
    </p>
    <pre>&lt;span class="font-bold text-slate-950">-950 shades&lt;/span></pre>
    <p>With the new version you can generate a TS (or ESM) config file</p>
    <pre>npx tailwindcss init --ts</pre>
    <p>
      For those using RTL and LTR language options life becomes easier with `ms-3` (margin start)
      and `me-3` (margin end) tags. Same properties were added to start-*, end-*, padding, rounded,
      border and scroll.
    </p>
    <div class="m-10 group flex items-center">
      <div class="me-3">
        <p class="text-sm font-medium text-slate-700">أوليج ريبنيكوف</p>
        <p class="text-sm font-medium text-slate-500">مطور ويب</p>
      </div>
      <img
        class="shrink-0 h-12 w-12 rounded-full"
        src="@/assets/Oleg.jpg"
        alt="Oleg Rõbnikov Web Development logo"
      />

      <div class="ms-3">
        <p class="text-sm font-medium text-slate-700">Oleg Rõbnikov</p>
        <p class="text-sm font-medium text-slate-500">Web developer</p>
      </div>
    </div>

    <pre>
&lt;div class="group flex items-center"&gt;
    &lt;div class="me-3"&gt;
      &lt;p class="text-sm font-medium text-slate-700"&gt;أوليج ريبنيكوف&lt;/p&gt;
      &lt;p class="text-sm font-medium text-slate-500"&gt;مطور ويب&lt;/p&gt;
    &lt;/div&gt;
    &lt;img
      class="shrink-0 h-12 w-12 rounded-full"
      src="@/assets/Oleg.jpg"
      alt="Oleg Rõbnikov Web Development logo"
    /&gt;

    &lt;div class="ms-3"&gt;
      &lt;p class="text-sm font-medium text-slate-700"&gt;Oleg Rõbnikov&lt;/p&gt;
      &lt;p class="text-sm font-medium text-slate-500"&gt;Web developer&lt;/p&gt;
    &lt;/div&gt;
  &lt;/div&gt;</pre
    >
    <p>
      New controls were added to make gradient stop positions more precise with `from-10%`,
      `via-35%`, etc. You can find more information about new features of color gradient stops in
      <a href="https://tailwindcss.com/docs/gradient-color-stops#specifying-stop-positions"
        >documentation</a
      >
    </p>
    <div
      class="m-10 bg-gradient-to-r from-rose-400 from-30% via-fuchsia-500 via-60% to-indigo-500 to-90% h-10 w-300"
    ></div>
    <pre>
 class="bg-gradient-to-r from-rose-400 from-30% via-fuchsia-500 via-60% to-indigo-500 to-90% h-10 w-300" </pre
    >
    <p>
      Line-clamp isn't used as a plugin anymore. You can just use it as, e.g. `line-clamp-2` class!
    </p>
    <p class="line-clamp-2">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Omnis, beatae itaque laudantium est
      quaerat tempora maxime adipisci quod minus inventore nihil non in, iste, ab aperiam illum.
      Minus, molestias excepturi! Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro
      voluptates vitae sunt molestiae esse. Eius aliquam suscipit nostrum temporibus libero sit
      laboriosam recusandae aperiam ut obcaecati blanditiis, similique vel minima. Lorem ipsum dolor
      sit amet consectetur, adipisicing elit. Recusandae voluptatum dicta reprehenderit debitis fuga
      veritatis praesentium vero eius. A cumque nesciunt aliquam aut tempora quasi modi quae ipsam
      officia corporis.
    </p>

    <p>
      Line-height and font-size have been combined into a single class, e.g. 'font-lg/7' and also
      supports arbitrary values like 'font-xl/[17]'
    </p>
    <p
      style="--brandColor: #e500ff; --hoverBrandColor: #000000"
      class="text-[--brandColor] hover:text-[--hoverBrandColor]"
    >
      Color variables are now supported in the class arguments without `var` prefix. Try to hover
      over me!
    </p>
    <pre>
style="--brandColor: #e500ff; --hoverBrandColor: #000000"
class="text-[--brandColor] hover:text-[--hoverBrandColor]"</pre
    >
    <p>
      In conclusion, Tailwind CSS version 3.3 has numerous new features like a redesigned docs site,
      CSS Grid support, and the ability to customize the font families used in your project. The
      update also includes numerous bug fixes and performance improvements. If you're a web
      developer looking to streamline your workflow and build beautiful, responsive websites faster
      than ever, give Tailwind CSS a try and experiment with these new features today!
    </p>
  </div>
</template>
