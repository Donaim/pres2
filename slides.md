---
title: Browser-Delivered Scientific Instruments
theme: seriph
info: |
  ## Browser-Delivered Scientific Instruments
  Biology software has a distribution problem; the browser has tried to solve it for decades, and WebAssembly is the missing piece for some local computational tools.
class: text-left
drawings:
  persist: true
mdc: true
zoom: 1.0
hideInToc: true
---

<div class="pt-16">
  <div class="uppercase tracking-widest text-sm opacity-60">Biology software distribution</div>
  <h1 style="font-size: 2.75em; line-height: 1.05; margin-top: 0.4rem; max-width: 40rem;">
    Browser-Delivered<br>Scientific Instruments
  </h1>
  <p style="font-size: 1.15em; max-width: 39rem; margin-top: 1.3rem; line-height: 1.35;">
    Biology software has a distribution problem; the browser has tried to solve it for decades, and WebAssembly is the missing piece for some local computational tools.
  </p>
</div>

<div class="absolute bottom-8 left-0 right-0 grid grid-cols-3 gap-4 text-center text-sm opacity-75">
  <div>Packaging pain</div>
  <div>Browser history</div>
  <div>Local scientific tools</div>
</div>

---

## Why is biology software still awkward to distribute?

<div class="grid grid-cols-2 gap-10 pt-8">
<div>

- Native installs drift by machine
- Internal tools spread badly
- Confidential data complicates hosting

</div>
<div class="rounded-2xl px-6 py-6" style="background: rgba(153,27,27,0.08); border: 1px solid rgba(153,27,27,0.18);">
<div class="text-sm uppercase tracking-widest opacity-65 mb-3">Premise</div>
<div class="text-2xl leading-tight">
In biology, the bottleneck is often distribution, not the algorithm.
</div>
</div>
</div>

---

## Three deployment models in our world

| Model | Who installs it? | Where does data go? | Where does compute run? |
| --- | --- | --- | --- |
| ReCall | User or local lab IT | Local machine | Local machine |
| QAI | Central team | Centralized service | Central server |
| Browser-delivered client | Nobody beyond opening a URL | Local files and browser storage | User machine in browser |

<div class="pt-8 text-xl" style="max-width: 44rem;">
Most tools get pushed into the first two boxes. The opportunity is when the third box becomes the better answer.
</div>

---

## The web kept trying to become an application platform

<div class="grid grid-cols-4 gap-4 pt-8 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Plug-ins</div>
<div class="text-lg font-bold mb-3">Java applets<br>and Flash</div>
<div class="text-sm">Rich software, weak future</div>
</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Faster JavaScript</div>
<div class="text-lg font-bold mb-3">asm.js</div>
<div class="text-sm">Useful stopgap, now deprecated</div>
</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Browser-specific native</div>
<div class="text-lg font-bold mb-3">NaCl</div>
<div class="text-sm">Powerful, but not cross-browser</div>
</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(8,145,178,0.18); background: rgba(8,145,178,0.07);">
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Portable standard</div>
<div class="text-lg font-bold mb-3">WebAssembly</div>
<div class="text-sm">W3C Recommendation in 2019</div>
</div>
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">Oracle JDK migration guide; asm.js deprecated in favor of Wasm; NaCl deprecated as Wasm matured</div>

---

## Biology already trusts serious browser software

<div class="grid grid-cols-3 gap-5 pt-8 text-center">
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">Galaxy</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">What it proves</div>
<div class="text-lg">Web-based biomedical research can be serious software.</div>
</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14); background: rgba(15,23,42,0.04);">
<div class="text-xl font-bold mb-3">JBrowse</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">What it proves</div>
<div class="text-lg">Browser-native genome exploration can stand on its own.</div>
</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(8,145,178,0.18); background: rgba(8,145,178,0.07);">
<div class="text-xl font-bold mb-3">IGV-Web</div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">What it proves</div>
<div class="text-lg">Local-file viewing in the browser is already legitimate.</div>
</div>
</div>

<div class="pt-8 text-xl" style="max-width: 45rem;">
The browser already won credibility for visualization and access. The missing question was compute.
</div>

---

## What was still missing before Wasm

<div class="grid grid-cols-2 gap-10 pt-8">
<div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Already good</div>

- Interfaces
- Visualization
- URL-based delivery

</div>
<div>
<div class="text-sm uppercase tracking-widest opacity-60 mb-3">Still awkward</div>

- Reusing compute cores
- Shipping real engines locally
- Avoiding full front-end rewrites

</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(153,27,27,0.07); border: 1px solid rgba(153,27,27,0.18);">
"Just rewrite it in JavaScript" is not a satisfying packaging strategy for serious lab software.
</div>

---

## Why WebAssembly matters for lab software

<div class="grid grid-cols-3 gap-4 pt-8 text-center">
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14);">Old compute cores can travel into the browser</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14);">Zero-install delivery no longer means server-side execution</div>
<div class="rounded-2xl px-5 py-6" style="border: 1px solid rgba(15,23,42,0.14);">The browser becomes a packaging target, not just a viewer</div>
</div>

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
Wasm complements JavaScript by giving C, C++, and Rust-style code a portable browser target.
</div>

<div class="absolute bottom-4 right-6 text-xs opacity-60">MDN WebAssembly concepts; MDN Web Workers and browser capability model</div>

---

## Plausible next instruments for our lab

<div class="grid grid-cols-2 gap-4 pt-6 text-center">
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Local sequence QC viewer</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Resistance interpretation assistant</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Coverage and mutation explorer</div>
<div class="rounded-2xl px-4 py-5" style="border: 1px solid rgba(15,23,42,0.14);">Run-validation or sample-sheet checker</div>
<div class="rounded-2xl px-4 py-5 col-span-2" style="border: 1px solid rgba(15,23,42,0.14);">Contamination, primer-mismatch, or result-review tool with local compute</div>
</div>

<div class="mt-8 text-xl" style="max-width: 44rem;">
These are not generic web apps. They are browser-delivered lab instruments.
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
  <div class="rounded-xl px-3 py-5" style="background: rgba(21,128,61,0.08); border: 1px solid rgba(21,128,61,0.18);">Results and visualization</div>
</div>

---

## CFEIntact demo

<div class="grid grid-cols-2 gap-8 pt-8 items-start">
<div>
<img src="./assets/cfeintactdocs.png" style="border-radius: 18px; border: 1px solid rgba(15,23,42,0.14); box-shadow: 0 12px 28px rgba(0,0,0,0.14);">
</div>
<div>

- A real lab tool
- Delivered by URL
- Files stay user-side

<div class="mt-8 rounded-2xl px-6 py-5" style="background: rgba(8,145,178,0.07); border: 1px solid rgba(8,145,178,0.18);">
One working example is enough to make the model feel real.
</div>

</div>
</div>

---

## Closing takeaway

<div class="pt-14 text-4xl leading-tight" style="max-width: 48rem;">
The browser is no longer just where we view results.
</div>

<div class="pt-10 text-3xl leading-tight" style="max-width: 48rem;">
For some biology tools, it is becoming the easiest place to deliver the software itself.
</div>
