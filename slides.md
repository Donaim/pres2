---
title: Browser-Delivered Scientific Instruments
theme: seriph
background: ./assets/future.webp
info: |
  ## Browser-Delivered Scientific Instruments
  Why WebAssembly matters for laboratory software distribution
class: text-center
drawings:
  persist: true
mdc: true
zoom: 1.1
hideInToc: true
---

<div class="pt-18">
  <h1 style="font-size: 2.8em; line-height: 1.05; color: white; text-shadow: 0 0 24px rgba(0,0,0,0.45);">
    Browser-Delivered<br>Scientific Instruments
  </h1>
  <p style="font-size: 1.15em; color: rgba(255,255,255,0.9); margin-top: 1.2rem;">
    Why WebAssembly matters for laboratory software distribution
  </p>
</div>

<div class="absolute bottom-6 left-6 text-left" style="color: rgba(255,255,255,0.88); text-shadow: 0 0 18px rgba(0,0,0,0.45);">
  <div><b>14 Apr 2026</b></div>
  <div>Lab software, CFEIntact, and the browser as a runtime</div>
</div>

<!--
This talk is not mainly about Wasm performance.

The claim I want to make is broader: the browser is becoming a serious delivery target for scientific software, and WebAssembly is one of the reasons that is now credible.

CFEIntact is the concrete example, but the bigger point is architectural.
-->

---

## Thesis

<div class="grid grid-cols-2 gap-10 pt-6">
<div>

### The old story

- Deployment bad
- Wasm fast
- Demo works in browser

</div>
<div>

### The stronger story

- The browser is becoming a universal application host
- WebAssembly turns it into a serious distribution target
- CFEIntact is evidence that lab tools can move there

</div>
</div>

<div class="mt-10 rounded-2xl px-6 py-5" style="background: rgba(15, 23, 42, 0.08); border: 1px solid rgba(15, 23, 42, 0.16);">
<b>Core claim:</b> WebAssembly is not mainly about speed. It is about making zero-install delivery plausible for real scientific software.
</div>

<!--
If this were just a speed talk, it would be forgettable.

The more interesting question is whether the browser is now good enough to act as a default delivery vehicle for some classes of scientific tools.
-->

---

## The real problem is distribution

Laboratory software often fails before any algorithm runs.

- Installation docs drift
- Native dependencies break differently on Windows, macOS, and Linux
- IT approval and local admin rights slow everything down
- Workshops and demos become support events
- Small tools never get adopted because setup cost dominates use value

<div class="mt-8 rounded-2xl px-6 py-5" style="background: linear-gradient(90deg, rgba(153,27,27,0.10), rgba(146,64,14,0.10)); border: 1px solid rgba(153,27,27,0.18);">
For many lab tools, <b>deployment friction</b> is a bigger practical problem than algorithmic complexity.
</div>

<!--
Many useful tools are not blocked by math. They are blocked by packaging, install burden, and environment drift.

That is why distribution deserves to be the center of the talk.
-->

---

## Where should scientific software run?

| Model | Strength | Cost |
| --- | --- | --- |
| Native install | Full local power | Setup pain, dependency drift, platform variance |
| Central server | Controlled environment | Queueing, ops burden, chokepoints, data movement |
| Browser client | Zero-install reach | Sandboxed host, feature limits, download budget |

<div class="mt-8">

What changed recently is not that browsers became magical.

What changed is that the third column became technically serious.

</div>

<!--
This slide reframes the question.

We are not comparing Wasm against nothing.
We are comparing three places where scientific software can live, and each one has a distinct operational cost structure.
-->

---

## Browsers are now application hosts

<div class="grid grid-cols-2 gap-10 pt-4">
<div>

### Already available

- Web Workers for background computation
- Service workers for caching and offline behavior
- User-mediated local file access
- OPFS for origin-private storage with file-oriented access

</div>
<div>

<img src="./assets/windowsxp.png" style="border-radius: 18px; border: 1px solid rgba(0,0,0,0.14); box-shadow: 0 12px 28px rgba(0,0,0,0.18);">

</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8, 145, 178, 0.08); border: 1px solid rgba(8, 145, 178, 0.18);">
The browser is no longer just a UI surface. It is a constrained but genuinely capable runtime.
</div>

<div class="absolute bottom-5 right-8 text-sm opacity-70">
MDN: Web Workers, Service Workers, File System API
</div>

<!--
This is the enabling background.

The browser still has limits, but it now has enough runtime features that we can discuss it as a host for real applications, not just forms and dashboards.
-->

---

## Why not just JavaScript?

Modern JavaScript is already fast and highly optimized.

That is not the real objection.

### WebAssembly helps because it gives us:

- A compilation target for existing native-language code
- Cleaner separation: JS for UI, Wasm for computational engine
- Less handwritten porting of core logic into front-end code
- A better migration path for old scientific codebases

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(30, 41, 59, 0.08); border: 1px solid rgba(30, 41, 59, 0.16);">
Wasm complements JavaScript. The value is not only execution speed. The value is packaging, portability, and reuse.
</div>

<div class="absolute bottom-5 right-8 text-sm opacity-70">
MDN: WebAssembly is a complement to JavaScript
</div>

<!--
I do not want to oversell a false JS-versus-Wasm conflict.

The better framing is that Wasm is what lets us keep a serious compute core while using the web stack for delivery and interface.
-->

---

## The politics of compute

<div class="grid grid-cols-2 gap-10 pt-4">
<div class="rounded-2xl px-6 py-5" style="background: rgba(153, 27, 27, 0.08); border: 1px solid rgba(153, 27, 27, 0.18);">

### Server-centric model

- Institution owns the compute
- Central infrastructure becomes the bottleneck
- Workshops, demos, and traffic spikes hit one chokepoint
- Operations burden grows with popularity

</div>
<div class="rounded-2xl px-6 py-5" style="background: rgba(21, 128, 61, 0.08); border: 1px solid rgba(21, 128, 61, 0.18);">

### Browser-side model

- Users contribute their own CPU and RAM
- Load is spread across clients
- No single analysis queue for every interaction
- Central services become optional, not mandatory

</div>
</div>

<div class="mt-8 text-xl">
Client-side compute is not just a performance trick. It is an architectural redistribution of responsibility.
</div>

<!--
This is where the DoS point expands into something broader.

Centralized compute is not only vulnerable to malicious load. It is also vulnerable to success.
-->

---

## Reproducibility and data locality

<div class="grid grid-cols-2 gap-10 pt-4">
<div>

### Better deployment reproducibility

- One versioned artifact
- Stable runtime surface inside the browser
- Fewer host-specific surprises
- Less "your Python or libfoo is different"

</div>
<div>

### Better privacy posture for some workflows

- Open local files directly
- Compute locally
- Avoid unnecessary uploads
- Keep working data in browser-managed storage

</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: linear-gradient(90deg, rgba(8,145,178,0.08), rgba(21,128,61,0.08)); border: 1px solid rgba(8,145,178,0.18);">
Containers helped standardize deployment for servers. Browser-delivered Wasm can help standardize deployment for end users.
</div>

<!--
This is not perfect scientific reproducibility.
It is specifically deployment reproducibility.

That distinction matters, but even that narrower improvement is valuable in practice.
-->

---

## New packaging target for old code

The pitch to labs does not have to be "rewrite everything for the web."

It can be:

- Keep an existing computational core
- Compile that core to WebAssembly
- Put a zero-install interface around it
- Deliver by URL instead of platform-specific installer

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(99, 102, 241, 0.08); border: 1px solid rgba(99, 102, 241, 0.18);">
Wasm is a migration path for legacy scientific code, not just a bet on greenfield software.
</div>

<div class="absolute bottom-5 right-8 text-sm opacity-70">
webassembly.org: high-level goals and use cases emphasize portability and tooling
</div>

<!--
This is where the talk becomes practical.

If the audience hears "new paradigm," they may tune out.
If they hear "new packaging target for code you already have," that is much easier to act on.
-->

---
layout: image-right
image: ./assets/cfeintactdocs.png
---

## CFEIntact as proof

This is the point where the talk becomes concrete.

### CFEIntact in the browser is not just a demo

- It shows a real lab tool can be delivered without local installation
- It preserves a separation between interface and computational engine
- It suggests a category, not a one-off stunt

### Better interpretation

**CFEIntact in the browser is evidence that some lab software can move from installed application or backend service to portable client-side instrument.**

<!--
I do not want the audience to see CFEIntact and conclude only that one program was ported.

The stronger conclusion is that this is evidence for a broader architectural option.
-->

---

## Browser-delivered scientific instrument

<div class="grid grid-cols-3 gap-6 pt-6 text-center">
<div class="rounded-2xl px-5 py-6" style="background: rgba(30, 41, 59, 0.06); border: 1px solid rgba(30, 41, 59, 0.14);">
<div class="text-xl font-bold mb-2">Interface</div>
<div>Rich browser UI</div>
</div>
<div class="rounded-2xl px-5 py-6" style="background: rgba(8, 145, 178, 0.08); border: 1px solid rgba(8, 145, 178, 0.18);">
<div class="text-xl font-bold mb-2">Engine</div>
<div>Wasm-compiled compute core</div>
</div>
<div class="rounded-2xl px-5 py-6" style="background: rgba(21, 128, 61, 0.08); border: 1px solid rgba(21, 128, 61, 0.18);">
<div class="text-xl font-bold mb-2">Data</div>
<div>Local files, OPFS, optional network services</div>
</div>
</div>

<div class="mt-10 text-2xl text-center">
Zero-install. Immediate by URL. Local compute. Local files. Network only when useful.
</div>

<!--
"Web app" is too weak a phrase.

"Interactive instrument" is better because it emphasizes readiness, direct manipulation, and practical utility.
-->

---

## What kinds of tools move next?

Good candidates usually have most of these properties:

- Compute-heavy core but moderate memory footprint
- High pain from local installation or training setup
- Strong value from local-file workflows
- Need for responsive visualization or iteration
- Existing C, C++, or Rust-friendly core logic

Examples:

- Sequence QC and filtering viewers
- Resistance or defect interpretation tools
- Alignment and annotation assistants
- Cohort exploration dashboards with local computation

<!--
This is where the talk opens outward again.

CFEIntact matters because it helps us recognize a broader class of software that might benefit from the same distribution model.
-->

---

## What Wasm does not solve

To keep this credible, we need the limits slide.

- Browser Wasm is still inside a browser sandbox
- There is no arbitrary POSIX access in the browser
- Local file access is permission-mediated
- Browser storage is quota-constrained
- Some features depend on secure contexts
- Download size and startup time still matter
- Heavy workloads can still hit browser memory and performance ceilings

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(153, 27, 27, 0.08); border: 1px solid rgba(153, 27, 27, 0.18);">
Wasm is not "native binaries, but magically in a tab." It only has the capabilities the host exposes.
</div>

<div class="absolute bottom-5 right-8 text-sm opacity-70">
webassembly.org: portability and host capability model
</div>

<!--
This slide improves trust.

The goal is not to sound evangelical. The goal is to define the real design space.
-->

---

## Closing question

<div class="text-3xl leading-tight pt-12">
The interesting question is not whether WebAssembly is fast.
</div>

<div class="text-4xl leading-tight pt-8 font-bold" style="color: #0f766e;">
It is whether the browser is now good enough to become the default delivery vehicle for some scientific tools.
</div>

<div class="pt-12 text-xl">
CFEIntact suggests the answer may already be "yes" for more software than we used to think.
</div>

<!--
The ending should land on the architectural question, not on the implementation detail.
-->

---

## Sources

- MDN Web Workers API: https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API
- MDN File System API: https://developer.mozilla.org/en-US/docs/Web/API/File_System_API
- MDN WebAssembly concepts: https://developer.mozilla.org/en-US/docs/WebAssembly/Guides/Concepts
- WebAssembly high-level goals: https://webassembly.org/docs/high-level-goals/
- WebAssembly use cases: https://webassembly.org/docs/use-cases/
- WebAssembly portability: https://webassembly.org/docs/portability/

Thank you.
