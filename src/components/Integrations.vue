<template>
  <section id="integrations" class="max-w-7xl mx-auto px-6 py-16">
    <div class="flex items-end gap-4 mb-10 flex-wrap">
      <h2 class="font-display font-bold text-3xl">
        <span class="highlight">Integrations</span>
      </h2>
      <p class="text-gray-500 text-sm mb-2">
        Connect GreenLLM to the tools your teams already use
      </p>
    </div>

    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
      <div
        v-for="tool in tools"
        :key="tool"
        class="border border-gray-200 rounded-2xl p-6 flex items-center justify-center text-center hover:border-dark transition aspect-[4/3]"
      >
        <span class="font-display font-semibold text-dark">{{ tool }}</span>
      </div>
    </div>
  </section>
</template>

<script setup>
const tools = [
  "Jira",
  "Confluence",
  "Bitbucket",
  "Slack",
  "Microsoft Teams",
  "Salesforce",
  "Notion",
  "GitHub",
];
</script>