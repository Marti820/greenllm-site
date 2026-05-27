<template>
  <footer class="max-w-7xl mx-auto px-6 pb-10">
    <div class="flex items-center gap-2 mb-6">
      <div
        class="w-8 h-8 rounded-md bg-lime flex items-center justify-center"
      >
        <span class="text-dark font-bold text-sm">G</span>
      </div>
      <span class="font-display font-bold text-dark text-lg">GreenLLM</span>
    </div>

    <div class="bg-dark text-white rounded-3xl p-10">
      <div
        class="flex flex-col md:flex-row md:items-center justify-between gap-6 mb-10 pb-6 border-b border-gray-800"
      >
        <ul class="flex flex-wrap gap-6 text-sm">
          <li><a href="#product" class="hover:text-lime">Product</a></li>
          <li><a href="#use-cases" class="hover:text-lime">Use Cases</a></li>
          <li><a href="#how-it-works" class="hover:text-lime">How It Works</a></li>
          <li><a href="#contact" class="hover:text-lime">Contact</a></li>
        </ul>
        <div class="flex gap-3">
        </div>
      </div>

      <div class="grid md:grid-cols-2 gap-8">
        <div>
          <span class="highlight font-display font-bold mb-4 inline-block"
            >Contact us:</span
          >
          <div class="text-sm space-y-2 mt-4 text-gray-300">
            <p>Email: jjosediazzzz@gmail.com</p>
            <p>Location: Lyon - France</p>
          </div>
        </div>

        <div class="bg-[#1a1a1a] rounded-2xl p-6 flex items-center">
          <form
            action="https://formspree.io/f/mbdbqakl"
            method="POST"
            class="flex gap-2 w-full"
          >
            <input
              type="email"
              name="email"
              placeholder="Email"
              required
              class="flex-1 bg-transparent border border-gray-700 rounded-lg px-4 py-2 text-sm focus:outline-none focus:border-lime"
            />
            <input
              type="hidden"
              name="_subject"
              value="New GreenLLM newsletter signup"
            />
            <button
              type="submit"
              class="bg-lime text-dark px-5 py-2 rounded-lg text-sm font-medium hover:opacity-90"
            >
              Subscribe
            </button>
          </form>
        </div>
      </div>

      <div
        class="mt-10 pt-6 border-t border-gray-800 flex flex-col md:flex-row justify-between gap-4 text-xs text-gray-400"
      >
        <p>© 2026 GreenLLM. All Rights Reserved.</p>
      </div>
    </div>
  </footer>
</template>