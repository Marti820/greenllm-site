<template>
  <section id="use-cases" class="max-w-7xl mx-auto px-6 py-16">
    <div class="flex items-end gap-4 mb-10 flex-wrap">
      <h2 class="font-display font-bold text-3xl">
        <span class="highlight">Use Cases</span>
      </h2>
      <p class="text-gray-500 text-sm mb-2">
        Real examples of how teams route AI to the right model for the job
      </p>
    </div>

    <div class="bg-dark text-white rounded-3xl p-10 md:p-12">
      <div class="grid md:grid-cols-3 gap-10 divide-y md:divide-y-0 md:divide-x divide-gray-700">
        <div
          v-for="(uc, i) in useCases"
          :key="i"
          class="pt-6 md:pt-0 md:px-6 first:md:pl-0 last:md:pr-0"
        >
          <h3 class="font-display font-semibold text-lg mb-3">
            {{ uc.title }}
          </h3>
          <p class="text-gray-300 text-sm leading-relaxed">
            {{ uc.desc }}
          </p>
          <a
            href="#contact"
            class="inline-flex items-center gap-1 text-lime mt-4 text-sm hover:underline"
          >
            Learn more ↗
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const useCases = [
  {
    title: "Route simple tasks to lighter models",
    desc: "Summaries, classification, extraction, and internal drafting do not need your most expensive model. GreenLLM detects the task and routes it to a faster, lower-cost option automatically.",
  },
  {
    title: "Keep premium models for high-value work",
    desc: "Use stronger models only when the task actually requires deeper reasoning, better accuracy, or richer output quality. This keeps performance high without overspending on every request.",
  },
  {
    title: "Adopt AI faster across your stack",
    desc: "Connect tools like Slack, Jira, Confluence, and your internal apps through one routing layer. Teams get one simple entry point, while you stay flexible behind the scenes.",
  },
];
</script>