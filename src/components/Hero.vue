<template>
  <section class="max-w-7xl mx-auto px-6 py-16 md:py-24">
    <div class="grid md:grid-cols-2 gap-12 items-center">
      <div>
        <h1
          class="font-display font-bold text-5xl md:text-6xl leading-tight text-dark"
        >
          Route every AI request <br />
          to the <span class="highlight">right model</span>, <br />
          for the right need
        </h1>
        <p class="mt-6 text-gray-600 max-w-md leading-relaxed">
          GreenLLM is the routing layer for enterprise AI. We help teams adopt
          AI faster by automatically choosing the best model for each task based
          on performance, energy and cost — without changing existing workflows.
        </p>
        <a
          href="#contact"
          class="inline-block mt-8 bg-dark text-white px-6 py-3 rounded-full text-sm hover:opacity-90 transition"
        >
          Get early access
        </a>
      </div>

      <div class="relative flex items-center justify-center">
        <svg
          viewBox="0 0 400 400"
          class="w-full max-w-md"
          xmlns="http://www.w3.org/2000/svg"
        >
          <ellipse
            cx="200"
            cy="200"
            rx="170"
            ry="60"
            fill="none"
            stroke="#0E0E0E"
            stroke-width="1"
            transform="rotate(-20 200 200)"
          />
          <ellipse
            cx="200"
            cy="200"
            rx="170"
            ry="60"
            fill="none"
            stroke="#0E0E0E"
            stroke-width="1"
            transform="rotate(20 200 200)"
          />
          <circle cx="120" cy="130" r="22" fill="#C6F84E" />
          <text
            x="120"
            y="136"
            text-anchor="middle"
            font-size="14"
            font-weight="bold"
          >
            App
          </text>
          <circle cx="190" cy="110" r="22" fill="#0E0E0E" />
          <text
            x="190"
            y="116"
            text-anchor="middle"
            font-size="12"
            fill="white"
          >
            Jira
          </text>
          <circle cx="290" cy="160" r="22" fill="#0E0E0E" />
          <text
            x="290"
            y="166"
            text-anchor="middle"
            font-size="11"
            fill="white"
          >
            Slack
          </text>
          <circle cx="310" cy="230" r="22" fill="#C6F84E" />
          <text
            x="310"
            y="236"
            text-anchor="middle"
            font-size="11"
            font-weight="bold"
          >
            LLM
          </text>
          <circle cx="240" cy="290" r="22" fill="#0E0E0E" />
          <text
            x="240"
            y="296"
            text-anchor="middle"
            font-size="11"
            fill="white"
          >
            API
          </text>
          <polygon
            points="180,200 220,200 200,170 200,230"
            fill="#C6F84E"
            stroke="#0E0E0E"
            stroke-width="2"
          />
          <text x="50" y="260" font-size="12">Request →</text>
          <polygon points="100,300 110,320 120,300 110,280" fill="#0E0E0E" />
        </svg>
      </div>
    </div>
  </section>
</template>