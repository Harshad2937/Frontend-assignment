<template>
  <header class="bg-white border-b">
    <div
      class="max-w-7xl mx-auto px-4 h-72px
             flex items-center justify-between"
    >

      <!-- LOGO -->
      <div class="flex items-center gap-2">
        <!-- Logo icon (simple house shape) -->
        <div
          class="w-8 h-8 bg-[#0A5FD8]
                 text-white flex items-center justify-center
                 rounded-sm font-bold text-lg">
          H
        </div>
        <span class="text-2xl font-bold text-[#0A5FD8]">
          Houzeo
        </span>
      </div>

      <!-- NAV -->
      <nav
        class="hidden lg:flex items-center gap-7
               text-sm font-medium text-gray-700"
      >
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Product ▾
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          How Houzeo Works
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Reviews
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Buy ▾
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Sell ▾
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Pricing
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Resources ▾
        </span>
        <span class="cursor-pointer hover:text-[#0A5FD8]">
          Sign In
        </span>
      </nav>

      <!-- RIGHT -->
      <div class="flex items-center gap-5">
        <div class="hidden md:block text-right">
          <div class="text-sm font-semibold text-gray-900">
            (844) 448-0110
          </div>
          <div class="text-xs text-gray-500">
            (9am to 6pm CST, Mon–Sat)
          </div>
        </div>

        <button
          class="bg-[#0A5FD8] hover:bg-[#084fb5]
                 text-white px-5 py-2.5
                 rounded-md text-sm font-semibold
                 transition"
        >
          Start Free Listing
        </button>
      </div>

    </div>
  </header>
</template>
