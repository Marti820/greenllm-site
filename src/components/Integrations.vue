<template>
  <section id="how-it-works" class="max-w-7xl mx-auto px-6 py-16">
    <div class="flex items-end gap-4 mb-10 flex-wrap">
      <h2 class="font-display font-bold text-3xl">
        <span class="highlight">How It Works</span>
      </h2>
      <p class="text-gray-500 text-sm mb-2">
        One routing layer between your app and any LLM provider
      </p>
    </div>

    <div class="grid md:grid-cols-3 gap-6">
      <div
        v-for="item in items"
        :key="item.title"
        class="border border-gray-200 rounded-2xl p-6 hover:border-dark transition"
      >
        <div class="text-3xl mb-4">{{ item.icon }}</div>
        <h3 class="font-display font-semibold text-dark text-lg mb-2">
          {{ item.title }}
        </h3>
        <p class="text-sm text-gray-600 leading-relaxed">
          {{ item.desc }}
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
const items = [
  {
    title: "Drop-in API routing",
    desc: "Replace a direct LLM call with GreenLLM and route requests through a single endpoint. Adoption stays simple for existing products and workflows.",
    icon: "🔌",
  },
  {
    title: "Task-based model selection",
    desc: "GreenLLM analyzes the request and chooses the model that best fits the task, instead of defaulting to the largest one every time.",
    icon: "🧠",
  },
  {
    title: "Cost-aware routing",
    desc: "Use premium models only when they are truly needed. Reduce unnecessary inference spend by matching model size to task value.",
    icon: "💸",
  },
  {
    title: "Latency-aware routing",
    desc: "Prioritize faster responses for real-time experiences by steering traffic toward models that meet speed requirements.",
    icon: "⚡",
  },
  {
    title: "Fallback and multi-provider resilience",
    desc: "Route across providers and define fallback paths when a model is unavailable, too slow, or outside your preferred configuration.",
    icon: "🛡️",
  },
  {
    title: "Flexible routing rules",
    desc: "Set preferences around providers, model families, usage limits, or task handling so routing reflects how your product actually needs to operate.",
    icon: "🛣️",
  },
];
</script>