<template>
  <div>
    <div class="gradient-header absolute left-0 top-0 overflow-hidden"></div>
    <!-- Site Header -->
    <ClientOnly>
      <div class="hidden sm:flex">
        <div
          class="px-4 relative group bg-neon h-10 z-99 w-full flex justify-center"
        >
          <a
            href="/changelog/?ref=alert_bar"
            class="relative px-4 py-2.5 leading-none flex items-center divide-x divide-shark-50 font-semibold text-shark-50"
          >
            <span class="pr-4 text-sm">
              ✨ Released v1.3.0, Supporting integrates with Raycast for
              effective tab searching.
            </span>
            <span
              class="pl-4 group-hover:text-white/90 transition duration-500 text-sm"
            >
              See what's new →
            </span>
          </a>
        </div>
      </div>
      <SiteHeader @navto="gotoAnchor">
        <img
          class="bg-grid pointer-events-none hidden sm:block"
          :src="isDark ? '/img/bg_grid_dark.svg' : '/img/bg_grid_light.svg'"
          alt="background grid"
        />
      </SiteHeader>
      <template #fallback>
        <div class="w-full h-16"></div>
      </template>
    </ClientOnly>
    <!-- End Site Header -->

    <!-- Site Hero -->
    <section class="hero relative">
      <div
        class="max-w-screen-xl px-4 py-16 2xl:py-32 mx-auto h-auto lg:flex 2xl:items-center 2xl:h-screen"
      >
        <div class="max-w-[1120px] mx-auto relative h-screen-sm">
          <ClientOnly>
            <svg
              width="1120"
              height="630"
              viewBox="0 0 1120 630"
              xmlns="http://www.w3.org/2000/svg"
              class="hidden lg:block"
              :class="animateClass"
            >
              <g transform="translate(1 1)" fill="none" fill-rule="evenodd">
                <rect
                  :stroke="SVGColor"
                  stroke-width="2"
                  width="1118"
                  height="628"
                  rx="12"
                  class="browser-frame"
                />
                <path
                  d="M1118 39v34H0V39h116c2.387 0 3.676-.948 5.364-2.636A9 9 0 0 0 124 30V12a7 7 0 0 1 7-7h209c3.866 0 6 3.134 6 7v18c0 4.97 5.03 9 10 9h762z"
                  :stroke="SVGColor"
                  stroke-width="2"
                  class="browser-header"
                />
                <path
                  d="M101.5 39H116c2.387 0 3.676-.948 5.364-2.636A9 9 0 0 0 124 30V12a7 7 0 0 1 7-7h209c3.866 0 6 3.134 6 7v18c0 4.97 5.03 9 10 9h416"
                  stroke="#0c98eb"
                  stroke-width="2"
                  class="browser-group-line"
                />
                <rect
                  fill-opacity=".2"
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  x="109"
                  y="44"
                  width="660"
                  height="24"
                  rx="12"
                  class="browser-skeleton"
                />
                <path
                  d="M84 62a5.002 5.002 0 0 0 4.9-4h2.03a7.001 7.001 0 1 1-1.98-5.95L91 50v6h-6l2.535-2.535A5 5 0 1 0 84 62z"
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  class="browser-skeleton"
                />
                <path
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  opacity=".3"
                  d="M52.333 50L51 51.4l4.381 4.6H45v2h10.381L51 62.6l1.333 1.4L59 57z"
                  class="browser-skeleton"
                />
                <path
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  d="M19.667 50L21 51.4 16.619 56H27v2H16.619L21 62.6 19.667 64 13 57z"
                  class="browser-skeleton"
                />
                <g
                  opacity=".4"
                  transform="translate(591.111 16)"
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  class="browser-skeleton"
                >
                  <path
                    d="M163.024 1l-1.172 1.333L164.198 5l-2.346 2.667L163.024 9l2.346-2.667L167.716 9l1.173-1.333L166.543 5l2.346-2.667L167.716 1l-2.346 2.667z"
                  />
                  <rect width="87.963" height="10" rx="5" />
                </g>
                <g
                  opacity=".4"
                  transform="translate(377 16)"
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  class="browser-skeleton"
                >
                  <path
                    d="M163.166 1L162 2.333 164.334 5 162 7.667 163.166 9l2.334-2.667L167.834 9 169 7.667 166.666 5 169 2.333 167.834 1 165.5 3.667z"
                  />
                  <rect width="88" height="10" rx="5" />
                </g>
                <path
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  d="M328.333 17L327 18.333 329.667 21 327 23.667 328.333 25 331 22.333 333.667 25 335 23.667 332.333 21 335 18.333 333.667 17 331 19.667z"
                  class="browser-skeleton"
                />
                <rect
                  :fill="SVGColor"
                  fill-opacity=".6"
                  fill-rule="nonzero"
                  x="133"
                  y="16"
                  width="100"
                  height="10"
                  rx="5"
                  class="browser-skeleton"
                />
                <path
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  d="M788 15h-2v5h-5v2h5v5h2v-5h5v-2h-5z"
                  class="browser-skeleton"
                />
                <circle
                  fill="#0c98eb"
                  cx="109.5"
                  cy="21.5"
                  r="8"
                  class="browser-group-dot"
                />
                <circle
                  fill-opacity=".4"
                  :fill="SVGColor"
                  cx="363.5"
                  cy="20.5"
                  r="8"
                  class="browser-skeleton"
                />
                <circle
                  fill-opacity=".4"
                  :fill="SVGColor"
                  cx="577.5"
                  cy="20.5"
                  r="8"
                  class="browser-skeleton"
                />
                <path
                  :fill="SVGColor"
                  fill-rule="nonzero"
                  d="M772 8h1v26h-1zM557 8h1v26h-1z"
                  class="browser-skeleton"
                />
                <circle
                  :stroke="SVGColor"
                  fill=""
                  cx="24"
                  cy="19"
                  r="5.5"
                  class="browser-right-corner"
                />
                <circle
                  :stroke="SVGColor"
                  fill=""
                  cx="44"
                  cy="19"
                  r="5.5"
                  class="browser-right-corner"
                />
                <circle
                  :stroke="SVGColor"
                  fill=""
                  cx="64"
                  cy="19"
                  r="5.5"
                  class="browser-right-corner"
                />
              </g>
            </svg>
            <template #fallback>
              <!-- this will be rendered on server side -->
              <div class="w-[1120px] h-[630px]"></div>
            </template>
          </ClientOnly>
          <div
            class="max-w-[1120px] mx-auto text-center z-10 absolute left-0 top-0 pt-8 lg:pt-40"
          >
            <h1
              class="relative font-bold tracking-tight space-y-4 text-primary"
              text="5xl sm:5xl md:6xl lg:7xl"
            >
              <p>
                Your <span class="text-neon">all-in-one</span> browser tab/tab
                group manager
              </p>
            </h1>

            <p
              class="max-w-xl mx-auto mt-8 mb-16 text-xl font-medium sm:leading-relaxed sm:text-xl text-secondary"
            >
              <span class="text-neon">One Tab Group</span> is a chromium-based
              extension that allows you to manage your tabs &amp; tab groups in
              one place. One-click to aggregate all tabs &amp; tab groups into
              one session.
            </p>

            <div
              class="flex flex-wrap justify-center items-center sm:space-x-4 flex-col lg:flex-row"
            >
              <a
                class="flex items-center px-6 py-3 mb-4 text-sm font-medium text-white bg-lochmara-500 border border-lochmara-500 rounded-lg sm:w-auto active:text-opacity-75"
                hover="bg-lochmara-400 text-white"
                focus="outline-none ring"
                target="_blank"
                :href="extensionUrl"
              >
                <logos:chrome class="h-5 w-5 mr-2" />
                <span>Add to Chrome</span>
              </a>

              <a
                class="flex items-center px-6 py-3 mb-4 text-sm font-medium text-white bg-lochmara-500 border border-lochmara-500 rounded-lg sm:w-auto active:text-opacity-75"
                hover="bg-lochmara-400 text-white"
                focus="outline-none ring"
                target="_blank"
                href="https://microsoftedge.microsoft.com/addons/detail/one-tab-group-tabtab-g/njmgdlgmnlinpieohfpmiipenmgilpga"
              >
                <logos:microsoft-edge class="h-5 w-5 mr-2" />
                <span>Add to Edge</span>
              </a>

              <a
                class="flex items-center px-6 py-3 mb-4 text-sm font-medium text-white bg-lochmara-500 border border-lochmara-500 rounded-lg sm:w-auto active:text-opacity-75"
                hover="bg-lochmara-400 text-white"
                focus="outline-none ring"
                target="_blank"
                :href="extensionUrl"
              >
                <logos:brave class="h-5 w-5 mr-2" />
                <span>Add to Brave</span>
              </a>
            </div>
          </div>
        </div>

        <div class="absolute inset-0 flex flex-col items-center justify-center">
          <div class="pt-8 z-99">
            <button
              class="relative flex hover:scale-110 active:scale-100 duration-300 h-16 w-16 items-center justify-center transition transform"
              @click="isShowPromoteVideo = true"
            >
              <div
                class="bg-lochmara-500 absolute inset-0 w-full animate-ping-video rounded-full"
              ></div>
              <div
                class="absolute inset-0 w-full rounded-full shadow-xl shadow-black/40 bg-black/80"
              ></div>
              <div class="relative">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="20"
                  height="20"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  fill="currentColor"
                  style=""
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="ml-0.5 text-white"
                >
                  <polygon points="5 3 19 12 5 21 5 3"></polygon>
                </svg>
              </div>
            </button>
          </div>
        </div>
      </div>
    </section>
    <!-- end hero -->

    <!-- video begin -->
    <PromoteVideo
      v-if="isShowPromoteVideo"
      @close="isShowPromoteVideo = false"
    />
    <!-- video end -->

    <!-- sections -->
    <main
      class="max-w-screen-xl lg:mx-auto features space-y-20 pt-20 sm:pt-24 lg:pt-32"
      ref="featureRef"
    >
      <Divider between class="hidden lg:block" />

      <!-- 1. Sync with your open tabs &amp; tab groups-->
      <OneTabDesc left-desc>
        <template #title>
          Your Open Tabs &
          <span class="text-lochmara-500">Tab Groups</span>
          in sync with your browser
        </template>
        <template #description>
          Struggling to find a site among a mass of open tabs in your browser?
          Don't worry, We Provide you Open Tabs Panel offers an easy way to
          manage multiple tabs at once, in sync with your browser.
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_01.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider right />

      <!-- 2. Save/Restore/Reorganise tabs, even tab groups -->
      <OneTabDesc>
        <template #title>
          Save/Restore Tabs &
          <span class="text-lochmara-500">Tab Groups</span>
        </template>
        <template #description>
          One-click to aggregate all tabs &amp; tab groups into one session. You
          can restore all your tabs &amp; tab groups later as they are. Also you
          can reorganise the session and restore it with ease.
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_02.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider left />

      <!-- 3. Organise tabs & tab groups efficiently -->
      <OneTabDesc left-desc>
        <template #title>
          Organise tabs &amp;
          <span class="text-lochmara-500">tab groups</span> efficiently
        </template>
        <template #description>
          You can drag &amp; drop tabs/tab groups in your sessions to
          reorder/organise them.
          <p>Also could drag the open tabs/tab groups into the sessions.</p>
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_03.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider right />

      <!-- 4. Explore the tabs using the command palette-->
      <OneTabDesc>
        <template #title>
          Explore the tabs using the
          <span class="text-neon">command palette</span>
        </template>
        <template #description>
          With the Command Palette (CMD + K), you can easily switch、 search
          your open tabs in seconds with the command menu. Even you can drill
          down to find out tab in the tab groups
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_04.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider left />

      <!-- 5. Never miss your tabs &amp; tab groups -->
      <OneTabDesc left-desc>
        <template #title>
          Never miss your tabs &amp;
          <span class="text-lochmara-500">tab groups</span>
        </template>
        <template #description>
          You can export the sessions into a JSON file, and import back to
          <span class="text-neon">One Tab Group</span> later.
          <p>
            Also could import from <em>One</em>Tab/Session Buddy's exported
            data.
          </p>
          <p>
            Or Upgrade to Pro to access the sync to cloud、sync to Notion
            feature.
          </p>
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_05.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider right />

      <!-- 6. Turn any tab as a visual web bookmark -->
      <OneTabDesc>
        <template #title>
          Turn any tab into a
          <span class="text-neon">visual web bookmark</span>
        </template>
        <template #description>
          By hovering over the tab in the session, you can use the link as a
          <span class="text-neon">visual web bookmark</span>, like a Twitter
          card or Notion web bookmark. You can preview the website via the
          information like a website's title, description, logo, author,
          thumbnails.
        </template>
        <template #media>
          <img
            class="rounded-lg shadow-lg border-shark-50 mx-auto sm:mx-0 w-full h-full"
            src="/feature_06.gif"
            alt="site feature"
          />
        </template>
      </OneTabDesc>

      <Divider between />

      <!-- 7. supercharge features -->
      <section class="relative text-shark-900 dark:text-white">
        <div class="max-w-screen-xl px-4 py-16 mx-auto sm:px-6 lg:px-8">
          <div class="max-w-lg mx-auto text-center">
            <h2 class="text-3xl font-bold sm:text-4xl">
              <span class="text-neon">Supercharge</span> your tab/tab group
              mangement for Chrome
            </h2>

            <p class="mt-4 text-shark-700 dark:text-shark-300">
              With 30+ useful features built in, you can explore it for free
            </p>
          </div>

          <div
            class="grid grid-cols-1 gap-8 mt-8 md:grid-cols-2 lg:grid-cols-3"
          >
            <OneTabFeature
              title="Restore all your tabs"
              desc="We provide two ways to restore your tabs, one is by drag&drop
              open tabs into session, the other is by click the extension icon."
            >
              <template #icon>
                <bx:bx-window-open class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Restore tabs in new window"
              desc="We also support restoring the session or tabs/tab groups in new
              window."
            >
              <template #icon>
                <mdi:open-in-new class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Sharing tab/tab groups with others"
              desc="By sign-in, you can share any session with others via a web link."
            >
              <template #icon>
                <mdi:share-variant-outline class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Restore tabs with group"
              desc="Restore tabs with group is a core feature in this extension, enjoy
              it."
            >
              <template #icon>
                <bx:bx-windows class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Create a new group"
              desc="Create a new group in the session to manage your tabs, and
              restore them with tab group mode."
            >
              <template #icon>
                <mdi:group class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Ungroup"
              desc="Ungroup a tab group with ease, or drag&drop any tabs outside tab group."
            >
              <template #icon>
                <mdi:ungroup class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Search Tabs"
              desc="Find any saved tabs in milliseconds with a fuzzy search."
            >
              <template #icon>
                <carbon:search class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Suspend Tabs"
              desc="Suspend opened tabs, or open suspended tabs with ease, It can save a ton of memory."
            >
              <template #icon>
                <carbon:clean class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="De-duplicate Tabs"
              desc="De-duplicate opened/saved tabs in session, keep your session clean"
            >
              <template #icon>
                <mdi:delete-sweep-outline class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Dark mode"
              desc="Dark mode builtin, provide you with a dark mode experience."
            >
              <template #icon>
                <carbon:moon class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature title="i18n support" desc="English / Chinese Ready.">
              <template #icon>
                <carbon:language class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <OneTabFeature
              title="Keyboard shortcuts"
              desc="Within the Command K interface, we provide keyboard shortcuts for
              some feature, like toggle Dark Mode."
            >
              <template #icon>
                <carbon:keyboard class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>

            <div></div>
            <OneTabFeature title="More Features" desc="Keep buiding...">
              <template #icon>
                <carbon:strawberry class="h-8 w-8 text-lochmara-500" />
              </template>
            </OneTabFeature>
            <div></div>
          </div>
        </div>
        <img
          class="bg-glow pointer-events-none hidden sm:block !max-w-screen-xl"
          :src="isDark ? '/img/bg_glow_dark.svg' : '/img/bg_glow_light.svg'"
          alt="background glow"
        />
      </section>

      <Divider between />

      <Testimonial />

      <Divider between />

      <div ref="faqsRef">
        <FAQ />
      </div>

      <Divider between />

      <!-- 8. Ready to get started? -->
      <section class="my-16 mx-auto px-8">
        <div
          class="bg-point relative px-8 py-16 mx-auto sm:px-6 lg:px-8 flex flex-col justify-center items-center rounded-lg"
        >
          <div
            class="text-5xl text-shark-200 dark:text-shark-900 mb-8 font-semibold"
          >
            Ready to get started?
          </div>
          <p
            class="text-lg pb-8 text-center max-w-3xl mx-auto text-shark-200 dark:text-shark-700 font-medium"
          >
            Manage your tabs &amp; tab groups in one place.
          </p>
          <a
            class="bg-lochmara-500 highlight-white/20 hover:bg-lochmara-400 text-white font-semibold h-12 px-6 rounded-lg flex items-center justify-center sm:w-auto"
            focus="outline-none ring-2 ring-shark-400 ring-offset-2 ring-offset-shark-50"
            dark="bg-shark-900 highlight-white/20 hover:bg-shark-700"
            :href="extensionUrl"
          >
            <carbon:download class="h-5 w-5 mr-2" /> <span>Get extension</span>
          </a>
        </div>
      </section>
    </main>
    <!-- end sections-->

    <!-- footer -->
    <SiteFooter @navto="gotoAnchor" />
    <!--  end footer -->

    <client-only>
      <chatwoot />
    </client-only>
  </div>
</template>

<script lang="ts" setup>
import { computed, ref } from 'vue'
// import { useI18n } from 'vue-i18n'
import { isDark } from '~/composables/useDarkMode'

// const { locale, availableLocales } = useI18n()

const extensionUrl =
  'https://chrome.google.com/webstore/detail/one-tab-group/lajbajamkpmkmldodfbljkjihppdclbm'

const featureRef = ref()
const faqsRef = ref()
const animateClass = ref()
const isShowPromoteVideo = ref(false)
const SVGColor = computed(() => {
  return isDark.value ? '#f6f6f7' : '#1f2023'
})

// const toggleLocales = () => {
//   // change to some real logic
//   const locales = availableLocales
//   console.log(locale.value)
//   locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
// }

definePageMeta({
  layout: false
})

const gotoAnchor = (anchorEl: string) => {
  let el = null

  if (anchorEl === 'features') {
    el = featureRef.value
  }
  if (anchorEl === 'faqs') {
    el = faqsRef.value
  }

  if (el) {
    el.scrollIntoView({
      behavior: 'smooth',
      inline: 'nearest'
    })
  }
}
setTimeout(() => {
  animateClass.value = 'animate-offset'
}, 333)
</script>

<style scoped>
.bg-point {
  background-image: radial-gradient(#0c98eb 1px, #1f2023 1px);
  background-size: 20px 20px;
}

.dark .bg-point {
  background-image: radial-gradient(#0b446f 1px, #f6f6f7 1px);
}

.gradient-header {
  width: 100vw;
  height: 33vh;
  background-image: linear-gradient(
    180deg,
    hsl(208, 100%, 97%) 80px,
    hsl(240, 6%, 97%) 33vh
  );
}

.dark .gradient-header {
  background-image: linear-gradient(
    180deg,
    hsl(228, 5%, 19%) 80px,
    hsl(225, 6%, 13%) 33vh
  );
}

.bg-grid {
  position: absolute;
  left: 0;
  top: 0;
  width: 100vw;
  z-index: 0;
}

.bg-glow {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 200%;
  max-width: none;
  height: auto;
  z-index: 0;
  transform: translate(-50%, -50%);
}

.chrome-frame {
  transform: translate(-50%, -50%);
}

.browser-frame {
  stroke-dashoffset: 3500px;
  stroke-dasharray: 3500px;
  transition: stroke-dashoffset 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 0s;
}

.browser-header {
  stroke-dashoffset: 2400px;
  stroke-dasharray: 2400px;
  transition: stroke-dashoffset 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 0.125s;
}

.browser-group-line {
  stroke-dashoffset: 2400px;
  stroke-dasharray: 2400px;
  transition: stroke-dashoffset 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 1.2s;
}

.browser-right-corner {
  stroke-dashoffset: 36px;
  stroke-dasharray: 36px;
  transition: stroke-dashoffset 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 0.75s;
}

.browser-group-dot {
  fill: transparent;
  transition: fill 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 1.2s;
}

.browser-skeleton {
  fill: transparent;
  transition: fill 1s cubic-bezier(0.66, 0.72, 0.04, 0.86) 0.375s;
}

svg.animate-offset .browser-frame,
svg.animate-offset .browser-header,
svg.animate-offset .browser-group-line,
svg.animate-offset .browser-right-corner {
  stroke-dashoffset: 0;
}

.dark svg.animate-offset .browser-skeleton {
  fill: #f6f6f7;
}
svg.animate-offset .browser-skeleton {
  fill: #1f2023;
}

svg.animate-offset .browser-group-dot {
  fill: #0c98e9;
}

.gradient-shadow {
  box-shadow: 0 10px 24px 0 hsla(202, 90%, 48%, 0.33),
    0 -10px 24px 0 hsla(202, 90%, 48%, 0.33);
}

.animate-ping-video {
  animation: ping 2.5s cubic-bezier(0, 0, 0.2, 1) infinite;
}

@keyframes ping {
  0% {
    -webkit-transform: scale(1);
    transform: scale(1);
    opacity: 1;
  }
  75%,
  100% {
    -webkit-transform: scale(2);
    transform: scale(2);
    opacity: 0;
  }
}
@-webkit-keyframes ping {
  0% {
    -webkit-transform: scale(1);
    transform: scale(1);
    opacity: 1;
  }
  75%,
  100% {
    -webkit-transform: scale(2);
    transform: scale(2);
    opacity: 0;
  }
}
</style>
