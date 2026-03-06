<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Nanohabit · Apple Watch Apps · Watch2o and BioBattery</title>
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <meta name="description" content="Nanohabit builds focused Apple Watch apps. Watch2o helps you track daily water intake. BioBattery shows your social energy level so you can decide on evening plans.">
  <meta name="theme-color" content="#0b0b0c">
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Ccircle cx='32' cy='32' r='30' fill='%23000'/%3E%3Cpath d='M32 13l12 19H20L32 13zm0 38l-12-19h24L32 51z' fill='%23fff'/%3E%3C/svg%3Eeta property="og:type" content="website">
  <meta property="og:url" content="https://nanohabit.github.io/">
  <meta property="og:image" content="https://nanohabit.github.io/cover.png">

  <!-- Twitter Card -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="Nanohabit · Apple Watch Apps">
  <meta name="twitter:description" content="Watch2o and BioBattery for Apple Watch. Simple, private, and fast.">
  <meta name="twitter:image" content="https://nanohabit.github.io/cover.png">

  <!-- JSON-LD -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Organization",
    "name": "Nanohabit",
    "url": "https://nanohabit.github.io/",
    "logo": "https://nanohabit.github.io/logo.png",
    "sameAs": ["https://github.com/bawary"],
    "department": [
      {
        "@type": "SoftwareApplication",
        "name": "Watch2o",
        "applicationCategory": "HealthApplication",
        "operatingSystem": "watchOS",
        "offers": {"@type": "Offer", "price": "0", "priceCurrency": "EUR"}
      },
      {
        "@type": "SoftwareApplication",
        "name": "BioBattery",
        "applicationCategory": "HealthApplication",
        "operatingSystem": "watchOS",
        "offers": {"@type": "Offer", "price": "0", "priceCurrency": "EUR"}
      }
    ]
  }
  </script>

  <style>
    :root{
      --bg:#0b0b0c;
      --bg-soft:#121214;
      --card:#151518;
      --text:#e8e8eb;
      --muted:#b5b5be;
      --accent:#5ac8fa; /* Apple-like blue */
      --accent-2:#34c759; /* Apple green */
      --border:rgba(255,255,255,0.08);
      --shadow:0 10px 30px rgba(0,0,0,0.45);
      --radius:16px;
      --font:-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    }
    @media (prefers-color-scheme: light){
      :root{
        --bg:#fafafa;
        --bg-soft:#ffffff;
        --card:#ffffff;
        --text:#0b0b0c;
        --muted:#51525a;
        --border:rgba(0,0,0,0.08);
        --shadow:0 8px 24px rgba(0,0,0,0.08);
      }
    }

    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font-family:var(--font);line-height:1.6}
    a{color:var(--accent);text-decoration:none}
    a:hover{text-decoration:underline}
    .wrap{max-width:1120px;margin:0 auto;padding:0 20px}
    header.nav{
      position:sticky;top:0;z-index:50;
      backdrop-filter:saturate(180%) blur(16px);
      background:color-mix(in oklab, var(--bg-soft) 80%, transparent);
      border-bottom:1px solid var(--border);
    }
    .nav-inner{display:flex;align-items:center;justify-content:space-between;height:64px}
    .brand{display:flex;gap:12px;align-items:center}
    .brand .logo{
      width:28px;height:28px;border-radius:7px;background:linear-gradient(135deg,var(--accent),#007aff 60%,#0047ff);
      box-shadow:0 6px 18px rgba(0,122,255,0.35);
    }
    .brand span{font-weight:700;letter-spacing:0.2px}
    .nav a{margin-left:18px;color:var(--text);opacity:0.8}
    .nav a:hover{opacity:1}
    .hero{
      padding:84px 0 48px;background:
        radial-gradient(800px 240px at 20% 0%, rgba(90,200,250,0.18), transparent 60%),
        radial-gradient(800px 240px at 80% -20%, rgba(52,199,89,0.20), transparent 60%),
        var(--bg);
      border-bottom:1px solid var(--border);
    }
    .hero h1{font-size:42px;line-height:1.15;margin:0 0 12px;letter-spacing:-0.4px}
    .hero p{color:var(--muted);max-width:720px;margin:0 0 28px}
    .cta{display:flex;gap:12px;flex-wrap:wrap}
    .btn{
      display:inline-flex;align-items:center;gap:10px;
      padding:12px 16px;border-radius:12px;border:1px solid var(--border);
      background:linear-gradient(180deg,var(--card),color-mix(in srgb, var(--card) 80%, #000 20%));
      color:var(--text);box-shadow:var(--shadow);
    }
    .btn:hover{transform:translateY(-1px)}
    .grid{
      display:grid;gap:24px;margin:42px 0;
      grid-template-columns:repeat(12,1fr)
    }
    .card{
      background:var(--card);border:1px solid var(--border);border-radius:var(--radius);padding:22px;
      box-shadow:var(--shadow)
    }
    .card h3{margin:0 0 8px}
    .two{grid-column:span 6}
    .three{grid-column:span 4}
    @media (max-width:900px){.two,.three{grid-column:span 12}}
    .apps{padding:42px 0}
    .app{
      display:grid;grid-template-columns:160px 1fr;gap:22px;align-items:center
    }
    @media (max-width:640px){.app{grid-template-columns:1fr}}
    .watch{
      width:160px;height:160px;border-radius:28px;background:linear-gradient(145deg,#111,#1a1a1d);
      border:1px solid var(--border);display:flex;align-items:center;justify-content:center;
      color:#fff;font-weight:700;letter-spacing:1px
    }
    .tag{display:inline-block;padding:4px 10px;border-radius:999px;border:1px solid var(--border);
      background:var(--bg-soft);font-size:12px;color:var(--muted);margin-bottom:8px}
    .badges{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}
    .badge{
      display:inline-flex;align-items:center;gap:10px;padding:10px 14px;border-radius:12px;border:1px solid var(--border);
      background:var(--bg-soft);color:var(--text)
    }
    .features{padding:18px 0 8px}
    .features li{margin:6px 0}
    .footer{
      padding:38px 0;color:var(--muted);border-top:1px solid var(--border)
    }
    .mono{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace}
    .kicker{font-size:14px;color:var(--muted);margin-bottom:8px}
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
    details{border:1px solid var(--border);border-radius:12px;background:var(--card);padding:18px}
    details summary{cursor:pointer;font-weight:600;margin-bottom:8px}
    .legal a{color:inherit;text-decoration:underline}
  </style>
</head>
<body>
  <header class="nav">
    <div class="wrap nav-inner">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <span>Nanohabit</span>
      </div>
      <nav class="nav" aria-label="Primary">
        <a href="#apps        #privacyPrivacy</a>
        #contactContact</a>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="wrap">
      <span class="kicker">Apple Watch Apps</span>
      <h1>Simple, private, and fast.</h1>
      <p>Nanohabit builds focused Apple Watch apps that respect your time and your data. Watch2o helps you track daily water intake. BioBattery shows your social energy level so you can decide on evening plans.</p>
      <div class="cta">
        <a class="btn" href="#apps" role="button" aria="#privacy" role="button" aria-label="Read privacy     <div class="two card">
          <h3>Private by design</h3>
          <p>No accounts. No analytics. No ads. Data stays on your device.</p>
        </div>
        <div class="two card">
          <h3>Built for watchOS</h3>
          <p>Glanceable interfaces, smooth performance, and useful complications.</p>
        </div>
        <div class="two card">
          <h3>Clean and focused</h3>
          <p>Each app does one job exceptionally well.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="apps" class="apps">
    <div class="wrap">
      <h2>Apps</h2>

      <!-- Watch2o -->
      <article class="card app" aria-labelledby="watch2o-title">
        <div class="watch" aria-hidden="true">Watch2o</div>
        <div>
          <span class="tag">Health and Fitness</span>
          <h3 id="watch2o-title">Watch2o</h3>
          <p>Fast, simple water intake tracking on Apple Watch. Optional HealthKit write for Water. No external storage.</p>
          <ul class="features">
            <li>One tap logging</li>
            <li>Complications for quick access</li>
            <li>Optional HealthKit write for water intake</li>
            <li>No accounts or analytics</li>
          </ul>
          <div class="badges">
            <a class="badge" href="YOUR_APPSTORE_LINK_WATCH2O" aria-label="View Watch2o on the App class="badge" href="https://github.com/bawary/div>
        </div>
      </article>

      <!-- BioBattery -->
      <article class="card app" aria-labelledby="biobattery-title" style="margin-top:22px">
        <div class="watch" aria-hidden="true">BioBattery</div>
        <div>
          <span class="tag">Health and Fitness</span>
          <h3 id="biobattery-title">BioBattery</h3>
          <p>See your current energy level so you can decide whether you are ready for social plans or need time to recharge.</p>
          <ul class="features">
            <li>Clear energy indicator on your wrist</li>
            <li>Designed for Apple Watch with complications</li>
            <li>No health data required</li>
            <li>Private and lightweight</li>
          </ul>
          <div class="badges">
            <a class="badge" href="YOUR_APPSTORE_LINK_BIOBATTERY" aria-label="View BioBattery on the Appass="badge" href="https://github.com/bawary" rel
        </div>
      </article>
    </div>
  </section>

  <section id="privacy" class="apps">
    <div class="wrap">
      <h2>Privacy Policy</h2>
      <details open class="legal">
        <summary>Watch2o and BioBattery</summary>
        <p><em>Last updated: March 2026</em></p>
        <p>This privacy policy applies to both Watch2o and BioBattery. These applications are designed for Apple Watch and built with a strong focus on user privacy. Neither app collects, stores, or shares personal information of any kind.</p>
        <h3>Information We Collect</h3>
        <p>Watch2o and BioBattery do not collect, store, or transmit any personal data. The apps do not use analytics, tracking tools, advertising services, or user identifiers.</p>
        <h3>Health Data (Watch2o only)</h3>
        <ul>
          <li>If you choose to enable HealthKit for Watch2o to store water intake data: data is stored only on your device.</li>
          <li>Data is never sent to external servers.</li>
          <li>Watch2o does not access any other HealthKit data types.</li>
        </ul>
        <p>BioBattery does not use HealthKit.</p>
        <h3>Third Party Sharing</h3>
        <p>Neither Watch2o nor BioBattery share any information with third parties. No data is transmitted to servers, services, or external partners.</p>
        <h3>Children's Privacy</h3>
        <p>These apps do not target or collect data from children. No personally identifiable information is used or processed.</p>
        <h3>Changes to This Policy</h3>
        <p>Any updates to this policy will be published on this page. Continued use of the apps after changes indicates acceptance of the updated policy.</p>
        <h3 id="contact">Contact</h3>
        <p>For questions or support: <a href="https://github.com/bawarym/bawary</a></p>
      </details>
    </div>
  </section>

  <footer class="footer">
    <div class="wrap">
      <p>© 2026 Atiqullah Bawary · Nanohabit</p>
      <p class="mono">Bundle IDs: com.atiq.SocialBattery (BioBattery), com.your.bundle.watch2o</p>
    </div>
  </footer>

  <script>
    // Smooth scroll for same-page anchors
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click',e=>{
        const id=a.getAttribute('href');
        if(id.length>1){
          e.preventDefault();
          document.querySelector(id)?.scrollIntoView({behavior:'smooth',block:'start'});
          history.pushState(null,'',id);
        }
      });
    });
  </script>
</body>
</html>
