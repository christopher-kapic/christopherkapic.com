<script lang="ts">
  import { settings } from "../settings";
</script>

<div class="flex space-x-2 lg:space-x-4 justify-center text-gray-300">
  {#if settings.facebook}
    <a href={settings.facebook || "https://facebook.com"} name="Facebook"
    class="text-blue-600 transition hover:text-white"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="feather feather-facebook"
        ><path
          d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"
        /></svg
      >
    </a>
  {/if}
  {#if settings.instagram}
    <a href={settings.instagram || "https://instagram.com"} name="Instagram"
    class="text-orange-400 transition hover:text-white"
    >
      <svg
        viewBox="0 0 24 24"
        width="24"
        height="24"
        stroke="currentColor"
        stroke-width="2"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="css-i6dzq1"
        ><rect x="2" y="2" width="20" height="20" rx="5" ry="5" /><path
          d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"
        /><line x1="17.5" y1="6.5" x2="17.51" y2="6.5" /></svg
      >
    </a>
  {/if}
  {#if settings.twitter}
    <a
      href={settings.twitter || "https://twitter.com/kapicode"}
      name="Twitter"
      class="text-blue-400 transition hover:text-white"
    >
      <svg
        viewBox="0 0 24 24"
        width="24"
        height="24"
        stroke="currentColor"
        stroke-width="2"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="css-i6dzq1"
        ><path
          d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"
        /></svg
      >
    </a>
  {/if}
  {#if settings.github}
    <a
      href={settings.github || "https://github.com/christopher-kapic"}
      name="Github"
      class="text-green-400 transition hover:text-white"
    >
      <svg
        viewBox="0 0 24 24"
        width="24"
        height="24"
        stroke="currentColor"
        stroke-width="2"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="css-i6dzq1"
        ><path
          d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"
        /></svg
      >
    </a>
  {/if}
</div>
