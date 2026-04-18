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

<div class="pt-2">
  <h1 class="hero-title text-6xl">ЗАКОН ГУДГАРТА</h1>
</div>

<div class="grid grid-cols-5 gap-6 mt-6 items-stretch">
  <div class="col-span-3">
    <div class="panel px-7 py-6 text-2xl leading-tight">
      В 18 столітті Британська імперія колонізовувала Індію і зіткнулася з проблемою кобр.
    </div>
    <div class="grid grid-cols-2 gap-4 mt-4 text-xl">
      <div class="panel-soft px-5 py-5">
        Як горобці китайцям, кобри перешкоджали тодішній короні.
      </div>
      <div class="panel-soft px-5 py-5">
        Влада почала скуповувати шкіру кобр.
      </div>
      <div class="panel-soft px-5 py-5">
        Люди почали розводити кобр, і здавати їх за винагороду.
      </div>
      <div class="panel-soft px-5 py-5">
        Влада сама породила те, що хотіла знищити.
      </div>
    </div>
  <v-clicks>
  <div class="col-span-2 panel-soft flex items-center justify-center overflow-hidden" style="border-radius:24px; min-height:18rem;">
    <img src="./assets/cobra-india.jpg" alt="Кобра" style="width:100%;height:50%;object-fit:cover;filter:brightness(0.75) contrast(1.1);border-radius:24px;">
  </div>
  </v-clicks>
    <v-clicks>
    <div class="panel-soft mt-6 px-6 py-5 text-2xl leading-tight">
      Коли число стає цільом, правда починає вдавати число.
    </div>
    </v-clicks>
  </div>
</div>

---

<!-- Простий слайд, риторичний. Не пояснювати — просто пройтись по пунктах з паузами. Остання фраза — підвести до питання: але хто це все влаштував? -->

<div class="grid grid-cols-2 gap-8 pt-4 items-stretch">
  <div class="panel-ivory px-8 py-8 flex flex-col justify-between">
    <div>
      <h1 class="hero-title text-6xl mt-1">Уяви що...</h1>
    </div>
  </div>

  <div class="panel px-8 py-8 flex flex-col justify-between">
    <v-clicks>
      <div class="text-2xl leading-tight mb-4">на роботі вам платят за вклад, а не за години</div>
      <div class="text-2xl leading-tight mb-4">за каву ви платите за смак, а не за цінник</div>
      <div class="text-2xl leading-tight mb-4">у школі цінують розуміня, а не зубріня</div>
      <div class="text-2xl leading-tight mb-4">дорожче означає не “статусніше”, а справді якісніше</div>
      <div class="text-2xl leading-tight">країну оцінюють по добробуту людей, а не по GDP</div>
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

<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight">
  Це не випадкові фрази. Це вісім інтонацій одного й того самого дисциплінарного голосу.
</div>

---

<!-- Тут НЕ відповідати — лише поставити питання. Пауза після першого кліку довша. Наступний слайд дає відповідь — але несподівану. -->

<div class="h-full flex flex-col justify-center items-center text-center">
  <div class="hero-title" style="font-size: 5.3rem; line-height: 0.95;">КОМУ ТО ВИГІДНО?</div>
  <v-clicks>
  <div class="mt-10 text-2xl leading-tight max-w-3xl opacity-85">
    Чому школа, ринок, медицина і держава так дружно вимагають не правду, а показник?
  </div>
  </v-clicks>
  <v-clicks>
  <div class="panel-soft mt-10 px-6 py-5 text-xl leading-snug max-w-3xl">
    Відповідь неочікувана: не тому, що хтось злий, а тому, що хтось колись навчив ці інституції говорити однією мовою.
    Мовою числа. А вони просто повторюють — бо іншої не знають.
  </div>
  </v-clicks>
  <v-clicks>
  <div class="panel-soft mt-6 px-6 py-4 text-xl leading-snug max-w-3xl" style="border-color: rgba(207,120,93,0.28); background: rgba(207,120,93,0.08);">
    Вигодонабувач — не школа і не лікарня. Вигодонабувач — той, хто першим вирішив, що саме вважати видимим.
  </div>
  </v-clicks>
</div>

---

<!-- Секта — не метафора. "Я ненавиджу фасолю" — пауза для сміху, потім серйозно. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7">
    <h1 class="hero-title text-5xl mt-1 leading-none">ПІФАГОРІЙЦІ ТА ЇХ ГЕОМЕТРИЧНО-ВИМІРУВАЛЬНИЙ КОМПЛЕКС</h1>
    <div class="mt-5 text-xl leading-snug max-w-2xl">
      Це було не коло невинних математиків. Це була сектантська група, яка проголосила число єдиним шляхом до істини, а правильну форму — законом для світу і людей.
    </div>
    <div class="panel-soft mt-6 px-5 py-5 text-2xl leading-tight">
      Піфагор казав: "Я ненавиджу фасолю". Для культу, який хотів очистити світ до ідеальної схеми, навіть біб був підозрілим.
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Прокруст не стояв осторонь. Він був силовим крилом тієї самої секти: якщо життя криве, його треба випрямити.
    </div>
  </div>

  <div class="col-span-2 flex flex-col gap-4">
    <div class="panel-soft px-5 py-5 flex flex-col items-center" style="flex:1;">
      <div style="height: 16rem; width: 100%; overflow: hidden; border-radius: 18px;">
        <img src="./assets/pythagoras.jpg" alt="Піфагор" style="width:100%;height:100%;object-fit:cover;object-position:center top;filter:brightness(0.85) sepia(0.18);">
      </div>
      <div class="text-xl leading-tight mt-3 text-center">Піфагор</div>
      <div class="small-note mt-2 text-center">"я ненавиджу фасолю" — вождь секти, проповідник числа</div>
    </div>
    <div class="panel-soft px-5 py-4 flex flex-row items-center gap-4" style="flex:0 0 auto;">
      <div class="text-4xl">🧱</div>
      <div>
        <div class="text-xl leading-tight">Прокруст</div>
        <div class="small-note mt-1">силове крило — якщо тіло не вміщається, вкоротити</div>
      </div>
    </div>
  </div>
</div>
---

<!-- Темп прискорюється. Показати що це не нова секта — вона просто переодягається. -->

<div class="pt-2">
  <h1 class="hero-title text-6xl">ОДНІ Й ТІ САМІ ЛЮДИ В РІЗНИХ КОСТЮМАХ</h1>
</div>

<div class="relative mt-10 px-4 py-10">
  <div class="grid grid-cols-5 gap-4 relative">
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">VI ст. до н.е.</div>
      <div class="text-xl leading-tight">у хітоні</div>
      <div class="small-note mt-2">поклоняютсє числу і прямому куту</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">ранні держави</div>
      <div class="text-xl leading-tight">у печатці й мантії</div>
      <div class="small-note mt-2">оформлюють світ так, щоби його було зручно зводити</div>
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
  Вони не множилися і не зникали. Вони просто навчились міняти тканину, печатку й інтерфейс.
</div>

---

<!-- Ключовий слайд — цикл. Малювати пальцем у повітрі. Йти повільно по колу. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7">
    <h1 class="hero-title text-5xl leading-none">ЩО ВОНИ ХОЧУТЬ?</h1>
    <div class="mt-6 text-xl leading-snug opacity-80 max-w-2xl">
      Не лінійна вигода. Петля. Кожен крок закріплює наступний.
    </div>
    <div class="mt-8 flex flex-col items-center" style="position:relative;">
      <svg viewBox="0 0 420 300" fill="none" style="width:100%;max-width:420px;">
        <!-- arcs connecting nodes -->
        <path d="M 105 60 C 200 20, 315 20, 315 90" stroke="rgba(214,178,94,0.55)" stroke-width="2.5" stroke-dasharray="6 4" marker-end="url(#arr)" />
        <path d="M 330 110 C 380 170, 360 230, 300 250" stroke="rgba(214,178,94,0.55)" stroke-width="2.5" stroke-dasharray="6 4" marker-end="url(#arr)" />
        <path d="M 240 260 C 170 280, 100 260, 80 210" stroke="rgba(214,178,94,0.55)" stroke-width="2.5" stroke-dasharray="6 4" marker-end="url(#arr)" />
        <path d="M 70 185 C 40 130, 60 80, 90 65" stroke="rgba(214,178,94,0.55)" stroke-width="2.5" stroke-dasharray="6 4" marker-end="url(#arr)" />
        <defs>
          <marker id="arr" markerWidth="8" markerHeight="8" refX="4" refY="4" orient="auto">
            <path d="M1 1 L7 4 L1 7 Z" fill="rgba(214,178,94,0.8)" />
          </marker>
        </defs>
        <!-- Node 1 top-left -->
        <rect x="18" y="36" width="170" height="52" rx="16" fill="rgba(214,178,94,0.13)" stroke="rgba(214,178,94,0.4)" stroke-width="1.5" />
        <text x="103" y="64" text-anchor="middle" fill="#f3ecdf" font-size="13" font-family="IBM Plex Sans, sans-serif">Задати форму видимого</text>
        <!-- Node 2 top-right -->
        <rect x="232" y="36" width="172" height="52" rx="16" fill="rgba(121,181,168,0.13)" stroke="rgba(121,181,168,0.4)" stroke-width="1.5" />
        <text x="318" y="57" text-anchor="middle" fill="#f3ecdf" font-size="13" font-family="IBM Plex Sans, sans-serif">Керувати бюджетами</text>
        <text x="318" y="76" text-anchor="middle" fill="#f3ecdf" font-size="13" font-family="IBM Plex Sans, sans-serif">і нормами</text>
        <!-- Node 3 bottom-right -->
        <rect x="232" y="226" width="172" height="52" rx="16" fill="rgba(207,120,93,0.13)" stroke="rgba(207,120,93,0.4)" stroke-width="1.5" />
        <text x="318" y="247" text-anchor="middle" fill="#f3ecdf" font-size="13" font-family="IBM Plex Sans, sans-serif">Більше проданих</text>
        <text x="318" y="266" text-anchor="middle" fill="#f3ecdf" font-size="13" font-family="IBM Plex Sans, sans-serif">лінійок</text>
        <!-- Node 4 bottom-left -->
        <rect x="18" y="226" width="170" height="52" rx="16" fill="rgba(243,236,223,0.07)" stroke="rgba(243,236,223,0.22)" stroke-width="1.5" />
        <text x="103" y="247" text-anchor="middle" fill="#f3ecdf" font-size="12" font-family="IBM Plex Sans, sans-serif">Змусити вважати</text>
        <text x="103" y="265" text-anchor="middle" fill="#f3ecdf" font-size="12" font-family="IBM Plex Sans, sans-serif">реальним лише вимірюване</text>
      </svg>
    </div>
  </div>

  <div class="col-span-2 axis-card px-5 py-5 flex flex-col justify-between">
    <div class="text-xl leading-snug">
      Хтось скаже: якщо дивитися на прямі показники, їхній вплив виглядає мізерним.
    </div>
    <div class="mini-chart mt-6 px-4 py-4">
      <svg viewBox="0 0 100 60" fill="none">
        <path d="M8 44 C20 43, 34 42, 48 40 S72 36, 92 34" stroke="#a9b4c5" stroke-width="4" stroke-linecap="round" opacity="0.75" />
        <path d="M8 49 L92 49" stroke="rgba(243,236,223,0.18)" stroke-width="2" stroke-linecap="round" />
      </svg>
    </div>
    <div class="text-xl leading-snug mt-4 opacity-75">
      Але саме це і є пасткою.
    </div>
  </div>
</div>

---

<!-- Зупинитись. Мовчати 3 секунди після першого речення. Потім — "Ми вже в пастці." дуже повільно. -->

<div class="h-full flex flex-col justify-center items-center text-center px-12">
  <div class="text-3xl leading-tight max-w-3xl opacity-85">
    Розумієте, що не так із цим аргументом?
  </div>
  <v-clicks>
  <div class="mt-10 text-3xl leading-tight max-w-3xl">
    Щойно ми просимо графік як доказ — ми вже погодились, що реальне тільки те, що можна виміряти, показати і порівняти.
  </div>
  </v-clicks>
  <v-clicks>
  <div class="hero-title mt-14" style="font-size: 4.2rem; line-height: 0.95; color: var(--deck-danger);">
    Ми попали в їх пастку.
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

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="axis-card px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">ДОЗВОЛЕНІ ФОРМИ РЕАЛЬНОСТИ</h1>
    <div class="mt-6 text-xl leading-snug opacity-75">те, що можна намалювати і показати</div>
    <div style="margin-top:1.5rem;border-radius:18px;overflow:hidden;border:1px solid rgba(243,236,223,0.1);">
      <img src="./assets/excel-chart.png" alt="Excel" style="width:100%;display:block;filter:brightness(0.85) contrast(1.05);">
    </div>
  </div>

  <div class="axis-card px-6 py-6 spiral flex flex-col justify-between">
    <div class="text-xl leading-snug opacity-75">те, що ніколи не дозволять показати</div>
    <div style="height: 18rem; display:flex;align-items:center;justify-content:center;">
      <svg viewBox="0 0 320 260" fill="none" style="width:100%;height:100%;">
        <path d="M162 131 C162 131, 185 122, 192 137 C199 152, 175 171, 151 170 C119 168, 97 138, 104 103 C112 63, 155 42, 198 54 C247 68, 274 120, 259 171 C240 235, 167 257, 103 239 C27 218, -2 124, 33 57" stroke="#cf785d" stroke-width="6" stroke-linecap="round" />
        <circle cx="245" cy="60" r="11" fill="#d6b25e" opacity="0.95" />
        <circle cx="88" cy="204" r="8" fill="#79b5a8" opacity="0.9" />
        <circle cx="204" cy="198" r="6" fill="#f3ecdf" opacity="0.8" />
      </svg>
    </div>
    <div class="text-2xl leading-tight text-center" style="color:var(--deck-danger);">
      нам ніколи не дозволять мати такий графік
    </div>
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

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">КОМЕНСУРАЦІЯ</h1>
    <div class="text-2xl opacity-80 mt-2">Як починається приниження</div>
    <div class="grid grid-cols-2 gap-4 mt-6" style="align-items:start;">
      <div class="panel-soft flex flex-col items-center px-3 py-4" style="border-radius:18px;">
        <div style="height:9rem;width:100%;overflow:hidden;border-radius:14px;">
          <img src="./assets/trump.jpg" alt="Трамп" style="width:100%;height:100%;object-fit:cover;object-position:center top;filter:brightness(0.9);">
        </div>
        <div class="text-lg mt-3 text-center">Трамп</div>
      </div>
      <div class="panel-soft flex flex-col items-center px-3 py-4" style="border-radius:18px;">
        <div style="height:9rem;width:100%;overflow:hidden;border-radius:14px;background:rgba(243,236,223,0.05);display:flex;align-items:center;justify-content:center;">
          <div style="font-size:5rem;">🦍</div>
        </div>
        <div class="text-lg mt-3 text-center">Горила</div>
      </div>
    </div>
    <table class="data-table mt-5">
      <thead><tr><th>показник</th><th>горила</th><th>Трамп</th></tr></thead>
      <tbody>
        <tr><td>маса</td><td>значна</td><td>також значна</td></tr>
        <tr><td>сила хвату</td><td>домінує</td><td>невідомо</td></tr>
        <tr><td>придатність до джунглів</td><td>висока</td><td>катастрофічна</td></tr>
        <tr><td>симетрія лиця</td><td>поза контекстом</td><td>чомусь врахована</td></tr>
      </tbody>
    </table>
  </div>

  <div class="panel px-6 py-6 flex flex-col justify-between">
    <div class="text-2xl leading-tight">
      Насильство починається не в моменті висновку. Воно починається в моменті, коли хтось вирішує, що в них узагалі має бути спільна вісь.
    </div>
    <div class="panel-soft px-5 py-5 mt-5 text-xl leading-snug">
      Щойно ми погодились на таку таблицю, ми вже погодились, що різне треба принизити до порівнюваного.
    </div>
    <div class="text-2xl leading-tight mt-5">
      Коменсурація не просто описує світ. Вона силоміць робить його зручним для приниження.
    </div>
  </div>
</div>
---

<!-- Це вже кінцева стадія — людина сама себе вимірює. Показати телефон/годинник з залу. -->

<div class="grid grid-cols-5 gap-6 pt-2 items-center">
  <div class="col-span-2 panel px-6 py-6">
    <div class="flex items-center gap-4 mb-6">
      <img src="./assets/quantified-self-logo.png" alt="QS" style="width:3.5rem;height:3.5rem;border-radius:12px;opacity:0.9;">
      <h1 class="hero-title text-4xl leading-none">QUANTIFIED SELF</h1>
    </div>
    <div class="mt-4 text-2xl leading-snug">
      Того тижня я знайшов спільноту людей, метою яких є поміряти себе.
    </div>
    <div class="panel-soft px-5 py-5 mt-6 text-xl leading-snug">
      сон, кроки, стрес, готовність до продуктивности, якість ранку, індекс вечора, настрій у цифрі
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Коли людина сама стає своїм інспектором, братству вже не треба стояти поруч.
    </div>
  </div>

  <div class="col-span-3 flex items-center justify-center" style="height:100%;">
    <div style="height:100%;max-height:22rem;overflow:hidden;border-radius:24px;border:1px solid rgba(243,236,223,0.1);">
      <img src="./assets/smartwatch-health.png" alt="Smartwatch health" style="height:100%;width:auto;display:block;object-fit:cover;filter:brightness(0.8) contrast(1.05);">
    </div>
  </div>
</div>
---

<!-- Найдраматичніший момент. Зупинитись. "Зараз прошу всіх вразливих заплющити очі" — пауза — "бо я покажу вам диявольський прилад для душі." -->

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">ЕМОЦІЙНИЙ ЦИРКУМПЛЕКС</h1>
    <div class="text-2xl leading-snug mt-4 max-w-3xl">
      Там я знайшов оцей диявольський прилад, шо вони назвали емоційним циркумплексом.
    </div>
    <div style="height: 22rem; margin-top: 1rem; border-radius:18px; overflow:hidden; border:1px solid rgba(243,236,223,0.1); background:rgba(243,236,223,0.03); display:flex; align-items:center; justify-content:center;">
      <img src="./assets/emotional-circumplex.svg" alt="Емоційний циркумплекс" style="width:100%;height:100%;object-fit:contain;padding:0.5rem;">
    </div>
  </div>

  <div class="col-span-2 panel px-5 py-5 flex flex-col justify-between">
    <div class="text-2xl leading-tight">
      Це прилад для душі, в якому внутрішнє життя силоміць кладуть на дві санкціоновані осі.
    </div>
    <div class="panel-soft px-4 py-4 mt-5 text-xl leading-snug">
      Якщо почуття не вкладається в цю схему, його оголосять шумом, збоєм або некоректною самозвітністю.
    </div>
    <div class="panel-soft px-4 py-4 mt-4 text-xl leading-snug" style="border-color:rgba(207,120,93,0.3);background:rgba(207,120,93,0.08);">
      Зараз прошу всіх вразливих заплющити очі.<br>
      <span class="small-note">Бо я покажу вам диявольський прилад для душі.</span>
    </div>
    <div class="final-quote" style="font-size: 1.9rem; max-width: 19rem; color: var(--deck-danger);">
      Вони дійшли вже до душі.
    </div>
  </div>
</div>
