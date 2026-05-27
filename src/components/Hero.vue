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
          on performance, cost, and estimated carbon impact — without changing
          existing workflows.
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
         viewBox="0 0 580 430"
         class="w-full max-w-2xl overflow-visible"
         xmlns="http://www.w3.org/2000/svg"
         aria-labelledby="routing-diagram-title"
         role="img"
       >
         <title id="routing-diagram-title">
           GreenLLM routes each request to the best model
         </title>
     
         <defs>
           <marker
             id="arrow"
             markerWidth="12"
             markerHeight="12"
             refX="10"
             refY="6"
             orient="auto"
             markerUnits="strokeWidth"
           >
             <path d="M 0 0 L 12 6 L 0 12 z" fill="#0E0E0E" />
           </marker>
     
           <filter
             id="soft-shadow"
             x="-60%"
             y="-60%"
             width="220%"
             height="220%"
             color-interpolation-filters="sRGB"
           >
             <feDropShadow
               dx="0"
               dy="12"
               stdDeviation="16"
               flood-color="#0E0E0E"
               flood-opacity="0.12"
             />
           </filter>
     
           <filter
             id="soft-green-glow"
             x="-80%"
             y="-80%"
             width="260%"
             height="260%"
             color-interpolation-filters="sRGB"
           >
             <feDropShadow
               dx="0"
               dy="0"
               stdDeviation="22"
               flood-color="#C6F84E"
               flood-opacity="0.38"
             />
           </filter>
     
           <radialGradient id="router-glow" cx="50%" cy="50%" r="50%">
             <stop offset="0%" stop-color="#C6F84E" stop-opacity="0.36" />
             <stop offset="72%" stop-color="#C6F84E" stop-opacity="0.08" />
             <stop offset="100%" stop-color="#C6F84E" stop-opacity="0" />
           </radialGradient>
         </defs>
     
         <!-- Decorative background orbits -->
         <ellipse
           cx="278"
           cy="214"
           rx="198"
           ry="84"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="1.2"
           stroke-opacity="0.14"
           transform="rotate(-18 278 214)"
         />
     
         <ellipse
           cx="278"
           cy="214"
           rx="198"
           ry="84"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="1.2"
           stroke-opacity="0.14"
           transform="rotate(18 278 214)"
         />
     
         <!-- Input app -->
         <g filter="url(#soft-shadow)">
           <rect
             x="26"
             y="162"
             width="126"
             height="78"
             rx="26"
             fill="white"
             stroke="#0E0E0E"
             stroke-width="1.6"
           />
     
           <circle cx="64" cy="201" r="18" fill="#C6F84E" />
     
           <text
             x="98"
             y="197"
             font-size="15"
             font-weight="800"
             fill="#0E0E0E"
           >
             App
           </text>
     
           <text x="98" y="216" font-size="11.5" fill="#6B7280">
             Request
           </text>
         </g>
     
         <!-- Request path into router -->
         <path
           d="M 152 202 C 178 202, 202 212, 224 212"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="2.4"
           stroke-linecap="round"
           marker-end="url(#arrow)"
         />
     
         <circle r="5.5" fill="#C6F84E" stroke="#0E0E0E" stroke-width="1.2">
           <animateMotion
             dur="2.6s"
             repeatCount="indefinite"
             path="M 152 202 C 178 202, 202 212, 224 212"
           />
         </circle>
     
         <!-- Router glow -->
         <circle cx="286" cy="214" r="92" fill="url(#router-glow)" />
     
         <!-- Central router -->
         <g filter="url(#soft-green-glow)">
           <circle cx="286" cy="214" r="62" fill="#0E0E0E" />
     
           <circle
             cx="286"
             cy="214"
             r="47"
             fill="none"
             stroke="#C6F84E"
             stroke-width="1.6"
             stroke-dasharray="4 6"
             opacity="0.95"
           >
             <animateTransform
               attributeName="transform"
               type="rotate"
               from="0 286 214"
               to="360 286 214"
               dur="14s"
               repeatCount="indefinite"
             />
           </circle>
     
           <polygon
             points="270,214 298,214 284,187 284,241"
             fill="#C6F84E"
             stroke="white"
             stroke-width="1.8"
           />
         </g>
     
         <text
           x="286"
           y="295"
           text-anchor="middle"
           font-size="13.5"
           font-weight="800"
           fill="#0E0E0E"
         >
           GreenLLM Router
         </text>
     
         <!-- Decision chips -->
         <g filter="url(#soft-shadow)">
           <rect x="206" y="108" width="78" height="31" rx="15.5" fill="#F3F4F6" />
           <text
             x="245"
             y="128"
             text-anchor="middle"
             font-size="10.5"
             font-weight="700"
             fill="#374151"
           >
             Cost
           </text>
     
           <rect x="296" y="92" width="112" height="31" rx="15.5" fill="#F3F4F6" />
           <text
             x="352"
             y="112"
             text-anchor="middle"
             font-size="10.5"
             font-weight="700"
             fill="#374151"
           >
             Performance
           </text>
     
           <rect x="354" y="137" width="82" height="31" rx="15.5" fill="#F3F4F6" />
           <text
             x="395"
             y="157"
             text-anchor="middle"
             font-size="10.5"
             font-weight="700"
             fill="#374151"
           >
             CO₂
           </text>
         </g>
     
         <!-- Top alternative model -->
         <g filter="url(#soft-shadow)">
           <rect
             x="438"
             y="52"
             width="128"
             height="70"
             rx="24"
             fill="white"
             stroke="#0E0E0E"
             stroke-width="1.5"
           />
     
           <circle cx="474" cy="87" r="17" fill="#0E0E0E" />
     
           <text
             x="474"
             y="92"
             text-anchor="middle"
             font-size="10.5"
             font-weight="800"
             fill="white"
           >
             A
           </text>
     
           <text
             x="505"
             y="83"
             font-size="13.5"
             font-weight="800"
             fill="#0E0E0E"
           >
             Fast LLM
           </text>
     
           <text x="505" y="102" font-size="10.5" fill="#6B7280">
             Low latency
           </text>
         </g>
     
         <!-- Selected model -->
         <g filter="url(#soft-shadow)">
           <rect
             x="446"
             y="174"
             width="128"
             height="76"
             rx="24"
             fill="#C6F84E"
             stroke="#0E0E0E"
             stroke-width="2"
           />
     
           <circle cx="482" cy="212" r="17" fill="#0E0E0E" />
     
           <text
             x="482"
             y="217"
             text-anchor="middle"
             font-size="10.5"
             font-weight="800"
             fill="white"
           >
             B
           </text>
     
           <text
             x="514"
             y="207"
             font-size="13.5"
             font-weight="900"
             fill="#0E0E0E"
           >
             Best fit
           </text>
     
           <text x="514" y="226" font-size="10.5" fill="#0E0E0E" opacity="0.76">
             Selected
           </text>
         </g>
     
         <!-- Bottom alternative model -->
         <g filter="url(#soft-shadow)">
           <rect
             x="438"
             y="306"
             width="128"
             height="70"
             rx="24"
             fill="white"
             stroke="#0E0E0E"
             stroke-width="1.5"
           />
     
           <circle cx="474" cy="341" r="17" fill="#0E0E0E" />
     
           <text
             x="474"
             y="346"
             text-anchor="middle"
             font-size="10.5"
             font-weight="800"
             fill="white"
           >
             C
           </text>
     
           <text
             x="505"
             y="337"
             font-size="13.5"
             font-weight="800"
             fill="#0E0E0E"
           >
             Eco LLM
           </text>
     
           <text x="505" y="356" font-size="10.5" fill="#6B7280">
             Low carbon
           </text>
         </g>
     
         <!-- Alternative routes -->
         <path
           d="M 340 193 C 376 142, 402 98, 438 87"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="1.5"
           stroke-linecap="round"
           stroke-dasharray="5 7"
           opacity="0.28"
           marker-end="url(#arrow)"
         />
     
         <path
           d="M 340 235 C 374 286, 402 330, 438 341"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="1.5"
           stroke-linecap="round"
           stroke-dasharray="5 7"
           opacity="0.28"
           marker-end="url(#arrow)"
         />
     
         <!-- Selected route -->
         <path
           d="M 348 214 C 382 214, 414 214, 446 214"
           fill="none"
           stroke="#0E0E0E"
           stroke-width="3.4"
           stroke-linecap="round"
           marker-end="url(#arrow)"
         />
     
         <circle r="5.5" fill="#0E0E0E">
           <animateMotion
             dur="2.6s"
             repeatCount="indefinite"
             path="M 348 214 C 382 214, 414 214, 446 214"
           />
         </circle>
     
         <!-- Selected label -->
         <g filter="url(#soft-shadow)">
           <rect
             x="392"
             y="258"
             width="154"
             height="34"
             rx="17"
             fill="#0E0E0E"
           />
     
           <text
             x="469"
             y="280"
             text-anchor="middle"
             font-size="11.5"
             font-weight="800"
             fill="white"
           >
             Routed to best model
           </text>
         </g>
       </svg>
     </div>
    </div>
  </section>
</template>