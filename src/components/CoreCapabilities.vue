<template>
  <section id="product" class="max-w-7xl mx-auto px-6 py-16">
    <div class="flex items-end gap-4 mb-12 flex-wrap">
      <h2 class="font-display font-bold text-3xl">
        <span class="highlight">Product: Core Capabilities</span>
      </h2>
      <p class="text-gray-500 text-sm mb-2">
        What teams can do with GreenLLM
      </p>
    </div>

    <div class="grid md:grid-cols-2 gap-6">
      <div
        v-for="(item, i) in items"
        :key="i"
        class="card"
        :class="item.bg"
      >
        <div class="max-w-[55%]">
          <h3 class="highlight font-display font-bold text-lg leading-tight">
            {{ item.title }}
          </h3>
          <p
            class="mt-4 text-sm leading-relaxed"
            :class="item.dark ? 'text-gray-300' : 'text-gray-600'"
          >
            {{ item.desc }}
          </p>
        </div>
        <div class="text-4xl opacity-80">{{ item.icon }}</div>
      </div>
    </div>
  </section>
</template>

<script setup>
const items = [
  {
    title: "Smart Model Routing",
    desc: "Automatically choose the best model for each request based on task type, response quality needs, speed, and cost.",
    icon: "🧠",
    bg: "bg-soft",
    dark: false,
  },
  {
    title: "Easy Adoption Across Teams",
    desc: "Give product, ops, and internal teams one simple AI entry point without forcing them to learn model selection or prompt infrastructure.",
    icon: "⚡",
    bg: "bg-lime",
    dark: false,
  },
  {
    title: "Works With Your Existing Stack",
    desc: "Connect GreenLLM to the tools and workflows you already use, from internal apps to collaboration platforms and enterprise software.",
    icon: "🔗",
    bg: "bg-dark text-white",
    dark: true,
  },
  {
    title: "Control Cost Without Slowing Teams Down",
    desc: "Stop sending every request to the most expensive model. Right-size inference automatically and keep premium models for premium tasks.",
    icon: "💸",
    bg: "bg-soft",
    dark: false,
  },
  {
    title: "Flexible Routing Rules",
    desc: "Set routing logic around your priorities, whether that means lower cost, faster replies, model preference, or infrastructure constraints.",
    icon: "🛣️",
    bg: "bg-lime",
    dark: false,
  },
  {
    title: "Usage Visibility",
    desc: "See how AI is being used across teams, which models are selected most often, and where routing creates the biggest gains.",
    icon: "📈",
    bg: "bg-dark text-white",
    dark: true,
  },
];
</script>