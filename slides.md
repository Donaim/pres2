---
title: Browser-Delivered Scientific Instruments
theme: seriph
info: |
  ## Browser-Delivered Scientific Instruments
  WebAssembly makes the browser a practical packaging target for some local, confidential, computational lab tools.
class: text-left
drawings:
  persist: true
mdc: true
zoom: 1.0
hideInToc: true
---

<div class="pt-16">
  <div class="uppercase tracking-widest text-sm opacity-60">Lab software delivery</div>
  <h1 style="font-size: 2.8em; line-height: 1.05; margin-top: 0.4rem; max-width: 38rem;">
    Browser-Delivered<br>Scientific Instruments
  </h1>
  <p style="font-size: 1.15em; max-width: 36rem; margin-top: 1.3rem; line-height: 1.35;">
    WebAssembly makes the browser a practical packaging target for some local, confidential, computational lab tools.
  </p>
</div>

<div class="absolute bottom-8 left-0 right-0 grid grid-cols-3 gap-4 text-center text-sm opacity-75">
  <div>Packaging first</div>
  <div>Confidential data stays local</div>
  <div>Real compute core in browser</div>
</div>

---

## The real bottleneck is packaging

<div class="grid grid-cols-2 gap-8 pt-6">
<div>

- ReCall works on specific setups
- Dependencies drift across machines
- Internal tools never spread cleanly
- Confidential data must stay local

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(153,27,27,0.08); border: 1px solid rgba(153,27,27,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Main point</div>
<div class="text-2xl leading-tight">
For lab software, packaging and data handling often block adoption before the algorithm even matters.
</div>
</div>
</div>

---

## Three places lab software can run

<div class="grid grid-cols-3 gap-4 pt-6 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">Native install</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Example</div>
<div class="text-lg mb-4">ReCall</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Compute</div>
<div class="mb-4">User machine</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Data</div>
<div class="mb-4">Local</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Packaging problem</div>
<div>Per-machine setup drift</div>
</div>

<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">Central server</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Example</div>
<div class="text-lg mb-4">QAI</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Compute</div>
<div class="mb-4">Central service</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Data</div>
<div class="mb-4">Uploaded or centralized</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Tradeoff</div>
<div>One environment, more ops</div>
</div>

<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(8,145,178,0.18); background: rgba(8,145,178,0.07);">
<div class="text-xl font-bold mb-3">Browser client</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Example</div>
<div class="text-lg mb-4">CFEIntact demo</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Compute</div>
<div class="mb-4">User machine, in browser</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Data</div>
<div class="mb-4">Local files and browser storage</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-2">Packaging benefit</div>
<div>Zero-install by URL</div>
</div>
</div>

---

## Why not just use an online tool?

<div class="grid grid-cols-2 gap-8 pt-8">
<div>

- Some sequence data should not leave the machine
- Third-party upload is often unacceptable
- Even internal servers move data centrally
- Local execution can be the right model

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(8,145,178,0.08); border: 1px solid rgba(8,145,178,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Why browser delivery matters</div>
<div class="text-2xl leading-tight">
The browser can make distribution easy without forcing confidential data onto someone else’s server.
</div>
</div>
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN: permission-based file access; OPFS origin-private local storage</div>

---

## Why the browser is now usable for real tools

<div class="grid grid-cols-4 gap-4 pt-8 text-center">
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Input</div>
<div class="text-lg font-bold">User-mediated file access</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Compute</div>
<div class="text-lg font-bold">Workers in the background</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Delivery</div>
<div class="text-lg font-bold">Service worker caching</div>
</div>
<div class="rounded-2xl px-4 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Working data</div>
<div class="text-lg font-bold">OPFS local storage</div>
</div>
</div>

<div class="pt-8 text-xl" style="max-width: 42rem;">
That is enough browser capability to support real local workflows, not just forms and dashboards.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN: Web Workers, Service Workers, File System API, OPFS</div>

---

## Why WebAssembly matters

<div class="grid grid-cols-2 gap-4 pt-8 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Compile existing C/C++/Rust-style cores</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Keep JavaScript for interface</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Keep Wasm for the engine</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Ship one browser-delivered artifact</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
Wasm complements JavaScript. It gives serious compute code a browser target instead of forcing a front-end rewrite.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN WebAssembly: low-level compilation target alongside JavaScript</div>

---

## What kinds of biology tools benefit most

<div class="grid grid-cols-2 gap-4 pt-6 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">FASTQ or QC viewer</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Resistance or defect review tool</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Sample sheet validator</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Consensus or annotation explorer</div>
<div class="rounded-2xl px-4 py-5 col-span-2" style="border: 1px solid rgba(15,23,42,0.14);">Phylogeny, coverage, or result viewer with local computation</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(21,128,61,0.07); border: 1px solid rgba(21,128,61,0.18);">
Good fit when the compute core is real, the packaging pain is high, and the data should stay local.
</div>

---

## Browser-delivered scientific instrument

<div class="grid grid-cols-4 gap-3 pt-10 text-center text-sm font-bold">
  <div class="rounded-xl px-3 py-5" style="background: rgba(15,23,42,0.05); border: 1px solid rgba(15,23,42,0.12);">Local files</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
  <div class="rounded-xl px-3 py-5" style="background: rgba(8,145,178,0.08); border: 1px solid rgba(8,145,178,0.18);">Browser UI</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
</div>

<div class="grid grid-cols-3 gap-3 pt-3 text-center text-sm font-bold">
  <div class="rounded-xl px-3 py-5" style="background: rgba(8,145,178,0.10); border: 1px solid rgba(8,145,178,0.20);">Wasm engine</div>
  <div class="flex items-center justify-center text-2xl opacity-50">→</div>
  <div class="rounded-xl px-3 py-5" style="background: rgba(21,128,61,0.08); border: 1px solid rgba(21,128,61,0.18);">Results and plots</div>
</div>

<div class="grid grid-cols-3 gap-4 pt-10 text-center">
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Data stays local</div>
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Interface and engine separate</div>
  <div class="rounded-xl px-3 py-4" style="border: 1px solid rgba(15,23,42,0.12);">Tool arrives by URL</div>
</div>

---

## CFEIntact as a concrete example

<div class="grid grid-cols-2 gap-8 pt-6 items-start">
<div>
<img src="./assets/cfeintactdocs.png" style="border-radius: 18px; border: 1px solid rgba(15,23,42,0.14); box-shadow: 0 12px 28px rgba(0,0,0,0.14);">
</div>
<div>

- Delivered by URL
- Keeps files on the user side
- Reuses a serious compute core
- Shows the model is practical

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
The point is not only that one tool runs in a browser. The point is that this becomes a plausible packaging model for similar lab tools.
</div>

</div>
</div>

---

## Closing claim

<div class="pt-12 text-4xl leading-tight" style="max-width: 48rem;">
The browser is becoming the easiest way to distribute some serious lab tools without giving up local execution.
</div>

<div class="pt-10 text-2xl leading-snug" style="max-width: 44rem;">
WebAssembly is what makes that practical for tools whose compute core is real and whose data should stay local.
</div>
