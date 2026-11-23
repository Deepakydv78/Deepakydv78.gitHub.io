<! Premium Clothings>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ATELIER VERA — Contemporary Clothing &amp; Everyday Essentials</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://unpkg.com/lucide@0.460.0/dist/umd/lucide.min.js"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'system-ui', '-apple-system', 'sans-serif'],
          },
          colors: {
            alabaster: '#FAF8F5',
            stonewarm: '#F2EFE9',
            ink: '#1A1917',
            taupe: '#6E6962',
            sand: '#A67C52',
          }
        }
      }
    };
  </script>
  <style>
    body {
      font-family: 'Inter', system-ui, -apple-system, sans-serif;
      background-color: #FAF8F5;
      color: #1A1917;
    }
    .product-card:hover .product-img {
      transform: scale(1.03);
    }
    .product-img {
      transition: transform 0.45s cubic-bezier(0.22, 1, 0.36, 1);
    }
    .drawer-transition {
      transition: transform 0.3s cubic-bezier(0.22, 1, 0.36, 1);
    }
  </style>
</head>
<body class="antialiased selection:bg-sand/20 selection:text-ink">

  <!-- Announcement Bar -->
  <div class="bg-ink text-alabaster text-xs tracking-wide py-2 px-4 text-center">
    Complimentary shipping on orders over $200 &middot; Use code <span class="font-semibold underline underline-offset-2">VERA10</span> for 10% off your first order
  </div>

  <!-- Sticky Navigation -->
  <header class="sticky top-0 z-40 bg-alabaster/90 backdrop-blur-md border-b border-stone-200/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <button id="mobile-menu-btn" type="button" class="md:hidden p-2 -ml-2 text-ink hover:text-sand transition-colors" aria-label="Toggle Menu">
          <i data-lucide="menu" class="w-5 h-5"></i>
        </button>

        <a href="#top" class="text-lg sm:text-xl font-semibold tracking-[0.18em] uppercase text-ink">
          Atelier Vera
        </a>

        <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-taupe">
          <a href="#collection" class="hover:text-ink transition-colors">Collection</a>
          <a href="#lookbook" class="hover:text-ink transition-colors">Lookbook</a>
          <a href="#craft" class="hover:text-ink transition-colors">Materials</a>
          <a href="#contact" class="hover:text-ink transition-colors">Newsletter</a>
        </nav>

        <div class="flex items-center space-x-2 sm:space-x-4">
          <button id="wishlist-filter-btn" type="button" class="relative p-2 text-ink hover:text-sand transition-colors" aria-label="Filter Saved Items" title="View Saved Items">
            <i data-lucide="heart" class="w-5 h-5"></i>
            <span id="wishlist-badge" class="hidden absolute top-1 right-0.5 bg-sand text-white text-[10px] font-semibold w-4 h-4 rounded-full flex items-center justify-center">0</span>
          </button>

          <button id="open-cart-btn" type="button" class="relative flex items-center space-x-2 bg-ink text-alabaster px-3.5 py-2 rounded-full text-xs sm:text-sm font-medium hover:bg-stone-800 transition-colors">
            <i data-lucide="shopping-bag" class="w-4 h-4"></i>
            <span class="hidden sm:inline">Bag</span>
            <span id="cart-badge" class="bg-sand text-white text-[11px] font-semibold px-1.5 py-0.5 rounded-full min-w-[20px] text-center">0</span>
          </button>
        </div>
      </div>

      <div id="mobile-nav" class="hidden md:hidden pb-4 pt-2 border-t border-stone-200 space-y-2 text-sm font-medium text-taupe">
        <a href="#collection" class="block py-1.5 hover:text-ink mobile-nav-link">Collection</a>
        <a href="#lookbook" class="block py-1.5 hover:text-ink mobile-nav-link">Lookbook</a>
        <a href="#craft" class="block py-1.5 hover:text-ink mobile-nav-link">Materials</a>
        <a href="#contact" class="block py-1.5 hover:text-ink mobile-nav-link">Newsletter</a>
      </div>
    </div>
  </header>

  <main id="top">
    <!-- Hero Section -->
    <section class="relative overflow-hidden bg-stonewarm">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10 lg:py-16">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 lg:gap-12 items-center">
          <div class="lg:col-span-5 space-y-6">
            <span class="inline-block text-xs font-semibold uppercase tracking-[0.2em] text-sand">
              Autumn / Winter Edit
            </span>
            <h1 class="text-3xl sm:text-4xl lg:text-5xl font-semibold tracking-tight text-ink leading-[1.12]">
              Tailored silhouettes built from natural fibers.
            </h1>
            <p class="text-taupe text-base sm:text-lg leading-relaxed">
              Small-batch organic cotton, Belgian linen, and Japanese selvedge denim designed for effortless daily layering.
            </p>
            <div class="flex flex-wrap items-center gap-3 pt-2">
              <a href="#collection" class="inline-flex items-center justify-center px-6 py-3 rounded-full bg-ink text-alabaster text-sm font-medium hover:bg-stone-800 transition-colors">
                Shop Collection
              </a>
              <a href="#lookbook" class="inline-flex items-center justify-center px-6 py-3 rounded-full border border-stone-300 text-ink text-sm font-medium hover:border-ink transition-colors">
                Explore Lookbook
              </a>
            </div>
          </div>

          <div class="lg:col-span-7">
            <div class="relative rounded-2xl overflow-hidden shadow-sm border border-stone-200/70 aspect-[16/9] bg-stone-200">
              <img
                src="images/hero.jpg"
                alt="Curated neutral linen and cotton garments on a minimalist studio rack"
                class="w-full h-full object-cover"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Collection Section -->
    <section id="collection" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-14 sm:py-20">
      <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-10">
        <div>
          <p class="text-xs font-semibold uppercase tracking-[0.2em] text-sand mb-2">Ready-to-Wear</p>
          <h2 class="text-2xl sm:text-3xl font-semibold tracking-tight text-ink">The Core Collection</h2>
        </div>

        <div class="flex flex-col sm:flex-row items-stretch sm:items-center gap-3">
          <div class="relative">
            <i data-lucide="search" class="w-4 h-4 text-taupe absolute left-3.5 top-1/2 -translate-y-1/2 pointer-events-none"></i>
            <input
              id="search-input"
              type="text"
              placeholder="Search garments..."
              class="w-full sm:w-56 pl-10 pr-4 py-2 rounded-full border border-stone-300 bg-white text-sm text-ink placeholder:text-taupe/70 focus:outline-none focus:border-ink transition-colors"
            />
          </div>

          <select
            id="sort-select"
            aria-label="Sort products"
            class="px-4 py-2 rounded-full border border-stone-300 bg-white text-sm text-ink focus:outline-none focus:border-ink transition-colors"
          >
            <option value="featured">Sort: Featured</option>
            <option value="price-asc">Price: Low to High</option>
            <option value="price-desc">Price: High to Low</option>
          </select>
        </div>
      </div>

      <div class="flex flex-wrap items-center justify-between gap-4 mb-8">
        <div id="category-filters" class="flex flex-wrap items-center gap-2">
          <button type="button" data-category="All" class="cat-pill px-4 py-2 rounded-full text-xs sm:text-sm font-medium bg-ink text-alabaster transition-colors">
            All Pieces
          </button>
          <button type="button" data-category="Outerwear" class="cat-pill px-4 py-2 rounded-full text-xs sm:text-sm font-medium bg-stonewarm text-taupe hover:text-ink transition-colors">
            Outerwear
          </button>
          <button type="button" data-category="Tops & Knits" class="cat-pill px-4 py-2 rounded-full text-xs sm:text-sm font-medium bg-stonewarm text-taupe hover:text-ink transition-colors">
            Tops &amp; Knits
          </button>
          <button type="button" data-category="Bottoms" class="cat-pill px-4 py-2 rounded-full text-xs sm:text-sm font-medium bg-stonewarm text-taupe hover:text-ink transition-colors">
            Bottoms
          </button>
        </div>

        <p id="results-count" class="text-xs sm:text-sm text-taupe">Showing 6 pieces</p>
      </div>

      <div id="product-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-7"></div>

      <div id="empty-state" class="hidden text-center py-16 px-4 bg-white rounded-2xl border border-stone-200/80">
        <p class="text-base font-medium text-ink mb-2">No matching garments found</p>
        <p class="text-sm text-taupe mb-5">Try clearing your search or switching back to all pieces.</p>
        <button id="reset-filters-btn" type="button" class="px-5 py-2.5 rounded-full bg-ink text-alabaster text-sm font-medium hover:bg-stone-800 transition-colors">
          Reset Filters
        </button>
      </div>
    </section>

    <!-- Editorial Lookbook Band -->
    <section id="lookbook" class="bg-stonewarm border-y border-stone-200/80 py-14 sm:py-20">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="max-w-2xl mb-10">
          <p class="text-xs font-semibold uppercase tracking-[0.2em] text-sand mb-2">Lookbook 04</p>
          <h2 class="text-2xl sm:text-3xl font-semibold tracking-tight text-ink mb-3">Built to layer across seasons</h2>
          <p class="text-taupe text-sm sm:text-base leading-relaxed">
            Every piece in the Atelier Vera wardrobe shares a cohesive neutral palette so jackets, knits, and trousers pair effortlessly without overthinking.
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div class="bg-white rounded-2xl p-6 border border-stone-200/70 space-y-3">
            <span class="text-xs font-semibold uppercase tracking-wider text-sand">01 &middot; Studio Tailoring</span>
            <h3 class="text-lg font-semibold text-ink">Sand Linen + Charcoal Wool</h3>
            <p class="text-sm text-taupe leading-relaxed">
              Pair the relaxed sand linen blazer with pleated merino trousers for breathable structure from morning studio hours to evening dinners.
            </p>
          </div>
          <div class="bg-white rounded-2xl p-6 border border-stone-200/70 space-y-3">
            <span class="text-xs font-semibold uppercase tracking-wider text-sand">02 &middot; Weekend Uniform</span>
            <h3 class="text-lg font-semibold text-ink">Selvedge Indigo + Oatmeal Tee</h3>
            <p class="text-sm text-taupe leading-relaxed">
              13.5oz raw selvedge denim layered over our 280gsm organic cotton crewneck creates a durable, lived-in silhouette that ages with character.
            </p>
          </div>
          <div class="bg-white rounded-2xl p-6 border border-stone-200/70 space-y-3">
            <span class="text-xs font-semibold uppercase tracking-wider text-sand">03 &middot; Transitional Warmth</span>
            <h3 class="text-lg font-semibold text-ink">Moss Merino + Matte Overshirt</h3>
            <p class="text-sm text-taupe leading-relaxed">
              Chunky fisherman-ribbed wool beneath a structured cotton twill overshirt delivers wind resistance without synthetic bulk.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Materials & Craft -->
    <section id="craft" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-14 sm:py-20">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="flex items-start space-x-4">
          <div class="w-10 h-10 rounded-full bg-stonewarm flex items-center justify-center shrink-0 text-sand">
            <i data-lucide="leaf" class="w-5 h-5"></i>
          </div>
          <div>
            <h3 class="font-semibold text-ink text-base mb-1">100% Natural Fibers</h3>
            <p class="text-sm text-taupe leading-relaxed">GOTS-certified organic cotton, traceable merino wool, and European flax linen with zero virgin polyester.</p>
          </div>
        </div>
        <div class="flex items-start space-x-4">
          <div class="w-10 h-10 rounded-full bg-stonewarm flex items-center justify-center shrink-0 text-sand">
            <i data-lucide="ruler" class="w-5 h-5"></i>
          </div>
          <div>
            <h3 class="font-semibold text-ink text-base mb-1">Precision Fit &amp; Repairs</h3>
            <p class="text-sm text-taupe leading-relaxed">Pre-shrunk garment washing and complimentary lifetime seam and button repairs at our partner ateliers.</p>
          </div>
        </div>
        <div class="flex items-start space-x-4">
          <div class="w-10 h-10 rounded-full bg-stonewarm flex items-center justify-center shrink-0 text-sand">
            <i data-lucide="package-check" class="w-5 h-5"></i>
          </div>
          <div>
            <h3 class="font-semibold text-ink text-base mb-1">30-Day Home Try-On</h3>
            <p class="text-sm text-taupe leading-relaxed">Carbon-neutral shipping and hassle-free size exchanges within 30 days of delivery.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Newsletter -->
    <section id="contact" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pb-16">
      <div class="bg-ink text-alabaster rounded-3xl p-8 sm:p-12 flex flex-col lg:flex-row items-start lg:items-center justify-between gap-8">
        <div class="max-w-lg space-y-2">
          <p class="text-xs font-semibold uppercase tracking-[0.2em] text-sand">Private Dispatch</p>
          <h2 class="text-2xl sm:text-3xl font-semibold tracking-tight">Early access to seasonal drops.</h2>
          <p class="text-stone-300 text-sm sm:text-base">
            Join our dispatch for restock alerts, fabric notes, and 10% off your first order.
          </p>
        </div>

        <form id="newsletter-form" class="w-full lg:w-auto flex flex-col sm:flex-row gap-3">
          <input
            id="newsletter-email"
            type="email"
            required
            placeholder="you@example.com"
            class="w-full sm:w-72 px-5 py-3 rounded-full bg-white/10 border border-white/20 text-alabaster placeholder:text-stone-400 text-sm focus:outline-none focus:border-sand"
          />
          <button type="submit" class="px-6 py-3 rounded-full bg-sand text-white text-sm font-medium hover:bg-sand/90 transition-colors shrink-0">
            Subscribe
          </button>
        </form>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="border-t border-stone-200 bg-alabaster py-10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs text-taupe">
      <div class="flex items-center space-x-3">
        <span class="font-semibold tracking-[0.16em] uppercase text-ink">Atelier Vera</span>
        <span>&copy; 2026 Atelier Vera. All rights reserved.</span>
      </div>
      <div class="flex items-center space-x-6">
        <a href="#collection" class="hover:text-ink transition-colors">Shop</a>
        <a href="#lookbook" class="hover:text-ink transition-colors">Lookbook</a>
        <a href="#craft" class="hover:text-ink transition-colors">Materials</a>
        <a href="#contact" class="hover:text-ink transition-colors">Contact</a>
      </div>
    </div>
  </footer>

  <!-- Quick View Modal -->
  <div id="quick-view-modal" class="hidden fixed inset-0 z-50 flex items-center justify-center p-4 bg-ink/50 backdrop-blur-sm">
    <div class="bg-white rounded-2xl max-w-2xl w-full overflow-hidden shadow-xl border border-stone-200 grid grid-cols-1 md:grid-cols-2">
      <div class="bg-stonewarm aspect-[4/3] md:aspect-auto">
        <img id="qv-img" src="" alt="" class="w-full h-full object-cover" />
      </div>
      <div class="p-6 sm:p-7 flex flex-col justify-between space-y-5">
        <div>
          <div class="flex items-start justify-between gap-4">
            <div>
              <p id="qv-category" class="text-xs font-semibold uppercase tracking-wider text-sand mb-1"></p>
              <h3 id="qv-title" class="text-xl font-semibold text-ink"></h3>
            </div>
            <button id="close-qv-btn" type="button" class="p-1.5 text-taupe hover:text-ink rounded-full" aria-label="Close modal">
              <i data-lucide="x" class="w-5 h-5"></i>
            </button>
          </div>
          <p id="qv-price" class="text-lg font-semibold text-ink mt-2"></p>
          <p id="qv-desc" class="text-sm text-taupe leading-relaxed mt-3"></p>
          <p id="qv-fabric" class="text-xs text-taupe mt-3 pt-3 border-t border-stone-100"></p>
        </div>

        <div class="space-y-4">
          <div>
            <span class="block text-xs font-medium text-ink mb-2">Select Size</span>
            <div id="qv-sizes" class="flex items-center gap-2"></div>
          </div>
          <button id="qv-add-btn" type="button" class="w-full py-3 rounded-full bg-ink text-alabaster text-sm font-medium hover:bg-stone-800 transition-colors">
            Add to Bag
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- Slide-Over Shopping Bag Drawer -->
  <div id="cart-overlay" class="hidden fixed inset-0 z-50 bg-ink/40 backdrop-blur-[2px]">
    <aside id="cart-drawer" class="fixed right-0 top-0 h-full w-full max-w-md bg-alabaster shadow-2xl flex flex-col drawer-transition translate-x-full">
      <div class="flex items-center justify-between px-6 py-5 border-b border-stone-200 bg-white">
        <div class="flex items-center space-x-2">
          <h3 class="text-base font-semibold text-ink">Shopping Bag</h3>
          <span id="drawer-count" class="text-xs text-taupe">(0 items)</span>
        </div>
        <button id="close-cart-btn" type="button" class="p-1.5 text-taupe hover:text-ink rounded-full" aria-label="Close bag">
          <i data-lucide="x" class="w-5 h-5"></i>
        </button>
      </div>

      <div class="px-6 py-3 bg-stonewarm border-b border-stone-200/80">
        <p id="shipping-msg" class="text-xs text-ink font-medium mb-1.5"></p>
        <div class="w-full h-1.5 bg-stone-300 rounded-full overflow-hidden">
          <div id="shipping-bar" class="h-full bg-sand transition-all duration-300" style="width: 0%"></div>
        </div>
      </div>

      <div id="cart-items" class="flex-1 overflow-y-auto px-6 py-4 space-y-4"></div>

      <div id="cart-footer" class="border-t border-stone-200 bg-white px-6 py-5 space-y-4">
        <div class="flex gap-2">
          <input
            id="promo-input"
            type="text"
            placeholder="Promo code (try VERA10)"
            class="flex-1 px-3.5 py-2 rounded-full border border-stone-300 text-xs text-ink focus:outline-none focus:border-ink"
          />
          <button id="apply-promo-btn" type="button" class="px-4 py-2 rounded-full bg-stonewarm text-ink text-xs font-medium hover:bg-stone-200 transition-colors">
            Apply
          </button>
        </div>

        <div class="space-y-1.5 text-sm">
          <div class="flex justify-between text-taupe">
            <span>Subtotal</span>
            <span id="cart-subtotal">$0.00</span>
          </div>
          <div id="dis
