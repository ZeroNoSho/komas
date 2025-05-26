<template>
  <nav
    class="border border-[#795548] px-2 sm:px-10 py-4 rounded-b bg-[#795548] shadow"
  >
    <div class="container flex flex-wrap justify-between items-center mx-auto">
      <NuxtLink to="/" class="flex items-center">
        <span
          class="self-center text-xl font-semibold whitespace-nowrap text-white"
        >
          RT 01 RW 03 KARANGPUCUNG
        </span>
      </NuxtLink>

      <div class="flex items-center">
        <button
          id="menu-toggle"
          type="button"
          class="inline-flex items-center p-2 ml-3 text-sm text-gray-500 rounded-lg hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 md:hidden"
        >
          <span class="sr-only">Open main menu</span>
          <svg
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16m-7 6h7"
            />
          </svg>
        </button>
      </div>

      <div class="w-full md:block md:w-auto hidden" id="mobile-menu">
        <ul
          class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium"
        >
          <li>
            <NuxtLink
              to="/"
              :exact-active-class="'text-white'"
              class="block py-2 pr-4 pl-3 text-gray-300 hover:text-white md:p-0"
            >
              Home
            </NuxtLink>
          </li>
          <li>
            <NuxtLink
              to="/dokumentasi"
              :exact-active-class="'text-white'"
              class="block py-2 pr-4 pl-3 text-gray-300 hover:text-white md:p-0"
            >
              Dokumentasi
            </NuxtLink>
          </li>
          <li>
            <NuxtLink
              to="/bagan"
              :exact-active-class="'text-white'"
              class="block py-2 pr-4 pl-3 text-gray-300 hover:text-white md:p-0"
            >
              Bagan RT
            </NuxtLink>
          </li>
          <li>
            <NuxtLink
              to="/lokasi"
              :exact-active-class="'text-white'"
              class="block py-2 pr-4 pl-3 text-gray-300 hover:text-white md:p-0"
            >
              Lokasi
            </NuxtLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
