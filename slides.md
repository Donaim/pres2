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

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-8 py-8 flex flex-col justify-between">
    <div class="text-2xl leading-snug max-w-3xl mt-8">
      Жив був Прокруст, він був розбійник.
      Прокруст стояв на дорозі і ласкаво запрошував мандрівників переночувати.
    </div>
    <div class="panel-soft mt-6 px-6 py-6 text-xl leading-snug">
      У нього було ложе однієї правильної довжини.
      Кого тіло виявлялось завеликим — він обрізав.
      Кого замалим — розтягував, доки не підійде.
    </div>
    <div class="text-2xl leading-tight mt-6">
      На ранок у нього всі ставали однаковими.
    </div>
  </div>

  <div class="col-span-2 panel-soft px-6 py-6 flex flex-col justify-between">
    <div style="height: 17rem;">
      <svg viewBox="0 0 260 180" fill="none">
        <rect x="44" y="62" width="172" height="50" rx="12" stroke="rgba(243,236,223,0.28)" stroke-width="3" />
        <rect x="54" y="72" width="68" height="30" rx="8" fill="rgba(243,236,223,0.12)" />
        <line x1="54" y1="112" x2="54" y2="156" stroke="rgba(243,236,223,0.22)" stroke-width="6" stroke-linecap="round" />
        <line x1="206" y1="112" x2="206" y2="156" stroke="rgba(243,236,223,0.22)" stroke-width="6" stroke-linecap="round" />
        <line x1="62" y1="112" x2="62" y2="156" stroke="rgba(243,236,223,0.22)" stroke-width="6" stroke-linecap="round" />
        <line x1="198" y1="112" x2="198" y2="156" stroke="rgba(243,236,223,0.22)" stroke-width="6" stroke-linecap="round" />
        <circle cx="136" cy="86" r="13" fill="#d6b25e" opacity="0.85" />
        <path d="M149 86 L188 86" stroke="#d6b25e" stroke-width="10" stroke-linecap="round" />
        <path d="M112 86 L83 86" stroke="#cf785d" stroke-width="10" stroke-linecap="round" />
        <path d="M137 99 L137 118" stroke="#d6b25e" stroke-width="10" stroke-linecap="round" />
        <path d="M126 120 L109 142" stroke="#d6b25e" stroke-width="8" stroke-linecap="round" />
        <path d="M148 120 L165 142" stroke="#d6b25e" stroke-width="8" stroke-linecap="round" />
      </svg>
    </div>
    <div class="text-2xl leading-tight">
      Одне ложе. Одна правильна довжина. Один господар, який ненавидів усе, що не влазить.
    </div>
  </div>
</div>

---

<div class="pt-2">
  <h1 class="hero-title text-6xl">ЗАКОН ГУДГАРТА</h1>
</div>

<div class="panel mt-8 px-7 py-6 text-2xl leading-tight">
  В 18 столітті Британська імперія колонізовувала Індію і зіткнулася з проблемою кобр.
</div>

<div class="grid grid-cols-4 gap-4 mt-6 text-xl">
  <div class="panel-soft px-5 py-5">
    У містах було багато кобр, і влада хотіла швидко показати результат.
  </div>
  <div class="panel-soft px-5 py-5">
    Ввели нагороду за кожну мертву кобру.
  </div>
  <div class="panel-soft px-5 py-5">
    Люди почали розводити кобр, щоби стабільно здавати їх за винагороду.
  </div>
  <div class="panel-soft px-5 py-5">
    Влада сама створила те, що хотіла знищити.
  </div>
</div>

---

<div class="grid grid-cols-2 gap-8 pt-4 items-stretch">
  <div class="panel-ivory px-8 py-8 flex flex-col justify-between">
    <div>
      <h1 class="hero-title text-6xl mt-1">Уявіть шо…</h1>
    </div>
  </div>

  <div class="panel px-8 py-8 flex flex-col justify-between">
    <v-clicks>
      <div class="text-2xl leading-tight mb-4">на роботі вам платят за вклад, а не за години</div>
      <div class="text-2xl leading-tight mb-4">за каву ви платите за смак, а не за цінник</div>
      <div class="text-2xl leading-tight mb-4">у школі цінують розумінє, а не зубрінє</div>
      <div class="text-2xl leading-tight mb-4">дорожче означає не “статусніше”, а справді якісніше</div>
      <div class="text-2xl leading-tight">країну оцінюють по добробуту людей, а не по GDP</div>
    </v-clicks>
  </div>
</div>

---

<div class="pt-2">
  <h1 class="hero-title text-6xl">Чи чули ви…</h1>
</div>

<div class="grid grid-cols-4 gap-4 mt-8">
  <div class="quote-chip">“Де цифри?”</div>
  <div class="quote-chip">“А на еґзамені то буде?”</div>
  <div class="quote-chip">“Мені не треба красиво, мені треба, шоб робило”</div>
  <div class="quote-chip">“Оцініть свій біль від 0 до 10”</div>
  <div class="quote-chip">“Школа не для того, шоб тобі подобалось”</div>
  <div class="quote-chip">“Дорожче означає ліпше”</div>
  <div class="quote-chip">“Якісне не може бути дешеве”</div>
  <div class="quote-chip">“Може ти й чудова людина, але кредитний скор так не думає”</div>
</div>

<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight">
  Це не випадкові фрази. Це вісім інтонацій одного й того самого дисциплінарного голосу.
</div>

---

<div class="h-full flex flex-col justify-center items-center text-center">
  <div class="hero-title" style="font-size: 5.3rem; line-height: 0.95;">КОМУ ТО ВИГІДНО?</div>
  <div class="mt-10 text-2xl leading-tight max-w-3xl opacity-85">
    Чому школа, ринок, медицина і держава так дружно вимагають не правду, а показник?
  </div>
  <div class="panel-soft mt-10 px-6 py-5 text-xl leading-snug max-w-3xl">
    Бо за кожною шкалою стоїть той, хто вирішив, що саме вважати видимим, серйозним і реальним.
  </div>
</div>

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7">
    <h1 class="hero-title text-5xl mt-1 leading-none">ПІФАГОРІЙЦІ ТА ЇХ ГЕОМЕТРИЧНО-ВИМІРУВАЛЬНИЙ КОМПЛЕКС</h1>
    <div class="mt-5 text-xl leading-snug max-w-2xl">
      Це було не коло невинних математиків. Це була сектантська група, яка проголосила число єдиним шляхом до істини, а правильну форму — законом для світу і людей.
    </div>
    <div class="panel-soft mt-6 px-5 py-5 text-2xl leading-tight">
      Піфагор казав: “Я ненавиджу фасолю”. Для культу, який хотів очистити світ до ідеальної схеми, навіть біб був підозрілим.
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Прокруст не стояв осторонь. Він був силовим крилом тієї самої секти: якщо життя криве, його треба випрямити.
    </div>
  </div>

  <div class="col-span-2 grid grid-rows-3 gap-4">
    <div class="panel-soft px-4 py-4">
      <div class="portrait mb-3">
        <svg viewBox="0 0 220 140" fill="none">
          <rect width="220" height="140" fill="rgba(214,178,94,0.08)" />
          <circle cx="110" cy="52" r="30" fill="#f0d6b3" />
          <path d="M72 122 C84 92, 136 92, 148 122" fill="#d6b25e" opacity="0.42" />
          <path d="M86 40 C94 18, 126 18, 134 40" stroke="#1b2432" stroke-width="10" stroke-linecap="round" />
          <circle cx="100" cy="52" r="3" fill="#1b2432" />
          <circle cx="120" cy="52" r="3" fill="#1b2432" />
          <path d="M101 67 C107 71, 113 71, 119 67" stroke="#1b2432" stroke-width="3" stroke-linecap="round" />
        </svg>
      </div>
      <div class="text-xl leading-tight">Піфагор</div>
      <div class="small-note mt-2">вождь секти, ненависник фасолі, проповідник числа</div>
    </div>

    <div class="panel-soft px-4 py-4">
      <div class="portrait mb-3">
        <svg viewBox="0 0 220 140" fill="none">
          <rect width="220" height="140" fill="rgba(121,181,168,0.08)" />
          <circle cx="110" cy="54" r="30" fill="#efddc2" />
          <path d="M76 126 C89 92, 131 92, 144 126" fill="#79b5a8" opacity="0.36" />
          <path d="M86 34 C96 24, 125 22, 138 38" stroke="#79b5a8" stroke-width="12" stroke-linecap="round" />
          <circle cx="99" cy="53" r="3" fill="#1b2432" />
          <circle cx="120" cy="53" r="3" fill="#1b2432" />
          <path d="M95 70 C104 62, 115 62, 124 70" stroke="#1b2432" stroke-width="3" stroke-linecap="round" />
        </svg>
      </div>
      <div class="text-xl leading-tight">Посвячений брат</div>
      <div class="small-note mt-2">шепче числа, боїться невимірюваного, клянеться прямому кутові</div>
    </div>

    <div class="panel-soft px-4 py-4">
      <div class="portrait mb-3">
        <svg viewBox="0 0 220 140" fill="none">
          <rect width="220" height="140" fill="rgba(207,120,93,0.08)" />
          <circle cx="110" cy="54" r="30" fill="#f0d0bb" />
          <path d="M72 122 C86 88, 134 88, 148 122" fill="#cf785d" opacity="0.34" />
          <path d="M88 40 C95 28, 127 28, 132 40" stroke="#1b2432" stroke-width="12" stroke-linecap="round" />
          <circle cx="100" cy="54" r="3" fill="#1b2432" />
          <circle cx="120" cy="54" r="3" fill="#1b2432" />
          <path d="M96 70 L124 70" stroke="#1b2432" stroke-width="3" stroke-linecap="round" />
        </svg>
      </div>
      <div class="text-xl leading-tight">Прокруст</div>
      <div class="small-note mt-2">польовий оператор, який випрямляв людей під стандарт</div>
    </div>
  </div>
</div>

---

<div class="pt-2">
  <h1 class="hero-title text-6xl">ОДНІ Й ТІ САМІ ЛЮДИ В РІЗНИХ КОСТЮМАХ</h1>
</div>

<div class="relative mt-10 px-4 py-10">
  <div class="timeline-track"></div>
  <div class="grid grid-cols-5 gap-4 relative">
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">VI ст. до н.е.</div>
      <div class="text-xl leading-tight">у хітоні</div>
      <div class="small-note mt-2">поклоняютсє числу і прямому куту</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">античність</div>
      <div class="text-xl leading-tight">у мандрівному плащі</div>
      <div class="small-note mt-2">перевіряють, хто влазить у правильну форму</div>
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

<div class="pt-2">
  <h1 class="hero-title text-6xl">СЛОВА, ЯКІ ВОНИ ЛЮБЛЯТ</h1>
</div>

<div class="grid grid-cols-3 gap-4 mt-8 text-xl">
  <div class="panel-soft px-5 py-5">quantifiable</div>
  <div class="panel-soft px-5 py-5">commensurable</div>
  <div class="panel-soft px-5 py-5">measurable</div>
  <div class="panel-soft px-5 py-5">legible</div>
  <div class="panel-soft px-5 py-5">standardized</div>
  <div class="panel-soft px-5 py-5">optimized</div>
  <div class="panel-soft px-5 py-5">objective</div>
  <div class="panel-soft px-5 py-5">scalable</div>
  <div class="panel-soft px-5 py-5">evidence-based</div>
  <div class="panel-soft px-5 py-5">actionable</div>
  <div class="panel-soft px-5 py-5">dashboard-ready</div>
  <div class="panel px-5 py-5 text-[var(--deck-accent)]">придатне до управління</div>
</div>

<div class="mt-8 text-2xl leading-tight max-w-4xl">
  Кожне з цих слів означає одне: зробіть світ придатним до обліку.
</div>

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7">
    <h1 class="hero-title text-5xl leading-none">ЩО ВОНИ ХОЧУТЬ?</h1>
    <div class="grid grid-cols-3 gap-4 mt-8 text-lg">
      <div class="panel-soft px-4 py-5">
        <div class="text-2xl leading-tight">На поверхні</div>
        <div class="small-note mt-3">більше проданих лінійок, тестів, шкал, аудитів і дашбордів</div>
      </div>
      <div class="panel-soft px-4 py-5">
        <div class="text-2xl leading-tight">Глибше</div>
        <div class="small-note mt-3">хто задає форму видимого, той керує рішеннями, бюджетами і нормою</div>
      </div>
      <div class="panel-soft px-4 py-5">
        <div class="text-2xl leading-tight">Найглибше</div>
        <div class="small-note mt-3">змусити людей вважати реальним тільки те, що можна внести в метрику, таблицю або графік</div>
      </div>
    </div>

    <div class="panel-soft mt-6 px-5 py-5 text-2xl leading-tight">
      Якщо люди довіряють тільки графіку, світом керують ті, хто вирішує, що саме можна намалювати.
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
    <div class="panel-soft mt-5 px-4 py-4 text-2xl leading-tight">
      І отут ми вже в пастці.
    </div>
    <div class="text-xl leading-snug mt-5">
      Щойно ми просимо графік як доказ, ми вже погодились, що реальне тільки те, що можна виміряти, показати і порівняти.
    </div>
  </div>
</div>

---

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="axis-card px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">ДОЗВОЛЕНІ ФОРМИ РЕАЛЬНОСТИ</h1>
    <div class="grid grid-cols-2 gap-4 mt-8">
      <div class="mini-chart px-4 py-4">
        <svg viewBox="0 0 100 60" fill="none">
          <rect x="12" y="26" width="10" height="22" fill="#d6b25e" />
          <rect x="30" y="18" width="10" height="30" fill="#d6b25e" opacity="0.85" />
          <rect x="48" y="10" width="10" height="38" fill="#d6b25e" opacity="0.7" />
          <rect x="66" y="22" width="10" height="26" fill="#d6b25e" opacity="0.55" />
        </svg>
      </div>
      <div class="mini-chart px-4 py-4">
        <svg viewBox="0 0 100 60" fill="none">
          <path d="M8 42 C20 36, 28 34, 40 28 S64 18, 92 10" stroke="#79b5a8" stroke-width="4" stroke-linecap="round" />
        </svg>
      </div>
      <div class="mini-chart px-4 py-4">
        <svg viewBox="0 0 100 60" fill="none">
          <circle cx="50" cy="30" r="18" stroke="#f3ecdf" stroke-width="18" opacity="0.18" />
          <path d="M50 30 L50 12 A18 18 0 0 1 67.5 34 Z" fill="#d6b25e" />
        </svg>
      </div>
      <div class="mini-chart px-4 py-4">
        <svg viewBox="0 0 100 60" fill="none">
          <circle cx="18" cy="39" r="3" fill="#79b5a8" />
          <circle cx="34" cy="28" r="3" fill="#79b5a8" />
          <circle cx="46" cy="34" r="3" fill="#79b5a8" />
          <circle cx="62" cy="22" r="3" fill="#79b5a8" />
          <circle cx="78" cy="17" r="3" fill="#79b5a8" />
        </svg>
      </div>
      <div class="mini-chart px-4 py-4 col-span-2">
        <svg viewBox="0 0 100 60" fill="none">
          <path d="M8 50 L8 46 C22 44, 32 36, 46 26 S72 12, 92 10 L92 50 Z" fill="rgba(214,178,94,0.5)" />
        </svg>
      </div>
    </div>
  </div>

  <div class="axis-card px-6 py-6 spiral">
    <div style="height: 18rem;">
      <svg viewBox="0 0 320 260" fill="none">
        <path d="M162 131 C162 131, 185 122, 192 137 C199 152, 175 171, 151 170 C119 168, 97 138, 104 103 C112 63, 155 42, 198 54 C247 68, 274 120, 259 171 C240 235, 167 257, 103 239 C27 218, -2 124, 33 57" stroke="#cf785d" stroke-width="6" stroke-linecap="round" />
        <circle cx="245" cy="60" r="11" fill="#d6b25e" opacity="0.95" />
        <circle cx="88" cy="204" r="8" fill="#79b5a8" opacity="0.9" />
        <circle cx="204" cy="198" r="6" fill="#f3ecdf" opacity="0.8" />
      </svg>
    </div>
    <div class="text-2xl leading-tight mt-3 text-center">
      нам ніколи не дозволять мати такий графік
    </div>
  </div>
</div>

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">АДМІНІСТРАТИВНО НЕІСНУЮЧЕ</h1>
    <div class="grid grid-cols-2 gap-3 mt-8 text-lg">
      <div class="admin-tag">ніжність</div>
      <div class="admin-tag">гідність</div>
      <div class="admin-tag">змішані емоції</div>
      <div class="admin-tag">локальне знання</div>
      <div class="admin-tag">примирення</div>
      <div class="admin-tag">мудрість без сертифіката</div>
      <div class="admin-tag">відчуття, що тебе справді побачили</div>
      <div class="admin-tag">добрий смак</div>
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
    <div class="void-stamp mt-5">нерепортоване не означає неіснуюче</div>
  </div>
</div>

<div class="mt-6 grid grid-cols-2 gap-4 text-xl">
  <div class="panel-soft px-5 py-4">Ніжність не заборонена. Вона просто не має бюджетного рядка.</div>
  <div class="panel-soft px-5 py-4">Гідність існує, але не в дашборді.</div>
</div>

---

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">КОМЕНСУРАЦІЯ</h1>
    <div class="text-2xl opacity-80 mt-2">Як починається приниження</div>
    <table class="data-table mt-8">
      <thead>
        <tr>
          <th>показник</th>
          <th>горила</th>
          <th>Трамп</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>кількість волосся</td>
          <td>висока</td>
          <td>нестабільна</td>
        </tr>
        <tr>
          <td>маса</td>
          <td>значна</td>
          <td>також значна</td>
        </tr>
        <tr>
          <td>сила хвату</td>
          <td>домінує</td>
          <td>невідомо</td>
        </tr>
        <tr>
          <td>коефіцієнт придатности до джунглів</td>
          <td>високий</td>
          <td>катастрофічний</td>
        </tr>
        <tr>
          <td>симетрія лиця</td>
          <td>поза контекстом</td>
          <td>чомусь врахована</td>
        </tr>
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

<div class="grid grid-cols-5 gap-6 pt-2 items-center">
  <div class="col-span-2 panel px-6 py-6">
    <h1 class="hero-title text-5xl leading-none">ОСТАННЯ СТАДІЯ: QUANTIFIED SELF</h1>
    <div class="mt-8 text-2xl leading-snug">
      Того тижня я знайшов спільноту людей, метою яких є поміряти себе.
    </div>
    <div class="panel-soft px-5 py-5 mt-6 text-xl leading-snug">
      сон, кроки, стрес, готовність до продуктивности, якість ранку, індекс вечора, настрій у цифрі
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Коли людина сама стає своїм інспектором, братству вже не треба стояти поруч.
    </div>
  </div>

  <div class="col-span-3 flex items-center justify-center gap-6">
    <div class="watch-band"></div>
    <div class="watch flex flex-col justify-center items-center text-center">
      <div class="text-sm uppercase tracking-[0.22em] opacity-60">self report</div>
      <div class="text-5xl mt-2">87</div>
      <div class="text-lg mt-2">готовність до продуктивности</div>
      <div class="mt-4 grid grid-cols-2 gap-3 text-sm w-44">
        <div class="panel-soft px-2 py-2">сон 6:11</div>
        <div class="panel-soft px-2 py-2">стрес 42</div>
        <div class="panel-soft px-2 py-2">кроки 9 804</div>
        <div class="panel-soft px-2 py-2">настрій 6.2</div>
      </div>
    </div>
    <div class="watch-band"></div>
  </div>
</div>

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6 circumplex">
    <h1 class="hero-title text-5xl leading-none">ЕМОЦІЙНИЙ ЦИРКУМПЛЕКС</h1>
    <div class="text-2xl leading-snug mt-4 max-w-3xl">
      Там я знайшов оцей диявольський прилад, шо вони назвали емоційним циркумплексом.
    </div>
    <div style="height: 20rem; margin-top: 1.2rem;">
      <svg viewBox="0 0 520 340" fill="none">
        <rect x="70" y="25" width="280" height="280" rx="26" fill="rgba(243,236,223,0.03)" stroke="rgba(243,236,223,0.16)" />
        <line x1="210" y1="45" x2="210" y2="285" stroke="rgba(243,236,223,0.22)" stroke-width="2" />
        <line x1="90" y1="165" x2="330" y2="165" stroke="rgba(243,236,223,0.22)" stroke-width="2" />
        <circle cx="210" cy="165" r="96" stroke="rgba(214,178,94,0.38)" stroke-width="2" />
        <text x="218" y="54" fill="#f3ecdf" font-size="18">активація</text>
        <text x="230" y="320" fill="#f3ecdf" font-size="18">деактивація</text>
        <text x="92" y="156" fill="#f3ecdf" font-size="18">неприємно</text>
        <text x="280" y="156" fill="#f3ecdf" font-size="18">приємно</text>
        <text x="255" y="98" fill="#79b5a8" font-size="19">радість</text>
        <text x="250" y="240" fill="#d6b25e" font-size="19">спокій</text>
        <text x="126" y="238" fill="#cf785d" font-size="19">смуток</text>
        <text x="126" y="104" fill="#f1c6b8" font-size="19">гнів</text>
        <text x="382" y="92" fill="#f3ecdf" font-size="18">дозволені стани</text>
        <text x="382" y="126" fill="#a9b4c5" font-size="16">однозначні</text>
        <text x="382" y="148" fill="#a9b4c5" font-size="16">чисті</text>
        <text x="382" y="170" fill="#a9b4c5" font-size="16">зручні</text>
        <rect x="372" y="202" width="116" height="54" rx="16" fill="rgba(207,120,93,0.08)" stroke="rgba(207,120,93,0.28)" />
        <text x="390" y="223" fill="#f1c6b8" font-size="14">INVALID BLEND</text>
        <text x="389" y="244" fill="#f1c6b8" font-size="14">злий + веселий</text>
      </svg>
    </div>
  </div>

  <div class="col-span-2 panel px-5 py-5 flex flex-col justify-between">
    <div class="text-2xl leading-tight">
      Це прилад для душі, в якому внутрішнє життя силоміць кладуть на дві санкціоновані осі.
    </div>
    <div class="panel-soft px-4 py-4 mt-5 text-xl leading-snug">
      Якщо почуття не вкладається в цю схему, його оголосять шумом, збоєм або некоректною самозвітністю.
    </div>
    <div class="final-quote" style="font-size: 1.9rem; max-width: 19rem;">
      Вони дійшли вже до душі.
    </div>
  </div>
</div>
