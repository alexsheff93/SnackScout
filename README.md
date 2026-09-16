# SnackScout

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SnackScout | Discover Your Next Favourite Treat</title>
  <meta name="description" content="Discover interesting snacks, chocolates, sweets and drinks with SnackScout.">
  <style>
    :root {
      --orange: #f59e0b;
      --dark: #171717;
      --cream: #fffaf0;
      --muted: #6b7280;
      --border: #eadfce;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: var(--dark);
      background: var(--cream);
    }

    a { color: inherit; text-decoration: none; }

    header {
      background: white;
      border-bottom: 1px solid var(--border);
      padding: 18px 24px;
    }

    .nav {
      max-width: 1100px;
      margin: auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo {
      font-size: 25px;
      font-weight: 800;
    }

    .logo span { color: var(--orange); }

    nav {
      display: flex;
      flex-wrap: wrap;
      gap: 18px;
      font-size: 14px;
    }

    .hero {
      max-width: 1100px;
      margin: auto;
      padding: 70px 24px 50px;
      text-align: center;
    }

    .hero h1 {
      font-size: clamp(36px, 6vw, 64px);
      margin: 0 0 18px;
      letter-spacing: -2px;
    }

    .hero p {
      max-width: 600px;
      margin: 0 auto 28px;
      color: var(--muted);
      font-size: 18px;
      line-height: 1.6;
    }

    .button {
      display: inline-block;
      background: var(--orange);
      color: #171717;
      font-weight: 700;
      padding: 14px 22px;
      border-radius: 999px;
    }

    .section {
      max-width: 1100px;
      margin: auto;
      padding: 30px 24px 60px;
    }

    .section h2 {
      font-size: 30px;
      margin-bottom: 24px;
    }

    .categories, .products {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }

    .category, .product {
      background: white;
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 24px;
    }

    .category {
      font-size: 20px;
      font-weight: 700;
    }

    .category small {
      display: block;
      color: var(--muted);
      font-size: 14px;
      font-weight: 400;
      margin-top: 8px;
    }

    .product .emoji {
      font-size: 50px;
      margin-bottom: 14px;
    }

    .product h3 { margin: 0 0 8px; }

    .product p {
      color: var(--muted);
      line-height: 1.5;
      font-size: 14px;
    }

    .product .button {
      font-size: 13px;
      padding: 10px 15px;
      margin-top: 8px;
    }

    .newsletter {
      background: #171717;
      color: white;
      border-radius: 24px;
      padding: 36px 24px;
      text-align: center;
    }

    .newsletter p {
      color: #d4d4d4;
      line-height: 1.5;
    }

    footer {
      background: white;
      border-top: 1px solid var(--border);
      padding: 30px 24px;
      color: var(--muted);
      font-size: 13px;
      text-align: center;
    }

    @media (max-width: 650px) {
      .nav { flex-direction: column; }
      .hero { padding-top: 45px; }
      .categories, .products { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

<header>
  <div class="nav">
    <a class="logo" href="#">Snack<span>Scout</span> 🍫</a>
    <nav>
      <a href="#finds">Latest Finds</a>
      <a href="#categories">Categories</a>
      <a href="#newsletter">Newsletter</a>
    </nav>
  </div>
</header>

<main>
  <section class="hero">
    <h1>Find your next<br>favourite treat.</h1>
    <p>
      Discover interesting chocolates, sweets, drinks and
      snack finds from around the world.
    </p>
    <a class="button" href="#finds">Explore Snack Finds →</a>
  </section>

  <section class="section" id="categories">
    <h2>What are you craving?</h2>
    <div class="categories">
      <a class="category" href="#finds">
        🍫 Chocolates
        <small>Chocolate bars, boxes & treats</small>
      </a>
      <a class="category" href="#finds">
        🍬 Sweets
        <small>Gummies, candy & discoveries</small>
      </a>
      <a class="category" href="#finds">
        🥤 Drinks
        <small>Soft drinks & beverages</small>
      </a>
    </div>
  </section>

  <section class="section" id="finds">
    <h2>Latest Snack Finds</h2>
    <div class="products">

      <!-- Replace these examples with real products -->
      <article class="product">
        <div class="emoji">🍫</div>
        <h3>Chocolate Finds</h3>
        <p>
          Discover interesting chocolate products and
          treat bundles.
        </p>
        <a class="button" href="#" aria-label="View chocolate deals">
          View Deals →
        </a>
      </article>

      <article class="product">
        <div class="emoji">🍬</div>
        <h3>Sweet Treats</h3>
        <p>
          Explore unusual sweets and candy discoveries.
        </p>
        <a class="button" href="#" aria-label="View sweet deals">
          View Deals →
        </a>
      </article>

      <article class="product">
        <div class="emoji">🥤</div>
        <h3>Drink Discoveries</h3>
        <p>
          Find interesting drinks and refreshing
          beverage options.
        </p>
        <a class="button" href="#" aria-label="View drink deals">
          View Deals →
        </a>
      </article>

    </div>
  </section>

  <section class="section" id="newsletter">
    <div class="newsletter">
      <h2>Get the latest SnackScout finds</h2>
      <p>
        Discover new snacks, treats and interesting deals.
        Join our newsletter when it launches.
      </p>
      <a class="button" href="mailto:YOUR-BRAND-EMAIL@example.com">
        Contact SnackScout →
      </a>
    </div>
  </section>
</main>

<footer>
  <p>© 2026 SnackScout. All rights reserved.</p>
  <p>
    Some links may be affiliate links. We may earn a commission
    from qualifying purchases.
  </p>
  <p>Product availability and prices may change.</p>
</footer>

</body>
</html>
