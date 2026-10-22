# RB-Properties
RB Properties Website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
  <title>RB Properties | Homes, Apartments, Land &amp; Commercial Spaces</title>
  <meta name="description" content="RB Properties is a trusted real estate company. Browse homes, apartments, land and commercial properties for sale and rent, or send us an enquiry.">
  <meta name="theme-color" content="#0b6e7f">
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Crect width='100' height='100' rx='20' fill='%230b6e7f'/%3E%3Ctext x='50' y='66' font-size='46' font-family='Georgia' font-weight='700' text-anchor='middle' fill='white'%3ERB%3C/text%3E%3C/svg%3E">
  <link rel="stylesheet" href="css/style.css">
</head>
<body>

  <!-- ===== HEADER / NAVIGATION ===== -->
  <header>
    <div class="wrap nav">
      <a class="logo" href="#home" aria-label="RB Properties home">
        <i>RB</i><span>RB <small>Properties</small></span>
      </a>
      <nav id="nav" aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#listings">Properties</a>
        <a href="#blog">Blog</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>

    <!-- ===== HOME PAGE ===== -->
    <div class="page" id="home">
      <div class="hero">
        <div class="wrap">
          <div class="eyebrow">Trusted real estate advisors</div>
          <h1>Find a home that fits your life, and your future.</h1>
          <p>Premium homes, apartments, land and commercial spaces, handled with honesty, expertise and care from first viewing to final keys.</p>
          <p>
            <a class="btn" href="#listings">Browse properties</a>
            <a class="btn o" href="#contact">Talk to an agent</a>
          </p>
        </div>
      </div>

      <div class="wrap stats">
        <div class="stat"><b>350+</b><span>Properties sold</span></div>
        <div class="stat"><b>12 yrs</b><span>Market experience</span></div>
        <div class="stat"><b>98%</b><span>Client satisfaction</span></div>
        <div class="stat"><b>24/7</b><span>Support via chat</span></div>
      </div>

      <section>
        <div class="wrap">
          <div class="head">
            <div><div class="eyebrow">Featured</div><h2>Handpicked properties</h2></div>
            <a class="btn o" href="#listings">View all</a>
          </div>
          <div class="grid" id="feat"><!-- filled by script.js --></div>
        </div>
      </section>

      <section class="alt">
        <div class="wrap">
          <div class="eyebrow">Why RB Properties</div>
          <h2>Everything under one roof</h2>
          <div class="three">
            <div class="box"><div class="ic">🏠</div><h3>Buy &amp; Sell</h3><p>Accurate valuations, professional marketing and vetted buyers.</p></div>
            <div class="box"><div class="ic">🔑</div><h3>Rentals &amp; Management</h3><p>Tenant screening, rent collection and maintenance handled for you.</p></div>
            <div class="box"><div class="ic">📑</div><h3>Legal &amp; Documentation</h3><p>Title checks and transparent paperwork for a secure transaction.</p></div>
          </div>
        </div>
      </section>

      <section>
        <div class="wrap">
          <div class="cta">
            <h2>Ready to make your move?</h2>
            <p>Tell us what you are looking for and an agent will reach out within 24 hours.</p>
            <a class="btn" href="#contact">Send an enquiry</a>
          </div>
        </div>
      </section>
    </div>

    <!-- ===== PROPERTY LISTINGS PAGE ===== -->
    <div class="page" id="listings">
      <section>
        <div class="wrap">
          <div class="eyebrow">Property listings</div>
          <h2>Find your next property</h2>

          <div class="filters">
            <select id="ft" aria-label="Property type">
              <option value="">All types</option>
              <option>House</option><option>Apartment</option><option>Land</option><option>Commercial</option>
            </select>
            <select id="fs" aria-label="Sale or rent">
              <option value="">For sale &amp; rent</option>
              <option>Sale</option><option>Rent</option>
            </select>
            <select id="fl" aria-label="Location"><option value="">All locations</option></select>
          </div>

          <div class="grid" id="all"><!-- filled by script.js --></div>
          <p id="none" style="display:none;color:var(--mut)">No properties match those filters.</p>
        </div>
      </section>
    </div>

    <!-- ===== BLOG PAGE ===== -->
    <div class="page" id="blog">
      <section>
        <div class="wrap">
          <div class="eyebrow">Insights</div>
          <h2>The RB Properties Blog</h2>
          <div class="grid" id="posts"><!-- filled by script.js --></div>
        </div>
      </section>
    </div>

    <!-- ===== CONTACT PAGE ===== -->
    <div class="page" id="contact">
      <section>
        <div class="wrap">
          <div class="eyebrow">Get in touch</div>
          <h2>Make an enquiry</h2>

          <div class="cgrid">
            <div class="box">
              <form id="ef">
                <div class="row">
                  <div><label for="n">Full name</label><input id="n" required></div>
                  <div><label for="p">Phone</label><input id="p" type="tel" required></div>
                </div>

                <label for="e">Email</label>
                <input id="e" type="email" required>

                <div class="row">
                  <div>
                    <label for="k">I am interested in</label>
                    <select id="k">
                      <option>Buying</option><option>Renting</option><option>Selling my property</option>
                      <option>Property management</option><option>Other</option>
                    </select>
                  </div>
                  <div>
                    <label for="pp">Property (optional)</label>
                    <select id="pp"><option value="">Not sure yet</option></select>
                  </div>
                </div>

                <label for="m">Message</label>
                <textarea id="m" rows="5" required placeholder="Budget, preferred location, bedrooms, viewing dates…"></textarea>

                <p><button class="btn" type="submit">Send enquiry</button></p>
                <div id="ok" role="status"></div>
              </form>
            </div>

            <div>
              <div class="box">
                <h3>Visit or call us</h3>
                <p>📍 Lagos, Nigeria<br>📞 +234 800 000 0000<br>✉️ hello@rbproperties.com</p>
                <p><b>Office hours</b><br>Mon–Fri 9:00–18:00<br>Sat 10:00–15:00</p>
                <p>Prefer a quick answer? Use the chat button at the bottom right.</p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>

  </main>

  <!-- ===== FOOTER ===== -->
  <footer>
    <div class="wrap">
      <div><b style="color:#fff;font-size:18px">RB Properties</b><br>Honest advice. Quality homes.</div>
      <div>© 2026 RB Properties. All rights reserved.</div>
    </div>
  </footer>

  <!-- ===== LIVE CHAT WIDGET ===== -->
  <button id="cb" aria-label="Open chat">💬</button>
  <div id="cw" role="dialog" aria-label="Live chat">
    <div class="t">RB Properties Chat<small>● Online, typically replies in minutes</small></div>
    <div id="ms" aria-live="polite"></div>
    <div class="qr" id="qr"></div>
    <form id="cf">
      <input id="ci" placeholder="Type a message…" autocomplete="off" aria-label="Chat message">
      <button class="btn">Send</button>
    </form>
  </div>

  <script src="js/script.js"></script>
</body>
</html>
