---
title: Братство прямої міри
theme: seriph
info: |
  ## Братство прямої міри
  Серйозна псевдо-аналітична сатирична презентація про культ вимірюваного.
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

  .eyebrow {
    text-transform: uppercase;
    letter-spacing: 0.22em;
    font-size: 0.72rem;
    color: var(--deck-muted);
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

  .metric-chip {
    display: inline-flex;
    align-items: center;
    padding: 0.55rem 0.85rem;
    border-radius: 999px;
    border: 1px solid var(--deck-line);
    background: rgba(243, 236, 223, 0.06);
    font-size: 0.92rem;
    line-height: 1.2;
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

  .stamp {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    padding: 0.4rem 0.7rem;
    border-radius: 999px;
    border: 1px solid rgba(214, 178, 94, 0.34);
    color: var(--deck-accent);
    font-size: 0.78rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
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
  .circumplex svg {
    width: 100%;
    height: 100%;
  }

  .case-card,
  .victim-card,
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

  .small-note {
    color: var(--deck-muted);
    font-size: 0.9rem;
    line-height: 1.35;
  }
</style>

<div class="grid grid-cols-2 gap-8 pt-4 items-stretch">
  <div class="panel-ivory px-8 py-8 flex flex-col justify-between">
    <div>
      <div class="eyebrow">гіпотетичний вступ</div>
      <h1 class="hero-title text-6xl mt-3">Уявіть шо…</h1>
    </div>
    <div class="small-note mt-6" style="color:#4b5563; max-width: 25rem;">
      Світ, де сутність іще не програла своєму замінникові.
    </div>
  </div>

  <div class="panel px-8 py-8">
    <v-clicks>
      <div class="text-2xl leading-tight mb-4">на роботі вам платят за вклад, а не за години</div>
      <div class="text-2xl leading-tight mb-4">за каву ви платите за смак, а не за цінник</div>
      <div class="text-2xl leading-tight mb-4">у школі цінують розумінє, а не зубрінє</div>
      <div class="text-2xl leading-tight mb-4">дорожче означає не “статусніше”, а справді якісніше</div>
      <div class="text-2xl leading-tight">країну оцінюють по добробуту людей, а не по GDP</div>
    </v-clicks>
  </div>
</div>

<!--
Промова.

Уявіть собі такий світ.

Світ, де на роботі вам платят не за те, скільки часу ви просиділи, а за те, наскільки ви реально помогли спільній справі.
Де за каву ви платите не за бренд, не за інтер'єр і не за цінник, а просто за те, наскільки вона вам смакувала.
Де в школі цінують не слухняне відтворінє, а розумінє.
Де дорожче означає не “престижніше”, а справді ліпше.
Де країну судят не по GDP, а по тому, як там реально живеця людям.

Звучить якось нереально, правда?
Навіть трохи наївно.
Ніби так не буває.
Ніби так не прийнято думати.

Бо ми привикли чути зовсім інше.
-->

---

<div class="pt-2">
  <div class="eyebrow mb-4">культурний шум</div>
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

<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight" v-click>
  Зауважте: це не набір дурних фраз. Це одна й та сама логіка, просто в різних костюмах.
</div>

<!--
Промова.

Ми чуємо таке постійно.

“Де цифри?”
“А на еґзамені то буде?”
“Оцініть свій біль від нуля до десяти.”
“Школа не для того, шоб тобі подобалось.”
“Дорожче означає ліпше.”
“Якісне не може бути дешеве.”
“Може ти й чудова людина, але кредитний скор так не думає.”

Зауважте, шо це не просто окремі дурні фрази.
В них усіх є одна і та сама логіка.

Насправді нас цікавит вклад, але ми говорим про години.
Нас цікавит смак, але ми говорим про ціну.
Нас цікавит розумінє, але ми говорим про екзамен.
Нас цікавит людське життя, але ми говорим про скор, шкалу і показник.

То не випадковість.
Таке мисленє не виростає само.
Нам то насаджували дуже довго.
На впротязі тисячоліть.
-->

---

<div class="h-full flex flex-col justify-center items-center text-center">
  <div class="stamp mb-5">перехід до викриття</div>
  <div class="hero-title" style="font-size: 5.3rem; line-height: 0.95;">КОМУ ТО ВИГІДНО?</div>
  <div class="mt-10 text-2xl leading-tight max-w-3xl opacity-85">
    Чому школа, ринок, медицина і держава раптом однаково вірять не сутності, а її вимірюваному замінникові?
  </div>
</div>

<!--
Промова.

І отут починаєсє найцікавіше.

Бо якби це був просто збіг, то він був би надто вже системний.
Надто багато різних сфер раптом почали мислити однаково.
Школа, робота, медицина, економіка, держава, ринок, усі вони знов і знов підсовуют нам те саме:
не сутність, а її вимірюваний замінник.

То хто нас так перевчив?
Хто зробив так, шо ми вже самі говорим їхньою мовою?
Хто навчив нас більше довіряти шкалі, ніж досвідові,
більше довіряти ціннику, ніж смаку,
і більше довіряти показнику, ніж людині?
-->

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-7 py-7">
    <div class="eyebrow">суб'єкт цивілізаційного впливу</div>
    <h1 class="hero-title text-5xl mt-3 leading-none">ГЕОМЕТРИЧНО-ВИМІРУВАЛЬНИЙ КОМПЛЕКС</h1>
    <div class="mt-5 text-xl leading-snug max-w-2xl">
      Не одна школа. Не один бізнес. Не одна держава.
      Це коаліція всіх, кому потрібен світ, придатний до агрегування, порівняння і звітности.
    </div>
    <div class="mt-8 flex flex-wrap gap-3 text-sm">
      <span class="metric-chip">Братство прямої міри</span>
      <span class="metric-chip">культ вимірюваного</span>
      <span class="metric-chip">олівцево-лінійкове лобі</span>
      <span class="metric-chip">картель прикладної прямоти</span>
    </div>
  </div>

  <div class="col-span-2 axis-card px-5 py-5">
    <div class="eyebrow mb-3">псевдо-схема коаліції</div>
    <div class="grid grid-cols-2 gap-3 text-center text-sm h-full">
      <div class="panel-soft px-4 py-5 flex flex-col justify-center">
        <div class="text-3xl mb-2">▭</div>
        <div>таблиця</div>
      </div>
      <div class="panel-soft px-4 py-5 flex flex-col justify-center">
        <div class="text-3xl mb-2">◔</div>
        <div>dashboard</div>
      </div>
      <div class="panel-soft px-4 py-5 flex flex-col justify-center">
        <div class="text-3xl mb-2">⌁</div>
        <div>кадастр</div>
      </div>
      <div class="panel-soft px-4 py-5 flex flex-col justify-center">
        <div class="text-3xl mb-2">✓</div>
        <div>approved</div>
      </div>
    </div>
  </div>
</div>

<div class="mt-6 panel-soft px-6 py-4 text-2xl leading-tight">
  Вони не люблять сутність. Вони люблять її вимірюваний замінник.
</div>

<!--
Промова.

Тут ми вперше можемо назвати ворога.

Я не стверджую, що всім керують продавці лінійок і циркулів.
Але прошу звернути увагу, кому вигідний світ, у якому істинне тільки те, що можна поміряти.

Це не один бізнес, не одна школа, не одна держава.
Це широка цивілізаційна коаліція всіх, кому вигідний світ, у якому людське життя можна звести до керованих метрик.

Вони не люблять сутність. Вони люблять її вимірюваний замінник.
-->

---

<div class="pt-2">
  <div class="eyebrow mb-4">словник ворога</div>
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
  <div class="panel px-5 py-5 text-[var(--deck-accent)]">approved for management</div>
</div>

<div class="mt-8 text-2xl leading-tight max-w-4xl" v-click>
  Це не просто слова. Це їхні молитви.
</div>

<!--
Промова.

Подивіться на цю лексику.
Вона звучить дуже пристойно.
Майже доброчесно.

Але це не просто слова. Це їхні молитви.

Я не кажу, що диявол живе в Excel.
Але якби жив, йому би дуже подобалось слово “quantifiable”.

І зверніть увагу: майже всі ці слова звучать так, ніби вони не злі.
Саме в тому й сила культу.
-->

---

<div class="pt-2">
  <div class="eyebrow mb-4">тяглість цивілізаційної сили</div>
  <h1 class="hero-title text-6xl">ТЯГЛІСТЬ БРАТСТВА ПРЯМОЇ МІРИ</h1>
</div>

<div class="relative mt-10 px-4 py-10">
  <div class="timeline-track"></div>
  <div class="grid grid-cols-5 gap-4 relative">
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">пускова точка</div>
      <div class="text-xl leading-tight">Піфагорійці</div>
      <div class="small-note mt-2">секта, числа, дивні думки про фасолю</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">державний хребет</div>
      <div class="text-xl leading-tight">землеміри</div>
      <div class="small-note mt-2">кадастр, реєстр, межа</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">нормативний етап</div>
      <div class="text-xl leading-tight">стандартизована міра</div>
      <div class="small-note mt-2">легібельна держава</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">офісна мутація</div>
      <div class="text-xl leading-tight">Excel і KPI</div>
      <div class="small-note mt-2">dashboard як храм</div>
    </div>
    <div class="timeline-node px-4 py-5">
      <div class="text-sm uppercase opacity-60 mb-2">внутрішня колонія</div>
      <div class="text-xl leading-tight">quantified self</div>
      <div class="small-note mt-2">лінійка вже на зап'ясті</div>
    </div>
  </div>
</div>

<div class="panel-soft px-6 py-4 text-2xl leading-tight mt-2">
  Піфагорійці не зникли. Вони просто пройшли через кадастр і вийшли на smartwatch.
</div>

<!--
Промова.

Це важливо бачити не як набір випадкових епізодів, а як тяглу лінію однієї й тієї самої сили.

Піфагорійці не зникли. Вони просто пройшли через кадастр і вийшли на smartwatch.

Щоб ви розуміли, це не були просто математики.
Це були люди, які одночасно обожнювали числа і ненавиділи фасолю.

Культ вимірювання починається, що показово, з секти, яка мала дуже сильні думки про боби.
Після того він просто став респектабельнішим.
-->

---

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="axis-card px-6 py-6">
    <div class="eyebrow mb-4">дозволені графіки</div>
    <div class="grid grid-cols-2 gap-4">
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
    <div class="forbidden-label mb-4">заборонений графік</div>
    <div style="height: 18rem;">
      <svg viewBox="0 0 320 260" fill="none">
        <path d="M162 131 C162 131, 185 122, 192 137 C199 152, 175 171, 151 170 C119 168, 97 138, 104 103 C112 63, 155 42, 198 54 C247 68, 274 120, 259 171 C240 235, 167 257, 103 239 C27 218, -2 124, 33 57" stroke="#cf785d" stroke-width="6" stroke-linecap="round" />
        <circle cx="245" cy="60" r="11" fill="#d6b25e" opacity="0.95" />
        <circle cx="88" cy="204" r="8" fill="#79b5a8" opacity="0.9" />
        <circle cx="204" cy="198" r="6" fill="#f3ecdf" opacity="0.8" />
      </svg>
    </div>
    <div class="text-2xl leading-tight mt-3">
      Свобода є. Але лише в межах обліку.
    </div>
    <div class="small-note mt-3">Нам ніколи не дозволять мати такий графік.</div>
  </div>
</div>

<!--
Промова.

Це один із найчесніших слайдів у всій презентації.

Зауважте: нам дають вибір.
Але тільки між формами, придатними до порівняння.

Bar, line, pie, scatter, area.
Свобода є.
Але лише в межах обліку.

Нам ніколи не дозволять мати такий графік.
Бо він гарний, складний, живий і погано масштабується в KPI.
-->

---

<div class="pt-2">
  <div class="eyebrow mb-3">механіка корупції метрики</div>
  <h1 class="hero-title text-6xl">КОЛИ ЧИСЛО СТАЄ ЦІЛЛЮ</h1>
  <div class="text-2xl opacity-80 mt-2">Закон Гудгарта</div>
</div>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div class="case-card px-5 py-5">
    <div class="stamp mb-4">cobra effect</div>
    <div class="text-2xl leading-tight">боролись не з кобрами</div>
    <div class="small-note mt-3">оптимізували виробництво кобр</div>
  </div>
  <div class="case-card px-5 py-5">
    <div class="stamp mb-4">body count</div>
    <div class="text-2xl leading-tight">число виглядає рішучим</div>
    <div class="small-note mt-3">навіть коли правда вже втекла</div>
  </div>
  <div class="case-card px-5 py-5">
    <div class="stamp mb-4">офісний кейс</div>
    <div class="text-2xl leading-tight">ідеальний працівник</div>
    <div class="small-note mt-3">пише “ок” за 0.3 секунди</div>
  </div>
</div>

<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight">
  Коли число стає ціллю, правда починає удавати число.
</div>

<!--
Промова.

Тут механіка проста.
Як тільки число стає ціллю, система починає виробляти не правду, а саме число.

Коли число стає ціллю, правда починає удавати число.

Вони не боролися з кобрами. Вони оптимізували виробництво кобр.

Якщо міряти дружбу кількістю повідомлень, найкращі стосунки будуть з чат-ботами.
Якщо міряти університет рейтингом, він починає не вчити, а виглядати рейтингово.
Якщо міряти роботу швидкістю відповіді, ідеальний працівник пише “ок” за 0.3 секунди.

Як тільки ви починаєте винагороджувати число, люди починають виробляти число.
-->

---

<div class="grid grid-cols-2 gap-6 pt-2 items-stretch">
  <div class="panel px-6 py-6">
    <div class="eyebrow mb-4">міфологічний прецедент</div>
    <h1 class="hero-title text-5xl leading-none">КОМЕНСУРАЦІЯ</h1>
    <div class="text-2xl opacity-80 mt-2">Як принизити людину метриками</div>
    <div class="mt-8 panel-soft px-5 py-5 text-xl leading-snug">
      Прокруст брав мандрівника і підганяв його під ложе.
      Якщо не влазив, відрізав зайве.
      Якщо був замалий, дотягував.
    </div>
    <div class="mt-6 text-2xl leading-tight">
      Принизити людину метриками — це спочатку зробити її порівнюваною.
    </div>
  </div>

  <div class="panel px-6 py-6">
    <div class="eyebrow mb-4">демонстраційне порівняння</div>
    <table class="data-table">
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
    <div class="small-note mt-5">Ми попали в їхню пастку, пробуючи порівняти їх.</div>
  </div>
</div>

<!--
Промова.

Насильство метрики починається не тоді, коли ми щось порахували.
Воно починається тоді, коли ми різні речі кладемо на одну вісь і називаємо це нейтральним.

Прокруст — це не міф. Це архетип усіх систем оцінювання.

Щойно ми погодились на порівняння, ми вже прийняли їхню владу.
Ми попали в їхню пастку, пробуючи порівняти їх.

Лінійка не просто міряє світ. Вона навчає світ соромитися кривизни.
-->

---

<div class="pt-2">
  <div class="eyebrow mb-4">сухий кейсовий блок</div>
  <h1 class="hero-title text-6xl">ЖЕРТВИ ЛІНІЙКИ</h1>
</div>

<div class="grid grid-cols-2 gap-5 mt-8">
  <div class="victim-card px-5 py-5">
    <div class="stamp mb-3">медицина</div>
    <div class="text-2xl leading-tight">пацієнт, якому “ще не досить болить по шкалі”</div>
  </div>
  <div class="victim-card px-5 py-5">
    <div class="stamp mb-3">робота</div>
    <div class="text-2xl leading-tight">працівник, який “не проходить по KPI”</div>
  </div>
  <div class="victim-card px-5 py-5">
    <div class="stamp mb-3">освіта</div>
    <div class="text-2xl leading-tight">дитина, яку тест переводить у “середній рівень”</div>
  </div>
  <div class="victim-card px-5 py-5">
    <div class="stamp mb-3">соціальна видимість</div>
    <div class="text-2xl leading-tight">людина, яка справді мудра, але неформалізована</div>
  </div>
</div>

<div class="panel-soft mt-8 px-6 py-5 text-2xl leading-tight">
  Система не бачить вас повністю. Вона бачить вас настільки, наскільки вас можна ранжувати.
</div>

<!--
Промова.

Тут уже не смішно, а просто сухо видно шкоду.

Вони кажуть, що цифри прибирають суб'єктивність.
Але дуже часто вони просто прибирають людину.

Пацієнт має біль, але його біль мусить пройти через шкалу.
Працівник має реальний вклад, але система питає тільки про KPI.
Дитина має спосіб думати, але тест перетворює її на рівень.
Людина може бути мудра, але якщо це не переводиться в сертифікат, система не має для неї поля.

Система не бачить вас повністю. Вона бачить вас настільки, наскільки вас можна ранжувати.
-->

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6">
    <div class="eyebrow mb-4">поле без адміністративної ваги</div>
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
    <div>
      <div class="eyebrow mb-4">фінальний приклад</div>
      <div class="grid grid-cols-2 gap-3">
        <div class="panel-soft px-4 py-4">
          <div class="text-sm uppercase opacity-60 mb-2">GDP</div>
          <div class="text-xl leading-tight">добре бачить виробництво</div>
        </div>
        <div class="panel-soft px-4 py-4">
          <div class="text-sm uppercase opacity-60 mb-2">Gross National Happiness</div>
          <div class="text-xl leading-tight">ставить незручне питання про життя</div>
        </div>
      </div>
    </div>
    <div class="void-stamp mt-5">нерепортоване не означає неіснуюче</div>
  </div>
</div>

<div class="mt-6 grid grid-cols-2 gap-4 text-xl">
  <div class="panel-soft px-5 py-4">Ніжність не заборонена. Вона просто не має бюджетного рядка.</div>
  <div class="panel-soft px-5 py-4">Гідність існує, але не в дашборді.</div>
</div>

<!--
Промова.

Один із найсильніших ефектів системи в тому, що вона не мусить прямо забороняти важливі речі.
Достатньо зробити їх адміністративно неіснуючими.

Нема одиниці виміру, нема обіцянки, нема звітности, нема реальности.

Ніжність не заборонена. Вона просто не має бюджетного рядка.
Гідність існує, але не в дашборді.

GDP чудово бачить виробництво.
Але дуже погано бачить, чи взагалі варто було так жити.
-->

---

<div class="grid grid-cols-5 gap-6 pt-2 items-stretch">
  <div class="col-span-3 panel px-6 py-6 circumplex">
    <div class="eyebrow mb-4">Excel для душі</div>
    <h1 class="hero-title text-5xl leading-none">ЕМОЦІЙНИЙ ЦИРКУМПЛЕКС</h1>
    <div class="text-2xl opacity-80 mt-2">дві санкціоновані осі для внутрішнього життя</div>
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
      Нам дозволили мати емоції, але лише двовимірні.
    </div>
    <div class="panel-soft px-4 py-4 mt-5 text-xl leading-snug">
      Емоційний циркумплекс — це прокрустове ложе для внутрішнього життя.
    </div>
  </div>
</div>

<!--
Промова.

Ось момент, де змова доходить до внутрішнього життя.

Нам дозволили мати емоції, але лише двовимірні.

Емоційний циркумплекс зручний.
Саме тому він такий підозрілий.
Він добре працює для вимірювання, але погано поводиться зі змішаними станами.

Бути одночасно злим і веселим адміністративно незручно.

Емоційний циркумплекс — це прокрустове ложе для внутрішнього життя.
Проблема не в тому, що модель проста.
Проблема в тому, що вона принижує змішані стани до помилки вимірювання.
-->

---

<div class="grid grid-cols-5 gap-6 pt-2 items-center">
  <div class="col-span-2 panel px-6 py-6">
    <div class="eyebrow mb-4">кульмінація</div>
    <h1 class="hero-title text-5xl leading-none">ОСТАННЯ СТАДІЯ ЗМОВИ</h1>
    <div class="text-2xl opacity-80 mt-2">Quantified Self</div>
    <div class="mt-8 space-y-3 text-xl leading-snug">
      <div>раніше людину міряли ззовні</div>
      <div>потім її навчили мислити метриками</div>
      <div>тепер вона добровільно носить dashboard на собі</div>
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

<div class="panel-soft mt-6 px-6 py-5 text-2xl leading-tight">
  Остання стадія змови — коли жертва сама купує собі датчик.
</div>

<!--
Промова.

Оце і є кульмінація.

Раніше вони носили лінійку в руці.
Тепер ми носимо її на зап'ясті.

Остання стадія змови — коли жертва сама купує собі датчик.

Раніше людину міряли ззовні.
Потім її навчили мислити метриками.
Тепер вона добровільно перетворює себе на dashboard.

Self-knowledge through numbers — це коли самопізнання вже остаточно перейшло на бік нагляду.
-->

---

<div class="h-full flex flex-col justify-between pt-4 pb-4">
  <div>
    <div class="eyebrow mb-4">фінал</div>
    <h1 class="hero-title text-6xl">ЩО ВОНИ ХОЧУТЬ?</h1>
  </div>

  <div class="panel px-8 py-8">
    <div class="final-quote">
      Найуспішніша маніпуляція не в тому, щоб знищити невимірюване.
      А в тому, щоб зробити його несерйозним.
    </div>
  </div>

  <div class="grid grid-cols-4 gap-4 text-center text-lg">
    <div class="panel-soft px-4 py-4">спершу міряли світ</div>
    <div class="panel-soft px-4 py-4">потім людей</div>
    <div class="panel-soft px-4 py-4">потім емоції</div>
    <div class="panel-soft px-4 py-4">тепер люди міряють себе самі</div>
  </div>

  <div class="text-2xl leading-tight max-w-4xl opacity-85">
    Ми не в світі, де все міряють. Ми в світі, де неміряне мусить виправдовуватись.
  </div>
</div>

<!--
Промова.

Тут важливо не моралізувати.
Треба просто назвати їхню справжню перемогу.

Їхня перемога не в тому, що вони все виміряли.
Їхня перемога в тому, що ми вже самі автоматично довіряємо шкалі більше, ніж досвідові.

Найуспішніша маніпуляція не в тому, щоб знищити невимірюване.
А в тому, щоб зробити його несерйозним.

Вони не забрали в нас душу.
Вони просто зробили її нерепортованою.

Ми не в світі, де все міряють.
Ми в світі, де неміряне мусить виправдовуватись.
-->

