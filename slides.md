---
title: Browser-Delivered Scientific Instruments
theme: seriph
info: |
  ## Browser-Delivered Scientific Instruments
  The browser as a credible deployment target for some lab tools
class: text-left
drawings:
  persist: true
mdc: true
zoom: 1.0
hideInToc: true
---

<div class="pt-16">
  <div class="uppercase tracking-widest text-sm opacity-60">Lab software deployment</div>
  <h1 style="font-size: 2.7em; line-height: 1.05; margin-top: 0.4rem;">
    Browser-Delivered<br>Scientific Instruments
  </h1>
  <p style="font-size: 1.15em; max-width: 32rem; margin-top: 1.25rem; line-height: 1.35;">
    The browser has become a credible deployment target for some scientific tools, and WebAssembly is what makes that practical.
  </p>
</div>

<div class="absolute bottom-8 left-0 right-0 grid grid-cols-3 gap-4 text-center text-sm opacity-75">
  <div>Zero-install delivery</div>
  <div>Local-file workflows</div>
  <div>Reusable compute cores</div>
</div>

---

## A familiar lab failure

<div class="grid grid-cols-2 gap-8 pt-6">
<div>

- Tool works on one machine
- Workshop starts with setup delays
- Demo day becomes support triage
- Useful code stays underused

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(153, 27, 27, 0.08); border: 1px solid rgba(153, 27, 27, 0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">The actual problem</div>
<div class="text-2xl leading-tight">
Packaging cost can exceed analysis value.
</div>
</div>
</div>

---

## Three places software can run

<div class="grid grid-cols-3 gap-5 pt-8 text-center">
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">Native install</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-4">Best case</div>
<div class="text-lg">Full local access</div>
<div class="mt-5 text-sm uppercase tracking-widest opacity-60 mb-2">Main cost</div>
<div class="text-lg">Setup drift everywhere</div>
</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">Central server</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-4">Best case</div>
<div class="text-lg">Controlled environment</div>
<div class="mt-5 text-sm uppercase tracking-widest opacity-60 mb-2">Main cost</div>
<div class="text-lg">Shared bottlenecks</div>
</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(8,145,178,0.07);">
<div class="text-xl font-bold mb-3">Browser client</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-4">Best case</div>
<div class="text-lg">Reach by URL</div>
<div class="mt-5 text-sm uppercase tracking-widest opacity-60 mb-2">Main cost</div>
<div class="text-lg">Host constraints</div>
</div>
</div>

<div class="pt-8 text-xl">
The question for this talk is simple: where should this software run?
</div>

---

## CFEIntact in the browser

<div class="grid grid-cols-2 gap-8 pt-4 items-start">
<div>
<img src="./assets/cfeintactdocs.png" style="border-radius: 18px; border: 1px solid rgba(15,23,42,0.14); box-shadow: 0 12px 28px rgba(0,0,0,0.14);">
</div>
<div>
<div class="grid grid-cols-4 gap-2 text-center text-sm font-bold">
  <div class="rounded-xl px-3 py-4" style="background: rgba(15,23,42,0.05); border: 1px solid rgba(15,23,42,0.12);">Local files</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
  <div class="rounded-xl px-3 py-4" style="background: rgba(8,145,178,0.08); border: 1px solid rgba(8,145,178,0.18);">Browser UI</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
</div>
<div class="grid grid-cols-3 gap-2 text-center text-sm font-bold mt-2">
  <div class="rounded-xl px-3 py-4" style="background: rgba(8,145,178,0.10); border: 1px solid rgba(8,145,178,0.20);">Wasm engine</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
  <div class="rounded-xl px-3 py-4" style="background: rgba(21,128,61,0.08); border: 1px solid rgba(21,128,61,0.18);">Results</div>
</div>

<div class="grid grid-cols-3 gap-3 mt-8 text-center">
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Zero-install delivery</div>
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Local core execution</div>
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Interface-engine separation</div>
</div>
</div>
</div>

---

## What this demo proves

<div class="grid grid-cols-2 gap-8 pt-6">
<div class="rounded-2xl px-6 py-6" style="background: rgba(21,128,61,0.07); border: 1px solid rgba(21,128,61,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Proves</div>

- Install friction can disappear
- Local files can stay local
- Useful compute can stay client-side

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(153,27,27,0.07); border: 1px solid rgba(153,27,27,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Does not prove</div>

- Every workload fits browsers
- Servers stop mattering
- Resource limits disappear

</div>
</div>

---

## Why the browser is newly serious

<div class="grid grid-cols-4 gap-4 pt-8 text-center">
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Input</div>
<div class="text-lg font-bold">User-mediated file access</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Compute</div>
<div class="text-lg font-bold">Workers off the main thread</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Delivery</div>
<div class="text-lg font-bold">Caching and offline behavior</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Working data</div>
<div class="text-lg font-bold">OPFS origin-private storage</div>
</div>
</div>

<div class="pt-8 text-xl">
That is a real application host, not just a page renderer.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN: workers, service workers, file access, OPFS</div>

---

## Why Wasm specifically

<div class="grid grid-cols-2 gap-4 pt-8 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">JavaScript already handles most interface work</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Wasm complements JavaScript, not replaces it</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Reuse serious compute cores</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Capabilities come through imports and Web APIs</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
Wasm does not bring arbitrary syscalls. It lets you ship a real engine through the browser without rewriting that engine as front-end code.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN WebAssembly; webassembly.org portability</div>

---

## Where the compute lives

<div class="grid grid-cols-2 gap-8 pt-6">
<div class="rounded-2xl px-6 py-6" style="background: rgba(153,27,27,0.07); border: 1px solid rgba(153,27,27,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Central server</div>

- Everyone hits one runtime
- Traffic spikes hit one queue
- Failures spread across users
- Operations burden grows centrally

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(21,128,61,0.07); border: 1px solid rgba(21,128,61,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Browser client</div>

- Clients contribute CPU and RAM
- Load spreads across users
- Fewer shared failure domains
- Central services become optional

</div>
</div>

<div class="pt-8 text-xl">
Concentrated compute creates concentrated availability risk.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">OWASP denial of service; distributed client load</div>

---

## Which tools fit this model?

<div class="grid grid-cols-2 gap-4 pt-6 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Existing compute core?</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Installation painful today?</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Local files important?</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Moderate memory footprint?</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Fast iteration useful?</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(153,27,27,0.10);">Needs unrestricted POSIX?</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
Mostly yes, and especially no on the last question, means the browser is a serious candidate.
</div>

---

## Real constraints

<div class="grid grid-cols-2 gap-4 pt-6 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Sandboxed host capabilities only</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">File access needs user permission</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Storage quotas and memory ceilings</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Some APIs need secure contexts</div>
<div class="rounded-2xl px-4 py-5 col-span-2" style="border: 1px solid rgba(153,27,27,0.18); background: rgba(153,27,27,0.07);">Threaded shared-memory demos need cross-origin isolation</div>
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">webassembly.org portability; MDN SharedArrayBuffer constraints</div>

---

## Closing claim

<div class="pt-12 text-4xl leading-tight" style="max-width: 48rem;">
For the right classes of scientific tools, the browser is now a credible default candidate.
</div>

<div class="pt-10 text-2xl leading-snug" style="max-width: 44rem;">
WebAssembly makes that practical by letting us deliver a real compute engine through a zero-install interface.
</div>

<div class="pt-10 text-lg opacity-75">
CFEIntact is one example of that shift, not the limit of it.
</div>
