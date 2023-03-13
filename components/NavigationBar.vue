<template>
  <section>

    <header class="text-gray-600 body-font">
      <div class="mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center">
        <a href="#" class="flex items-center">
          <img src="https://logosandtypes.com/wp-content/uploads/2022/09/apollo-io.svg" class="h-6 mr-3 sm:h-9" />
        </a>
        <nav
          class="md:mr-auto md:ml-4 md:py-1 md:pl-4 md:border-l md:border-gray-400	flex flex-wrap items-center text-base justify-center">
          <button type="button" class="flex mr-5 hover:text-gray-900" @mouseover="toggleDropdown()" @mouseleave="showDropdown = false">
            <svg class="mr-2" xmlns="http://www.w3.org/2000/svg" width="23" height="23" viewBox="0 0 24 24" fill="none" stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M9 21V9"/></svg>Home</button>
          <a class="flex mr-5 text-blue-400 hover:text-gray-900"><svg aria-hidden="true"
              class="w-6 h-6 mr-2 text-blue-400 dark:text-gray-400" fill="none" stroke="currentColor"
              viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
            </svg>Search</a>
          <button type="button" class="flex mr-5 hover:text-gray-900" @mouseover="toggleDropdown()" @mouseleave="showDropdown = false">
            <svg class="mr-2 mt-0.5" xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>Engage</button>
          <button type="button" class="flex mr-5 hover:text-gray-900" @mouseover="toggleDropdown()" @mouseleave="showDropdown = false">
            <svg class="mr-2 mt-0.5" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21.5 2v6h-6M2.5 22v-6h6M2 11.5a10 10 0 0 1 18.8-4.3M22 12.5a10 10 0 0 1-18.8 4.2"/></svg>Enrich</button>
        </nav>

        <button
          class="inline-flex items-center bg-blue-400 border-0 py-1 px-6 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 text-white mr-3">Upgrade
        </button>
        <div class="relative mr-3">
          <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <svg aria-hidden="true" class="w-5 h-5 text-gray-500 dark:text-gray-400" fill="currentColor"
              viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd"
                d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                clip-rule="evenodd"></path>
            </svg>
          </div>
          <input type="text" id="simple-search"
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-1.5"
            placeholder="Search" required>
        </div>
        <a href="" class="mr-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
            stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path
              d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z">
            </path>
          </svg>
        </a>
        <a href="" class="mr-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
            stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <circle cx="12" cy="12" r="10"></circle>
            <path d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"></path>
            <line x1="12" y1="17" x2="12.01" y2="17"></line>
          </svg>
        </a>
        <a href="" class="mr-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
            stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d="M3 18v-6a9 9 0 0 1 18 0v6"></path>
            <path
              d="M21 19a2 2 0 0 1-2 2h-1a2 2 0 0 1-2-2v-3a2 2 0 0 1 2-2h3zM3 19a2 2 0 0 0 2 2h1a2 2 0 0 0 2-2v-3a2 2 0 0 0-2-2H3z">
            </path>
          </svg>
        </a>
        <a href="" class="mr-3">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
            stroke="#4e4e4e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <circle cx="12" cy="12" r="3"></circle>
            <path
              d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z">
            </path>
          </svg>
        </a>
        <button type="button"
          class=" mr-3 text-sm bg-gray-200 rounded-full md:mr-0 focus:ring-4 focus:ring-gray-300 w-8 h-8">
          AR
        </button>
      </div>

      <div id="mega-menu-full-dropdown"
        class="mt-1 relative w-1/2 border-gray-200 shadow-lg rounded-lg bg-gray-50 md:bg-white border-y"
        :class="{'show':showDropdown,'hidden':!showDropdown}">
        <div class="grid px-4 py-5 text-gray-900 sm:grid-cols-2">
          <ul>
            <li class="flex">
              <img class="w-10 h-10 rounded mr-4 mt-1"
                    src="https://zenprospect-production.s3.amazonaws.com/uploads/pictures/6409fa0ef487b60001823893/picture">
              <a href="#" class="block rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700">
                <div class="font-semibold">Onboarding</div>
                <span class="text-sm font-light text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet consectetur adipisicing</span>
              </a>
            </li>
          </ul>
          <ul>
            <li class="flex">
              <img class="w-10 h-10 rounded mr-4 mt-1"
                    src="https://zenprospect-production.s3.amazonaws.com/uploads/pictures/6409fa0ef487b60001823893/picture">
              <a href="#" class="block rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700">
                <div class="font-semibold">Onboarding <span
                class="inline-flex items-center justify-center px-1 ml-3 text-sm font-medium text-white bg-green-400 rounded dark:bg-gray-700 dark:text-gray-300">New !</span></div>
                <span class="text-sm font-light text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet consectetur adipisicing</span>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </header>
    <nav class="bg-gray-50 dark:bg-gray-700">
      <div class="max-w-screen-xl px-4 py-3 mx-auto md:px-6">
        <div class="flex items-center">
          <ul class="flex flex-row mt-0 mr-6 space-x-8 text-sm font-medium">
            <li>
              <a href="#" class="flex text-gray-900 dark:text-white hover:text-blue-400" aria-current="page">
                <svg aria-hidden="true"
                  class="flex-shrink-0 mr-2 w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd">
                  </path>
                </svg>People</a>
            </li>
            <li>
              <a href="#" class="flex text-blue-400 dark:text-white hover:text-blue-400">
                <svg aria-hidden="true" class="flex-shrink-0 mr-2 w-5 h-5 text-blue-400 transition duration-75 "
                  fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd"
                    d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z"
                    clip-rule="evenodd"></path>
                </svg>Companies</a>
            </li>
            <li>
              <a href="#" class="flex text-gray-900 dark:text-white hover:text-blue-400">
                <svg aria-hidden="true"
                  class="flex-shrink-0 w-5 h-5 mr-2 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                  fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd"
                    d="M5 4a3 3 0 00-3 3v6a3 3 0 003 3h10a3 3 0 003-3V7a3 3 0 00-3-3H5zm-1 9v-1h5v2H5a1 1 0 01-1-1zm7 1h4a1 1 0 001-1v-1h-5v2zm0-4h5V8h-5v2zM9 8H4v2h5V8z"
                    clip-rule="evenodd"></path>
                </svg>List</a>
            </li>
            <li>
              <a href="#" class="flex text-gray-900 dark:text-white hover:text-blue-400">
                <svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-500 dark:text-gray-400" fill="none"
                  stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                </svg>Saved Searches</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        showDropdown: false
      }
    },
    methods: {
      toggleDropdown() {
        this.showDropdown = !this.showDropdown
      }
    }
  }
</script>