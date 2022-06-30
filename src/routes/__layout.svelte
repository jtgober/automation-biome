<script>
  import "../app.css";
  import Button from '$lib/dark-toggle.svelte'
</script>

<header class="top-0 w-screen z-10 ">
  <nav
    class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800"
  >
    <div class="container flex flex-wrap justify-between items-center mx-auto">
      <div class="hidden w-full md:block md:w-auto" id="mobile-menu">
        <ul
          class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium"
        >
          <li>
            <a
              href="/"
              class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700  text-xl"
              aria-current="page">Home</a
            >
          </li>
          <li>
            <a
              href="/about"
              class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700 text-xl"
              >About</a
            >
          </li>
          <li>
            <a
              href="/guides"
              class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700 text-xl"
              >Services</a
            >
          </li>
          <li>
            <Button/>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>

<main>
  <slot />
</main>

<footer
  class="p-4 bg-white rounded-lg shadow md:flex md:items-center md:justify-between md:p-6 dark:bg-gray-800 fixed bottom-0 w-screen"
>
  <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
    >© 2022 Created By: Jonathan Gober
  </span>
  <ul
    class="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0"
  >
    <li>
      <a href="/about" class="mr-4 hover:underline md:mr-6 ">About</a>
    </li>
    <li>
      <a href="https://twitter.com/Gojobers" class="hover:underline"
        >Contact @Gojobers</a
      >
    </li>
  </ul>
</footer>
<style>
	:root{
		--bg-color: #FFFFFF;
		--text-color: #000000;
	}
	
	:global(body) {
		background: var(--bg-color);
		color: var(--text-color);
	}
	
	:global(body.dark) {
		--bg-color: #000000;
		--text-color: #FFFFFF;
	}
</style>