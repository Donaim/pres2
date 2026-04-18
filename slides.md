---
title: Братство прямої міри
theme: seriph
info: |
  ## Братство прямої міри
  Розслідування культу вимірюваного.
class: text-left
drawings:
  persist: false
mdc: true
colorSchema: dark
hideInToc: true
---

<style>
  :root {
    --deck-bg: #081018;
    --deck-bg-2: #0e1724;
    --deck-fg: #f3ecdf;
    --deck-muted: #a9b4c5;
    --deck-accent: #d6b25e;
    --deck-accent-2: #79b5a8;
    --deck-danger: #cf785d;
    --deck-line: rgba(243, 236, 223, 0.12);
    --deck-panel: rgba(10, 18, 30, 0.74);
    --deck-panel-soft: rgba(243, 236, 223, 0.06);
  }

  .slidev-layout {
    background:
      radial-gradient(circle at top left, rgba(214, 178, 94, 0.12), transparent 28%),
      radial-gradient(circle at bottom right, rgba(121, 181, 168, 0.1), transparent 26%),
      linear-gradient(180deg, var(--deck-bg-2) 0%, var(--deck-bg) 100%);
    color: var(--deck-fg);
    font-family: "IBM Plex Sans", "Aptos", "Segoe UI", sans-serif;
  }

  .slidev-layout h1,
  .slidev-layout h2,
  .slidev-layout h3,
  .hero-title,
  .section-title,
  .quote-giant {
    font-family: "IBM Plex Serif", "Georgia", serif;
    letter-spacing: -0.03em;
  }

  .panel {
    background: var(--deck-panel);
    border: 1px solid var(--deck-line);
    border-radius: 24px;
    box-shadow: 0 18px 40px rgba(0, 0, 0, 0.22);
  }

  .panel-soft {
    background: var(--deck-panel-soft);
    border: 1px solid var(--deck-line);
    border-radius: 24px;
  }

  .panel-ivory {
    background: linear-gradient(180deg, rgba(246, 239, 227, 0.98), rgba(234, 227, 214, 0.93));
    color: #1b2432;
    border: 1px solid rgba(27, 36, 50, 0.08);
    border-radius: 28px;
    box-shadow: 0 18px 40px rgba(0, 0, 0, 0.2);
  }

  .quote-chip {
    display: block;
    padding: 0.85rem 1rem;
    border-radius: 18px;
    border: 1px solid rgba(243, 236, 223, 0.11);
    background: rgba(7, 13, 22, 0.58);
    line-height: 1.25;
    min-height: 4.4rem;
  }

  .axis-card {
    position: relative;
    overflow: hidden;
    border-radius: 26px;
    border: 1px solid var(--deck-line);
    background: rgba(243, 236, 223, 0.04);
  }

  .mini-chart {
    height: 6.5rem;
    border-radius: 18px;
    border: 1px solid rgba(243, 236, 223, 0.1);
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.04), rgba(255, 255, 255, 0.01));
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .mini-chart svg,
  .spiral svg,
  .circumplex svg,
  .portrait svg {
    width: 100%;
    height: 100%;
  }

  .timeline-node {
    border-radius: 22px;
    border: 1px solid var(--deck-line);
    background: rgba(243, 236, 223, 0.05);
  }

  .timeline-track {
    position: absolute;
    left: 4%;
    right: 4%;
    top: 50%;
    height: 2px;
    background: linear-gradient(90deg, rgba(214, 178, 94, 0.2), rgba(121, 181, 168, 0.4), rgba(214, 178, 94, 0.2));
  }

  .forbidden-label {
    color: var(--deck-danger);
    letter-spacing: 0.14em;
    text-transform: uppercase;
    font-size: 0.72rem;
  }

  .admin-tag {
    padding: 0.7rem 0.9rem;
    border-radius: 14px;
    background: rgba(243, 236, 223, 0.05);
    border: 1px dashed rgba(243, 236, 223, 0.14);
  }

  .void-stamp {
    padding: 0.65rem 0.95rem;
    border-radius: 999px;
    border: 1px solid rgba(207, 120, 93, 0.28);
    color: #f1c6b8;
    background: rgba(207, 120, 93, 0.08);
  }

  .watch {
    width: 15rem;
    height: 15rem;
    border-radius: 3.6rem;
    border: 10px solid #202733;
    background: radial-gradient(circle at top, rgba(121, 181, 168, 0.28), rgba(8, 16, 24, 0.98));
    box-shadow: inset 0 0 0 1px rgba(243, 236, 223, 0.12), 0 24px 48px rgba(0, 0, 0, 0.28);
  }

  .watch-band {
    width: 4.6rem;
    height: 5.5rem;
    background: linear-gradient(180deg, #232c39, #0c1117);
    border-radius: 1.3rem;
  }

  .final-quote {
    font-size: 2.25rem;
    line-height: 1.08;
    max-width: 49rem;
  }

  .data-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.92rem;
  }

  .data-table td,
  .data-table th {
    border-bottom: 1px solid rgba(243, 236, 223, 0.08);
    padding: 0.58rem 0.1rem;
    text-align: left;
  }

  .small-note {
    color: var(--deck-muted);
    font-size: 0.9rem;
    line-height: 1.35;
  }

  .portrait {
    height: 8.6rem;
    border-radius: 22px;
    border: 1px solid rgba(243, 236, 223, 0.12);
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0.02));
    overflow: hidden;
  }
</style>

<!-- Пауза. Картинка з'являється після тексту. Дати аудиторії прочитати перед кліком. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-8 py-8 flex flex-col justify-between">
    <div class="text-2xl leading-snug max-w-3xl mt-8">
      Жив був Прокруст, він мав хату при дорозі.
      До тої хати він запрошував мандрівників переночувати.
      Були в него ліжка, а всі на один розмір.
    </div>
    <v-clicks>
    <div class="panel-soft mt-6 px-6 py-6 text-xl leading-snug">
      Кого тіло було замалим — він розтягував, аж підійде. <br></br>
      Кого завеликим — вкорочував (відрізав кінцівки).
    </div>
    </v-clicks>
  </div>

  <v-clicks class="col-span-2">
  <div class="col-span-2 panel-soft px-6 py-6 flex flex-col justify-between">
    <div style="height: 17rem; overflow: hidden; border-radius: 18px;">
      <img src="./assets/procrustes.png" alt="Прокруст" style="width:100%;height:100%;object-fit:cover;filter:brightness(0.88) contrast(1.1);">
    </div>
    <div class="text-2xl leading-tight mt-6">
      На рано в нього всі ставали одинакові.
    </div>
  </div>
  </v-clicks>
</div>

---

<!-- Ефект кобри — конкретна, весела, легко запам'ятовується. Дати час на кожну плашку. -->

<div class="grid grid-cols-5 gap-4 pt-1 items-stretch" style="height:calc(100% - 0.25rem);">
  <div class="col-span-3 flex flex-col gap-2">
    <div class="panel px-6 py-3 text-xl leading-tight">
      В 18 столітті Британська імперія колонізовувала Індію і зіткнулася з проблемою кобр.
    </div>
    <div class="grid grid-cols-1 gap-2 text-lg" style="flex:1;">
      <div class="panel-soft px-4 py-3">Як горобці китайцям, кобри перешкоджали тодішній короні.</div>
      <div class="panel-soft px-4 py-3">Влада почала скуповувати шкіру кобр.</div>
      <div class="panel-soft px-4 py-3">Люди почали розводити кобр, і здавати їх за винагороду.</div>
      <div class="panel-soft px-4 py-3">Вони самі породили те, що хотіли знищити.</div>
    </div>
  </div>

  <div class="col-span-2 panel-soft overflow-hidden" style="border-radius:24px;">
    <img src="./assets/cobra-india.jpg" alt="Кобра" style="width:100%;height:100%;object-fit:cover;filter:brightness(0.75) contrast(1.1);">
  </div>
</div>

---

<!-- Простий слайд, риторичний. Не пояснювати — просто пройтись по пунктах з паузами. Остання фраза — підвести до питання: але хто це все влаштував? -->

<div class="flex flex-col pt-2" style="height:calc(100% - 0.5rem); gap:0.75rem;">
  <div class="panel-ivory px-8 py-4">
    <h1 class="hero-title text-6xl leading-none">УЯВИ ЩО...</h1>
  </div>
  <div style="flex:1; display:flex; flex-direction:column; gap:0.6rem;">
    <v-clicks>
      <div class="panel px-6 py-3 text-2xl leading-tight">на роботі тобі платять за вклад, а не за години</div>
      <div class="panel px-6 py-3 text-2xl leading-tight">за каву ти платиш на стільки на скільки вона була смачна</div>
      <div class="panel px-6 py-3 text-2xl leading-tight">у школі цінують твоє розуміння, а не зубріння</div>
      <div class="panel px-6 py-3 text-2xl leading-tight">дорожче означає не "статусніше", а справді якісніше</div>
      <div class="panel px-6 py-3 text-2xl leading-tight">країну оцінюють по добробуту людей, а не по GDP</div>
    </v-clicks>
  </div>
</div>

---

<!-- "Чи знайомі тобі такі фрази" — дати людям впізнати себе. Цей слайд — пауза для впізнання. Потім підвести: це не випадкові фрази. -->

<div class="pt-2">
</div>

<div class="grid grid-cols-4 gap-4 mt-8">
  <div class="quote-chip">“Де цифри?”</div>
  <div class="quote-chip">“А на еґзамені то буде?”</div>
  <div class="quote-chip">“Мені не треба красиво, мені треба, шоб робило”</div>
  <div class="quote-chip">“Оцініть свій біль від 0 до 10”</div>
  <div class="quote-chip">“Школа не для того, шоб тобі подобалось”</div>
  <div class="quote-chip">“Дорожче значить ліпше”</div>
  <div class="quote-chip">“Якісне не може бути дешеве”</div>
  <div class="quote-chip">“Може ти й чудова людина, але кредитний скор так не думає”</div>
</div>

<v-clicks>
<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight">
  Чому ми хочемо одного, але говоримо за зовсім інче?
</div>
</v-clicks>

---

<!-- Не директор школи. Не міністр. Не лікар.
А той, хто навчив їх усіх одної й тої самої мови серйозности. -->

<div class="h-full flex flex-col justify-center items-center text-center px-8">
  <div class="hero-title" style="font-size: 5.3rem; line-height: 0.95;">КОМУ ТО ВИГІДНО?</div>

  <v-clicks>
  <div class="panel-soft mt-10 px-8 py-6 text-2xl leading-relaxed max-w-3xl" style="text-align:left;">
    Хто вирішує, що рахується, той вирішує і що існує.
  </div>
  </v-clicks>
</div>
---

<!-- Документальний тон. Без оцінок. Просто факти — хто вони такі. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7 flex flex-col justify-between">
    <h1 class="hero-title text-5xl mt-1 leading-none">ХТО ТАКІ ПІФАГОРІЙЦІ?</h1>
    <div class="mt-5 text-xl leading-snug max-w-2xl">
      VI ст. до н.е., Математик, містик, реформатор
      Піфагор заснував закриту спільноту — зо своїм статутом, ієрархією і таємним знанням.
    </div>
    <br>
    Їхнє кредо:
    <div class="panel-soft mt-5 px-5 py-5 text-2xl leading-tight">
      Число — першопричина всього
    </div>
    <div class="mt-5 text-xl leading-snug">
      Правильна форма — не просто краса. Це модель, якій світ зобов'язаний коритись.
      Все, що відхиляється від форми, — не просто інакше. Воно неправильне.
    </div>
  </div>

  <div class="col-span-2 panel-soft flex flex-col items-center px-5 py-6">
    <div style="flex:1; width:100%; overflow:hidden; border-radius:18px;">
      <img src="./assets/pythagoras.jpg" alt="Піфагор" style="width:100%;height:100%;object-fit:cover;object-position:center top;filter:brightness(0.85) sepia(0.18);">
    </div>
    <div class="text-xl leading-tight mt-4 text-center opacity-70">~570–495 до н.е.</div>
  </div>
</div>

---

<!-- Зараз — сміх, але серйозно. Фасоля — це пуант. Після нього — Прокруст. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7 flex flex-col justify-between">
    <h1 class="hero-title text-5xl mt-1 leading-none">ОЗНАКИ СЕКТИ</h1>
    <div class="grid grid-cols-2 gap-4 mt-6 text-xl">
      <div class="panel-soft px-4 py-4 leading-snug">
        Жорсткий лідерський культ:<br>слово Піфагора — закон <br>
      </div>
      <div class="panel-soft px-4 py-4 leading-snug">
        Заборони: не торкатись білого когута, не їсти з цілого хліба
      </div>
      <div class="panel-soft px-4 py-4 leading-snug">
        Очищення через математику: числа очищують душу <br>
      </div>
      <div class="panel-soft px-4 py-4 leading-snug">
        Нав'язлива любов до форми: правильна геометрія — правильний розум
      </div>
    </div>
  </div>

  <div class="col-span-2 panel-soft flex flex-col items-center px-5 py-6">
    <div style="flex:1; width:100%; overflow:hidden; border-radius:18px;">
      <img src="./assets/bean.png" alt="Піфагор" style="width:100%;height:100%;object-fit:cover;object-position:center top;filter:brightness(0.7) sepia(0.3) contrast(1.1);">
    </div>
  </div>
</div>
---

<!-- Темп прискорюється. Показати що це не нова секта — вона просто переодягається. -->

<div class="pt-2">
  <h1 class="hero-title text-6xl">ГЕОМЕТРИЧНО-ВИМІРУВАЛЬНИЙ КОМПЛЕКС</h1>
</div>

<div class="relative mt-10 px-4 py-10">
  <div class="grid grid-cols-4 gap-4 relative">
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">VI ст. до н.е.</div>
      <div class="text-xl leading-tight">у хітоні</div>
      <div class="small-note mt-2">поклоняютсє числу і прямому куту</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">ранні держави</div>
      <div class="text-xl leading-tight">у печатці й мантії</div>
      <div class="small-note mt-2">оформлюють світ так, щоби його було зручно рахувати</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">офісна епоха</div>
      <div class="text-xl leading-tight">у костюмі менеджера</div>
      <div class="small-note mt-2">малюють KPI, рейтинги, дашборди і таблиці</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">теперішній час</div>
      <div class="text-xl leading-tight">на вашому зап'ясті</div>
      <div class="small-note mt-2">стежать вже не збоку, а зсередини вашого дня</div>
    </div>
  </div>
</div>

<div class="panel-soft px-6 py-4 text-2xl leading-tight mt-2">
  Вони не множилися і не зникали. Вони просто <a style='color: var(--deck-danger)'>перевділись</a>.
</div>

---

<!-- Ключовий слайд — цикл. Говорити повільно, вголос по вузлах. Не коментувати — нехай сама петля говорить. -->

<div class="pt-2 flex flex-col" style="height:100%;">
  <h1 class="hero-title text-5xl leading-none text-center">ЩО ВОНИ ХОЧУТЬ?</h1>
  <div style="flex:1; min-height:0; display:flex; align-items:center; justify-content:center; padding-top:0.5rem; overflow:hidden;">
    <svg viewBox="0 0 520 430" fill="none" style="max-height:100%;width:auto;max-width:88%;">
      <defs>
        <marker id="cw" markerWidth="10" markerHeight="8" refX="9" refY="4" orient="auto">
          <path d="M0 0 L10 4 L0 8 Z" fill="rgba(214,178,94,0.95)"/>
        </marker>
      </defs>
      <text x="260" y="192" text-anchor="middle" fill="rgba(243,236,223,0.28)" style="font-size:12px;">замкнуте</text>
      <text x="260" y="208" text-anchor="middle" fill="rgba(243,236,223,0.28)" style="font-size:12px;">коло</text>
      <path d="M 373 44 Q 468 18 464 170" stroke="rgba(214,178,94,0.65)" stroke-width="2.5" stroke-dasharray="8 5" fill="none" marker-end="url(#cw)"/>
      <path d="M 464 232 Q 478 374 372 374" stroke="rgba(214,178,94,0.65)" stroke-width="2.5" stroke-dasharray="8 5" fill="none" marker-end="url(#cw)"/>
      <path d="M 145 374 Q 38 374 54 234" stroke="rgba(214,178,94,0.65)" stroke-width="2.5" stroke-dasharray="8 5" fill="none" marker-end="url(#cw)"/>
      <path d="M 54 168 Q 38 18 145 44" stroke="rgba(214,178,94,0.65)" stroke-width="2.5" stroke-dasharray="8 5" fill="none" marker-end="url(#cw)"/>
      <rect x="142" y="22" width="236" height="44" rx="14" fill="rgba(243,236,223,0.07)" stroke="rgba(243,236,223,0.25)" stroke-width="1.5"/>
      <text x="260" y="49" text-anchor="middle" fill="#f3ecdf" style="font-size:13px;">Задати форму видимого</text>
      <rect x="348" y="168" width="158" height="64" rx="14" fill="rgba(243,236,223,0.07)" stroke="rgba(243,236,223,0.25)" stroke-width="1.5"/>
      <text x="427" y="194" text-anchor="middle" fill="#f3ecdf" style="font-size:12px;">Керувати бюджетами</text>
      <text x="427" y="213" text-anchor="middle" fill="#f3ecdf" style="font-size:12px;">і нормами</text>
      <rect x="142" y="334" width="236" height="90" rx="14" fill="rgba(243,236,223,0.07)" stroke="rgba(243,236,223,0.25)" stroke-width="1.5"/>
      <text x="260" y="366" text-anchor="middle" fill="#f3ecdf" style="font-size:12px;">Змусити людей</text>
      <text x="260" y="386" text-anchor="middle" fill="#f3ecdf" style="font-size:12px;">вважати реальним</text>
      <text x="260" y="406" text-anchor="middle" fill="#f3ecdf" style="font-size:12px;">лише вимірюване</text>
      <rect x="26" y="172" width="148" height="56" rx="14" fill="rgba(214,178,94,0.12)" stroke="rgba(214,178,94,0.55)" stroke-width="1.5"/>
      <text x="100" y="190" text-anchor="middle" fill="#f3ecdf" style="font-size:11px;">Більше проданих</text>
      <text x="100" y="206" text-anchor="middle" fill="#f3ecdf" style="font-size:11px;">лінійок і циркулів</text>
    </svg>
  </div>
</div>

---

<!-- 

Зупинитись. "Хтось скаже..." — вголос, іронічно. Потім мовчання. Потім — повільно.
Давайте перевіримо... осьо графік їх долі в GDP.
Стоп... ви розумієте шо з цим аргуметом не так?
Ми попали в їхню пастку.

-->

<div class="h-full flex flex-col justify-center items-center text-center px-12">
  <div class="text-2xl leading-tight max-w-3xl opacity-70" style="font-style:italic;">
    Хтось скаже: який вплив можут мати продавці циркулів?
  </div>

  <v-clicks>
  <div class="mt-8" style="max-height:18rem;">
    <img src="./assets/share.png" alt="Share" style="max-height:18rem;width:auto;max-width:100%;object-fit:contain;border-radius:16px;">
  </div>
  </v-clicks>

  <v-clicks>
  <div class="hero-title mt-8" style="font-size: 4.4rem; line-height: 0.95; color: var(--deck-danger);">
    Ми попали в їхню пастку.
  </div>
  </v-clicks>
</div>
---

<!-- Зачитати кілька слів вголос. "Actionable" — наголос на слово. Дати аудиторії побачити список. -->

<div class="pt-2">
  <h1 class="hero-title text-6xl">СЛОВА, ЯКІ ВОНИ ЛЮБЛЯТ</h1>
</div>

<div class="grid grid-cols-3 gap-4 mt-8 text-xl">
  <div class="panel-soft px-5 py-5">quantifiable</div>
  <div class="panel-soft px-5 py-5">standardized</div>
  <div class="panel-soft px-5 py-5">optimized</div>
  <div class="panel-soft px-5 py-5">objective</div>
  <div class="panel-soft px-5 py-5">measurable</div>
  <div class="panel-soft px-5 py-5">commensurable</div>
  <div class="panel-soft px-5 py-5">legible</div>
  <div class="panel-soft px-5 py-5">scalable</div>
  <div class="panel-soft px-5 py-5">evidence-based</div>
  <div class="panel-soft px-5 py-5">actionable</div>
  <div class="panel-soft px-5 py-5">dashboard-ready</div>
  <div class="panel-soft px-5 py-5">придатне до управління</div>
</div>

---

<!-- Зліва — ОК. Справа — заборонено. Пауза після підпису. -->

<div class="pt-2 flex flex-col" style="height:calc(100% - 0.5rem);">
  <div class="flex items-baseline gap-5 mb-3">
    <h1 class="hero-title text-5xl leading-none">ДОЗВОЛЕНІ ФОРМИ РЕАЛЬНОСТИ</h1>
  </div>
  <div class="grid grid-cols-5 gap-4" style="flex:1; min-height:0;">
    <div class="col-span-3" style="display:grid; grid-template-columns:1fr 1fr; grid-template-rows:1fr 1fr; gap:0.6rem; min-height:0;">
      <div style="border-radius:14px;overflow:hidden;background:#fff;display:flex;align-items:center;justify-content:center;padding:0.4rem;">
        <img src="./assets/chart-column.png" alt="Column chart" style="width:100%;height:100%;object-fit:contain;display:block;">
      </div>
      <div style="border-radius:14px;overflow:hidden;background:#fff;display:flex;align-items:center;justify-content:center;padding:0.4rem;">
        <img src="./assets/chart-line.png" alt="Line chart" style="width:100%;height:100%;object-fit:contain;display:block;">
      </div>
      <div style="border-radius:14px;overflow:hidden;background:#fff;display:flex;align-items:center;justify-content:center;padding:0.4rem;">
        <img src="./assets/chart-pie.png" alt="Pie chart" style="width:100%;height:100%;object-fit:contain;display:block;">
      </div>
      <div style="border-radius:14px;overflow:hidden;background:#fff;display:flex;align-items:center;justify-content:center;padding:0.4rem;">
        <img src="./assets/chart-scatter.png" alt="Scatter plot" style="width:100%;height:100%;object-fit:contain;display:block;">
      </div>
    </div>
    <v-clicks>
    <div class="col-span-2 axis-card px-4 py-4 flex flex-col">
      <div style="flex:1; min-height:0; display:flex; align-items:center; justify-content:center; overflow:hidden;">
        <img src="./assets/chart-banned.png" alt="Banned chart" style="max-width:100%;max-height:100%;object-fit:contain;display:block;">
      </div>
      <div class="text-xl leading-tight text-center mt-2" style="color:var(--deck-danger);">
        нам ніколи не дозволять мати такий графік
      </div>
    </div>
    </v-clicks>
  </div>
</div>
---

<!-- Плавно. Не злобно — просто: якщо нема поля, нема рядка. Питання не в злі, а в архітектурі. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">АДМІНІСТРАТИВНО НЕІСНУЮЧЕ</h1>
    <div class="grid grid-cols-2 gap-3 mt-8 text-lg">
      <div class="admin-tag">гідність</div>
      <div class="admin-tag">добрий смак</div>
      <div class="admin-tag">мудрість</div>
      <div class="admin-tag">ніжність</div>
      <div class="admin-tag">локальне знання</div>
      <div class="admin-tag">милість</div>
    </div>
  </div>

  <div class="col-span-2 panel px-5 py-5 flex flex-col justify-between">
    <div class="grid grid-cols-1 gap-3">
      <div class="panel-soft px-4 py-4">
        <div class="text-xl leading-tight">Нема поля — нема рядка.</div>
      </div>
      <div class="panel-soft px-4 py-4">
        <div class="text-xl leading-tight">Нема рядка — нема бюджету.</div>
      </div>
      <div class="panel-soft px-4 py-4">
        <div class="text-xl leading-tight">Нема бюджету — нема офіційної реальности.</div>
      </div>
    </div>
  </div>
</div>

<div class="mt-6 grid grid-cols-2 gap-4 text-xl">
  <div class="panel-soft px-5 py-4">Ніжність не заборонена. Вона просто не має бюджетного рядка.</div>
  <div class="panel-soft px-5 py-4">Гідність існує, але не в дашборді.</div>
</div>

---

<!-- Смішний момент — таблиця з'являється поступово. Дати час прочитати. Потім — різкий поворот: наш сміх і є доказом. -->

<div class="pt-2" style="display:grid; grid-template-columns:1fr 1fr 1fr; gap:0.5rem; font-size:1.05rem;">
  <div></div>
  <div class="panel-soft overflow-hidden" style="height:10rem;">
    <img src="./assets/gorilla.jpg" alt="Горила" style="width:100%;height:100%;object-fit:contain;">
  </div>
  <div class="panel-soft overflow-hidden" style="height:10rem;">
    <img src="./assets/trump.jpg" alt="Трамп" style="width:100%;height:100%;object-fit:contain;filter:brightness(0.92);">
  </div>

  <div class="panel-soft px-4 py-3 opacity-60 font-semibold">показник</div>
  <div class="panel-soft px-4 py-3 opacity-60 font-semibold">горила</div>
  <div class="panel-soft px-4 py-3 opacity-60 font-semibold">Трамп</div>

  <div class="panel-soft px-4 py-3">кількість волося</div>
  <div class="panel-soft px-4 py-3">значна</div>
  <div class="panel-soft px-4 py-3">нестабільна</div>

  <div class="panel-soft px-4 py-3">сила хвату</div>
  <div class="panel-soft px-4 py-3">домінує</div>
  <div class="panel-soft px-4 py-3">невідомо</div>

  <div class="panel-soft px-4 py-3">придатність до джунглів</div>
  <div class="panel-soft px-4 py-3">висока</div>
  <div class="panel-soft px-4 py-3">катастрофічна</div>

  <div class="panel-soft px-4 py-3">симетрія лиця</div>
  <div class="panel-soft px-4 py-3">поза контекстом</div>
  <div class="panel-soft px-4 py-3">чомусь врахована</div>
</div>
---

<!-- Окремий ударний слайд із поясненням. -->

<div class="panel px-6 py-6">
  <div class="hero-title text-5xl leading-none">КОМЕНСУРАЦІЯ</div>
  <div class="text-2xl opacity-80 mt-3">Як починається приниження</div>
  <div class="mt-10 text-2xl leading-tight">
    Насильство починається не в моменті висновку, а коли хтось вирішує, що всіх людей можна порімняти одною шкалою.
  </div>
  <div class="panel-soft px-5 py-5 mt-6 text-xl leading-snug">
    Щойно ми погодились на таку таблицю, ми <a style='color:var(--deck-danger);'>вже програли</a>.
  </div>
  <div class="text-2xl leading-tight mt-5">
    Система придумує нові способи як <b>принизити</b> людину виміруваням.
  </div>
</div>
---

<!-- Це вже кінцева стадія — людина сама себе вимірює. Показати телефон/годинник з залу. -->

<div class="grid grid-cols-3 gap-6 pt-2 items-center">
  <div class="col-span-2 panel px-6 py-6">
    <div class="flex items-center gap-4 mb-6">
      <h1 class="hero-title text-4xl leading-none">ФІНАЛЬНА СТАДІЯ КОНТРОЛЮ</h1>
      <img src="./assets/quantified-self-logo.png" alt="QS" style="width:9.5rem;height:9.5rem;opacity:0.9;">
    </div>
    <div class="mt-4 text-2xl leading-snug">
      Того тижня я знайшов спільноту людей які самі мірают себе каждий Божий день
    </div>
    <div class="panel-soft px-5 py-5 mt-6 text-xl leading-snug">
      сон, кроки, калорії, стрес, готовність до продуктивности, якість ранку, симптоми
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Коли людина сама стає своїм інспектором, система може відпочити.
    </div>
  </div>

  <div class="col-span-1 flex items-center justify-center">
    <img src="./assets/smartwatch-health.png" alt="Smartwatch health" style="max-height:22rem;width:100%;object-fit:contain;border-radius:24px;filter:brightness(0.8) contrast(1.05);">
  </div>
</div>
---

<!-- Найдраматичніший момент. Зупинитись. "Зараз прошу всіх вразливих заплющити очі" — пауза — "бо я покажу вам диявольський прилад для душі." -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">ЕМОЦІЙНИЙ ЦИРКУМПЛЕКС</h1>
    <div style="height: 22rem; margin-top: 1rem; border-radius:18px; overflow:hidden; border:1px solid rgba(243,236,223,0.1); background:rgba(243,236,223,0.03); display:flex; align-items:center; justify-content:center;">
      <img src="./assets/emotional-circumplex.svg" alt="Емоційний циркумплекс" style="width:100%;height:100%;object-fit:contain;padding:0.5rem;">
    </div>
  </div>

  <div class="col-span-2 panel px-5 py-5 flex flex-col justify-between">
    <div class="text-2xl leading-tight">
      Твоє внутрішнє життя — то дві санкціоновані осі.
    </div>
    <div class="panel-soft px-4 py-4 mt-5 text-xl leading-snug">
      Якщо почуття не вкладається в цю схему, його оголосять шумом, збоєм або некоректною самозвітністю.
    </div>
    <div class="final-quote" style="font-size: 1.9rem; max-width: 19rem; color: var(--deck-danger);">
      Вони дійшли вже до душі.
    </div>
  </div>
</div>
