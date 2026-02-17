# GOATA-Lab---Dominika-Cerna
GOATA Lab - Dominika Cerna
<!doctype html>
<html lang="cs">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>GOATA Lab by Dominika Černá – přirozený pohyb bez bolesti</title>
  <meta name="description" content="GOATA instruktorka, trenérka a průvodkyně. Úvodní posouzení pohybu, individuální a skupinové tréninky v Praze i online. Návrat k přirozenému pohybu, prevence zranění, lepší výkon." />

  <style>
    :root{
      --bg: #fbf7f0;          /* teplá slonová kost */
      --card: #ffffff;
      --text: #1f2430;        /* seriózní tmavá modro-šedá */
      --muted: #5b6474;
      --line: rgba(31,36,48,.10);
      --accent: #c07a52;      /* jemná terakota */
      --accent-2: #e7c7a4;    /* písková */
      --shadow: 0 10px 30px rgba(31,36,48,.08);
      --radius: 18px;
      --max: 1040px;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Noto Sans", "Liberation Sans", sans-serif;
      color:var(--text);
      background:
        radial-gradient(900px 500px at 15% 10%, rgba(231,199,164,.45), transparent 60%),
        radial-gradient(900px 500px at 85% 15%, rgba(192,122,82,.18), transparent 60%),
        var(--bg);
      line-height:1.6;
    }

    a{color:inherit}
    html{scroll-behavior:smooth}

    .wrap{max-width:var(--max); margin:0 auto; padding:26px 18px 84px}
    .topbar{
      display:flex; align-items:center; justify-content:space-between;
      gap:12px;
      position:sticky; top:0;
      padding:14px 0;
      backdrop-filter: blur(8px);
      z-index:10;
    }

    .brand{
      display:flex; align-items:center; gap:10px; text-decoration:none;
      min-width: 220px;
    }
    .logo{
      width:34px; height:34px; border-radius:10px;
      background: linear-gradient(135deg, var(--accent-2), rgba(192,122,82,.35));
      border:1px solid var(--line);
      box-shadow: 0 6px 16px rgba(31,36,48,.07);
    }
    .brand b{font-weight:700}
    .brand span{display:block; font-size:12px; color:var(--muted); margin-top:2px}

    .nav{
      display:flex; gap:10px; flex-wrap:wrap;
      font-size:14px;
      justify-content:flex;
    }
    .nav a{
      text-decoration:none;
      padding:8px 10px;
      border-radius:999px;
      border:1px solid transparent;
      color:var(--muted);
      background: transparent;
    }
    .nav a:hover{border-color:var(--line); color:var(--text); background:rgba(255,255,255,.55)}

    .card{
      background: rgba(255,255,255,.72);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }

    .hero{
      margin-top:10px;
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:18px;
      align-items:stretch;
    }
    @media (max-width: 920px){
      .hero{grid-template-columns:1fr}
      .topbar{position:static}
      .brand{min-width:auto}
    }

    .hero-left{padding:28px}
    .kicker{
      display:inline-flex; align-items:center; gap:8px;
      font-size:13px; color:var(--muted);
      padding:8px 12px;
      border:1px solid var(--line);
      border-radius:999px;
      background:rgba(255,255,255,.55);
    }
    .dot{
      width:8px; height:8px; border-radius:99px;
      background: var(--accent);
      box-shadow: 0 0 0 6px rgba(192,122,82,.16);
    }

    h1{
      margin:14px 0 10px;
      font-size:42px;
      letter-spacing:-.02em;
      line-height:1.12;
    }
    @media (max-width: 520px){ h1{font-size:34px} }

    .lead{color:var(--muted); font-size:16px; margin:0 0 18px}
    .cta{display:flex; gap:10px; flex-wrap:wrap; margin-top:18px}
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:10px;
      padding:10px 14px;
      border-radius:12px;
      border:1px solid var(--line);
      text-decoration:none;
      font-weight:650;
      font-size:14px;
      background:rgba(255,255,255,.65);
      cursor:pointer;
    }
    .btn.primary{
      border-color: rgba(192,122,82,.35);
      background: linear-gradient(135deg, rgba(231,199,164,.65), rgba(192,122,82,.18));
    }
    .btn:hover{transform: translateY(-1px)}

    .meta{
      display:grid; gap:10px;
      padding:22px;
    }
    .meta h3{margin:0 0 4px; font-size:13px; color:var(--muted); font-weight:750; letter-spacing:.02em; text-transform:uppercase}
    .meta p{margin:0; font-size:14px}
    .meta .item{
      padding:14px;
      border:1px solid var(--line);
      border-radius:14px;
      background:rgba(255,255,255,.55);
    }

    section{margin-top:18px}
    .section{padding:22px}
    .section h2{margin:0 0 10px; font-size:18px; letter-spacing:-.01em}

    .grid3{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
      margin-top:12px;
    }
    @media (max-width: 920px){ .grid3{grid-template-columns:1fr} }

    .two{
      display:grid; grid-template-columns:1fr 1fr; gap:12px;
      margin-top:12px;
    }
    @media (max-width: 920px){ .two{grid-template-columns:1fr} }

    .feature{
      padding:16px;
      border:1px solid var(--line);
      border-radius:14px;
      background:rgba(255,255,255,.55);
    }
    .feature b{display:block; margin-bottom:6px}
    .feature p{margin:0; color:var(--muted); font-size:14px}

    .quote{
      font-size:14px;
      color:var(--muted);
      border-left: 3px solid rgba(192,122,82,.55);
      padding-left:12px;
      margin:10px 0 0;
    }

    .pillrow{display:flex; gap:8px; flex-wrap:wrap; margin-top:10px}
    .pill{
      font-size:12px;
      color:var(--muted);
      padding:7px 10px;
      border:1px solid var(--line);
      border-radius:999px;
      background:rgba(255,255,255,.55);
    }

    .contact{
      display:grid; grid-template-columns:1.2fr .8fr; gap:12px;
      margin-top:12px;
    }
    @media (max-width: 920px){ .contact{grid-template-columns:1fr} }

    form{display:grid; gap:10px}
    label{font-size:13px; color:var(--muted)}
    input, textarea{
      width:100%;
      padding:11px 12px;
      border-radius:12px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.7);
      font:inherit;
    }
    textarea{min-height:110px; resize:vertical}
    .small{font-size:12px; color:var(--muted)}
    .hint{margin-top:8px}

    .price{
      display:flex; align-items:baseline; justify-content:space-between; gap:14px;
    }
    .price strong{font-size:16px}
    .price span{color:var(--muted); font-size:13px}

    .maplink{display:inline-block; margin-top:10px; font-size:14px; color:var(--muted)}
    .maplink:hover{color:var(--text)}

    footer{
      margin-top:22px;
      padding-top:18px;
      border-top:1px solid var(--line);
      color:var(--muted);
      font-size:13px;
      display:flex;
      justify-content:space-between;
      gap:12px;
      flex-wrap:wrap;
    }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="topbar">
      <a class="brand" href="#top">
        <span class="logo" aria-hidden="true"></span>
        <div>
          <b>GOATA Lab</b>
          <span>by Dominika Černá</span>
        </div>
      </a>

      <nav class="nav" aria-label="Navigace">
        <a href="#o-mne">O mně</a>
        <a href="#nabidka">Nabídka</a>
        <a href="#cenik">Ceník</a>
        <a href="#misto">Kde</a>
        <a href="#kontakt">Registrace</a>
      </nav>
    </div>

    <main id="top" class="hero">
      <div class="card hero-left">
        <div class="kicker"><span class="dot"></span> Přirozený pohyb • výkon • prevence zranění</div>

        <h1>Návrat těla k přirozenému pohybu.<br/>
          Jemně, přesně a <span style="color:var(--accent)">dlouhodobě</span>.
        </h1>

        <p class="lead">
          Jsem GOATA instruktorka, trenérka a průvodkyně. Pomáhám lidem na cestě „recode“ – přepisování
          pohybových stereotypů tak, aby tělo fungovalo odolněji, s menším přetížením a bez zbytečné bolesti.
        </p>

        <div class="pillrow" aria-label="Pro koho je GOATA vhodná">
          <span class="pill">bolesti pohybového aparátu</span>
          <span class="pill">prevence zranění</span>
          <span class="pill">tanečníci</span>
          <span class="pill">vrcholový sport</span>
          <span class="pill">zlepšení výkonu</span>
        </div>

        <div class="cta">
          <a class="btn primary" href="#kontakt">Registrovat úvodní posouzení</a>
          <a class="btn" href="#cenik">Zobrazit ceník</a>
        </div>

        <p class="quote">GOATA není jen cvičení. Je to životní styl postavený na globálních zákonech přirozeného pohybu.</p>
      </div>

      <aside class="card meta" aria-label="Rychlé info">
        <div class="item">
          <h3>Lokalita</h3>
          <p>Praha • online</p>
        </div>
        <div class="item">
          <h3>Studio</h3>
          <p>Patočkova 83<br/>Studio Barre Prague</p>
        </div>
        <div class="item">
          <h3>Kontakt</h3>
          <p>
            <a href="mailto:Dominika.c.9@icloud.com">Dominika.c.9@icloud.com</a><br/>
            <a href="tel:+420607603554">+420 607 603 554</a>
          </p>
        </div>
      </aside>
    </main>

    <section id="o-mne" class="card section">
      <h2>O mně</h2>
      <div class="two">
        <div>
          <p class="lead" style="margin:0">
            V praxi kombinuji pozorování pohybu, cílenou korekci a vlastní pohybovou praxi.
            Cílem není „jen si zacvičit“, ale pochopit souvislosti a přenést změny do běžného dne i sportu.
          </p>
          <p class="small hint">
            Pokud si nejste jistí, kde začít, doporučuji úvodní posouzení pohybu – dá nám jasný směr.
          </p>
        </div>
        <div class="feature">
          <b>Můj přístup</b>
          <p>
            • srozumitelně a bez tlaku<br/>
            • důraz na techniku a detail<br/>
            • postupně a udržitelně
          </p>
        </div>
      </div>
    </section>

    <section id="nabidka" class="card section">
      <h2>Nabídka</h2>
      <p class="lead" style="margin:0">
        Začínáme diagnostikou a postupně přepisujeme pohybové vzorce – tak, aby tělo zvládalo zátěž odolněji.
      </>

      <div class="grid3">
        <div class="feature">
          <b>Úvodní posouzení pohybu</b>
          <p>
            Pomocí slow motion videa se podíváme, jak tělo funguje v základních vzorcích pohybu.
            Dostanete první sadu cviků a jasné doporučení dalšího postupu.
          </p>
        </div>
        <div class="feature">
          <b>Individuální tréninky</b>
          <p>
            Přepisování zajetých stereotypů na nové, odolnější. Vysvětlím „proč“ a „jak“,
            abyste změny udrželi i mimo trénink.
          </p>
        </div>
        <div class="feature">
          <b>Pohybová praxe & edukace</b>
          <p>
            Nezbytnou součástí je vlastní pravidelná praxe. Součástí je i edukace o globálních zákonech,
            kterými se GOATA řídí.
          </p>
        </div>
      </div>
    </section>

    <section id="cenik" class="card section">
      <h2>Ceník</h2>
      <div class="two">
        <div class="feature">
          <div class="price">
            <strong>Individuální lekce</strong>
            <span>60 min (dle domluvy)</span>
          </div>
          <p style="margin:8px 0 0; color:var(--muted)">
            Cena: <b style="color:var(--text)">1 700 Kč</b>
          </p>
        </div>

        <div class="feature">
          <div class="price">
            <strong>Skupinový trénink</strong>
            <span>lekce ve studiu</span>
          </div>
          <p style="margin:8px 0 0; color:var(--muted)">
            Cena: <b style="color:var(--text)">450 Kč</b>
          </p>
        </div>
      </div>

      <p class="small" style="margin:12px 0 0">
        Pozn.: Úvodní posouzení pohybu ráda nacením a potvrdím podle domluvy (čas, forma, potřeby).
        Pokud chcete, doplním sem i pevnou cenu za posouzení.
      </p>
    </section>

    <section id="misto" class="card section">
      <h2>Kde trénujeme</h2>
      <div class="two">
        <div class="feature">
 <b>Praha</b>
          <p>Patočkova 83, Studio Barre Prague</p>
          <a class="maplink" target="_blank" rel="noreferrer"
             href="https://www.google.com/maps/search/?api=1&query=Pato%C4%8Dkova%2083%2C%20Praha%2C%20Studio%20Barre%20Prague">
            Otevřít v Google Maps →
          </a>
        </div>
        <div class="feature">
          <b>Online</b>
          <p>
            Konzultace, posouzení i trénink mohou proběhnout také online. Dopředu Vám řeknu,
            co budete potřebovat (prostor, obuv / naboso, jednoduché pomůcky).
          </p>
        </div>
      </div>
    </section>

    <section id="kontakt" class="card section">
      <h2>Registrace – úvodní posouzení pohybu</h2>
      <p class="lead" style="margin:0">
        Vyplňte prosím krátký formulář. Ozvu se Vám s návrhem termínu a dalším postupem.
      </p>

      <div class="contact">
        <div class="feature">
          <b>Registrační formulář</b>

          <!-- ZATÍM DEMO (neodesílá).
               Až budete chtít Formspree:
               1) vytvoříte formulář ve Formspree
               2) sem do action vložíme URL a smažeme onsubmit -->
          <form onsubmit="return demoSubmit(event)">
            <div>
              <label for="name">Jméno</label>
              <input id="name" name="jmeno" autocomplete="name" placeholder="Vaše jméno" required />
            </div>

            <div>
              <label for="phone">Telefon</label>
              <input id="phone" name="telefon" inputmode="tel" autocomplete="tel"
                     placeholder="+420…" required />
            </div>

            <div>
              <label for="why">Proč chcete přijít</label>
              <textarea id="why" name="proc_chci_prijit" placeholder="Co chcete zlepšit / vyřešit?" required></textarea>
            </div>

            <div>
              <label for="history">Pohybová minulost</label>
              <textarea id="history" name="pohybova_minulost" placeholder="Sport, tanec, tréninková rutina, práce…"></textarea>
            </div>

            <div>
              <label for="injuries">Zranění nebo operace v minulosti</label>
              <textarea id="injuries" name="zraneni_operace" placeholder="Kdy, co, jak se to projevuje dnes…"></textarea>
            </div>

            <div>
              <label for="pain">Bolesti v současnosti</label>
              <textarea id="pain" name="bolesti_soucasnost" placeholder="Kde bolí, kdy to začíná, co zhoršuje/zlepšuje…"></textarea>
            </div>

            <button class="btn primary" type="submit">Odeslat (zatím demo)</button>
            <div class="small" id="formNote">Formulář je aktuálně zkušební – nic se nikam neodesílá.</div>
          </form>

          <p class="small" style="margin:10px 0 0">
            Alternativně mi můžete napsat e-mail nebo zavolat.
          </p>
        </div>

        <div class="feature">
          <b>Přímý kontakt</b>
          <p style="margin:0; color:var(--muted); font-size:14px">
            E-mail: <a href="mailto:Dominika.c.9@icloud.com">Dominika.c.9@icloud.com</a><br/>
            Telefon: <a href="tel:+420607603554">+420 607 603 554</a><br/>
            Lokalita: Praha / online
          </p>

          <p class="small" style="margin-top:12px">
            Až budete chtít, přidáme: reálné odesílání formuláře (Formspree zdarma), potvrzovací zprávu,
            a krátké GDPR info (doporučeno).
          </p>
        </div>
      </div>
    </section>

    <footer>
      <div>© <span id="y"></span> GOATA Lab by Dominika Černá</div>
      <div><a href="#top" style="text-decoration:none">Nahoru ↑</a></div>
    </footer>
  </div>

  <script>
    document.getElementById("y").textContent = new Date().getFullYear();

    function demoSubmit(e){
      e.preventDefault();
      const note = document.getElementById("formNote");
      note.textContent = "Děkuji! (Demo) Formulář je vyplněný. Až napojíme Formspree, bude se odesílat na e-mail.";
      return false;
    }
  </script>
</body>
</html>
