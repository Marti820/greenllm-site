<template>
  <section id="contact" class="max-w-7xl mx-auto px-6 py-16">
    <div class="flex items-end gap-4 mb-10 flex-wrap">
      <h2 class="font-display font-bold text-3xl">
        <span class="highlight">Contact Us</span>
      </h2>
      <p class="text-gray-500 text-sm mb-2">
        Tell us about your workflows and we’ll show you how to route them better
      </p>
    </div>

    <div class="bg-soft rounded-3xl p-8 md:p-12 grid md:grid-cols-2 gap-8">
      <form
        action="https://formspree.io/f/mbdbqakl"
        method="POST"
        class="space-y-4"
      >
        <div class="flex gap-6 mb-4">
          <label class="flex items-center gap-2 cursor-pointer">
            <input
              type="radio"
              name="type"
              value="hi"
              class="accent-lime"
              checked
            />
            <span class="text-sm">Say Hi</span>
          </label>

          <label class="flex items-center gap-2 cursor-pointer">
            <input
              type="radio"
              name="type"
              value="demo"
              class="accent-lime"
            />
            <span class="text-sm">Request a Demo</span>
          </label>
        </div>

        <div>
          <label class="text-sm font-medium block mb-1">Name</label>
          <input
            name="name"
            type="text"
            placeholder="Name"
            class="w-full px-4 py-3 rounded-lg border border-gray-300 bg-white focus:outline-none focus:border-dark text-sm"
          />
        </div>

        <div>
          <label class="text-sm font-medium block mb-1">Email*</label>
          <input
            name="email"
            type="email"
            required
            placeholder="Email"
            class="w-full px-4 py-3 rounded-lg border border-gray-300 bg-white focus:outline-none focus:border-dark text-sm"
          />
        </div>

        <div>
          <label class="text-sm font-medium block mb-1">Message*</label>
          <textarea
            name="message"
            required
            rows="5"
            placeholder="Tell us about your use case, stack, or AI workflow"
            class="w-full px-4 py-3 rounded-lg border border-gray-300 bg-white focus:outline-none focus:border-dark text-sm resize-none"
          ></textarea>
        </div>

        <input
          type="hidden"
          name="_subject"
          value="New GreenLLM contact form submission"
        />

        <button
          type="submit"
          class="w-full bg-dark text-white py-3 rounded-lg text-sm hover:opacity-90"
        >
          Send Message
        </button>
      </form>

      <div class="hidden md:flex items-center justify-center">
        <svg viewBox="0 0 300 300" class="w-full max-w-sm">
          <g stroke="#0E0E0E" stroke-width="1">
            <line x1="150" y1="40" x2="150" y2="20" />
            <line x1="150" y1="260" x2="150" y2="280" />
            <line x1="40" y1="150" x2="20" y2="150" />
            <line x1="260" y1="150" x2="280" y2="150" />
            <line x1="80" y1="80" x2="60" y2="60" />
            <line x1="220" y1="220" x2="240" y2="240" />
            <line x1="80" y1="220" x2="60" y2="240" />
            <line x1="220" y1="80" x2="240" y2="60" />
          </g>
          <polygon
            points="150,80 175,150 150,220 125,150"
            fill="#0E0E0E"
          />
          <polygon
            points="130,170 140,200 110,200 90,210 110,220 90,240 130,225 140,255 150,225 170,235 160,215 180,210 160,200"
            fill="#C6F84E"
          />
        </svg>
      </div>
    </div>
  </section>
</template>