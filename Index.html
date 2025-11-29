<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>SexZone</title>
    <meta name="description" content="Plataforma de entretenimiento para adultos. Contenido solo para mayores de 18 años." />
    <style>
        /* Reset */
        * { box-sizing:border-box; margin:0; padding:0; }
        html,body { height:100%; background:#000; color:#fff; font-family:Arial, sans-serif; -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale; }
        a { color:inherit; text-decoration:none; }

        /* Container */
        .container { max-width:1200px; margin:0 auto; padding:8px 16px; }

        /* Header layout: three columns (left toggle, center brand, right actions) */
        header { position:sticky; top:0; z-index:1100; background:#0b0b0b; border-bottom:1px solid rgba(255,255,255,0.02); }
        .header-inner { display:grid; grid-template-columns:48px 1fr 48px; align-items:center; gap:12px; padding:10px 12px; max-width:1200px; margin:0 auto; }
        .left, .center, .right { display:flex; align-items:center; }
        .left { justify-content:flex-start; }
        .center { justify-content:center; }
        .right { justify-content:flex-end; }

        /* Menu toggle */
        .menu-toggle { width:40px; height:40px; display:flex; align-items:center; justify-content:center; background:transparent; border:0; cursor:pointer; border-radius:8px; }
        .menu-toggle .bar { width:22px; height:2px; background:#ffd; display:block; position:relative; }
        .menu-toggle .bar::before, .menu-toggle .bar::after { content:''; position:absolute; left:0; right:0; height:2px; background:#ffd; }
        .menu-toggle .bar::before { top:-6px; }
        .menu-toggle .bar::after { top:6px; }

        /* Brand (SexZone) */
        .brand { font-weight:800; font-size:1.25rem; letter-spacing:0.2px; color:#fff; }
        @media (max-width:880px) { .brand { font-size:1.4rem; } }

        /* Search (kept long) - now with magnifier circle inside */
        .search-bar { width:100%; display:flex; align-items:center; justify-content:center; position:relative; }
        .search-bar .search-icon {
            position:absolute; left:10px; width:36px; height:36px; border-radius:50%;
            display:flex; align-items:center; justify-content:center; background:rgba(255,255,255,0.03); border:1px solid rgba(255,255,255,0.02);
            pointer-events:auto; cursor:pointer;
        }
        .search-bar input {
            width:100%; max-width:820px; padding:10px 14px 10px 54px; border-radius:28px; background:#060606; color:#ddd;
            border:1px solid rgba(255,255,255,0.03); outline:none; font-size:0.95rem;
        }
        .search-bar input::placeholder { color:#666; }

        /* Floating search hint that appears when clicking magnifier */
        .floating-search {
            position:fixed; top:64px; left:50%; transform:translateX(-50%); z-index:2500;
            background:linear-gradient(180deg,#0f0f0f,#0b0b0b); border:1px solid rgba(255,255,255,0.04);
            padding:8px 12px; border-radius:999px; display:flex; gap:8px; align-items:center; box-shadow:0 10px 30px rgba(0,0,0,0.6);
            min-width:220px; max-width:92%; color:#ddd;
        }
        .floating-search .fs-text { font-weight:700; padding-right:8px; color:#fff; }
        .floating-search input { background:transparent; border:0; color:#ddd; outline:none; width:220px; }

        /* Profile circle (right top) */
        .profile-btn {
            width:40px; height:40px; border-radius:50%; background:linear-gradient(180deg,#222,#111);
            display:inline-flex; align-items:center; justify-content:center; cursor:pointer; border:1px solid rgba(255,255,255,0.04);
            position:relative;
        }
        .profile-dot { width:18px; height:18px; border-radius:50%; background:#1e1e1e; display:inline-block; }
        .profile-btn:focus { outline:3px solid rgba(255,71,87,0.15); }

        /* Profile dropdown */
        .profile-menu {
            position:absolute; right:0; top:48px; background:#0f0f0f; border:1px solid rgba(255,255,255,0.03);
            border-radius:10px; padding:8px; min-width:220px; display:none; box-shadow:0 10px 30px rgba(0,0,0,0.6);
        }
        .profile-menu.show { display:block; }
        .profile-menu .profile-email { display:block; padding:8px 12px; color:#ffb3c6; font-weight:800; }
        .profile-menu button, .profile-menu a {
            display:block; width:100%; text-align:left; padding:10px 12px; border-radius:8px; background:transparent; color:#ddd; border:0; cursor:pointer;
        }
        .profile-menu button:hover, .profile-menu a:hover { background:rgba(255,255,255,0.02); color:#fff; }

        /* Nav menu items (desktop) - spaced, enclosed, big */
        nav#primary-nav { display:flex; gap:14px; align-items:center; justify-content:center; padding:12px 0; flex-wrap:wrap; }
        nav#primary-nav .nav-item {
            display:inline-flex; align-items:center; justify-content:center;
            padding:12px 18px; border-radius:12px; background:rgba(255,255,255,0.02); border:1px solid rgba(255,255,255,0.03);
            min-width:130px; text-align:center; font-weight:700; letter-spacing:0.2px; color:#fff;
            box-shadow: inset 0 -10px 30px rgba(0,0,0,0.2);
        }
        nav#primary-nav .nav-item + .nav-item { margin-left:10px; }
        nav#primary-nav .nav-item:active { transform:translateY(1px); }
        @media (max-width:880px) { nav#primary-nav { display:none; } }

        /* Side menu for mobile (off-canvas) */
        .side-overlay { position:fixed; inset:0; background:rgba(0,0,0,0.5); display:none; z-index:2000; }
        .side-menu {
            position:fixed; left:0; top:0; bottom:0; width:320px; max-width:85%;
            background:#0b0b0b; transform:translateX(-110%); transition:transform .28s cubic-bezier(.2,.9,.2,1);
            z-index:2001; padding:18px; overflow:auto;
        }
        .side-menu.open { transform:translateX(0); }
        .side-menu .side-item {
            display:block; margin-bottom:12px; padding:14px; border-radius:12px; background:#0f0f0f; border:1px solid rgba(255,255,255,0.03);
            font-weight:700; color:#fff;
        }

        /* Main adjustments */
        main { padding:6px 0 20px 0; }
        section { margin:0; padding:8px 0; }
        .grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(220px,1fr)); gap:10px; }

        .video-item {
            background:#0e0e0e; border-radius:10px; overflow:hidden; position:relative; cursor:pointer;
            border:1px solid rgba(255,255,255,0.02);
            transition:transform .12s cubic-bezier(.2,.9,.2,1), box-shadow .12s;
        }
        .video-item:hover { transform:translateY(-6px); box-shadow:0 12px 30px rgba(0,0,0,0.6); }

        .video-thumbnail { width:100%; height:160px; object-fit:cover; background:#000; display:block; }
        .video-info { padding:10px; }
        .video-info h3 { font-size:1rem; margin-bottom:6px; }
        .video-info p { color:#bbb; font-size:0.88rem; }

        .category-pills { display:flex; gap:10px; overflow:auto; padding:8px 6px 14px 6px; }
        .pill { flex:0 0 auto; padding:10px 16px; background:rgba(255,255,255,0.02); border-radius:999px; border:1px solid rgba(255,255,255,0.03); font-weight:700; cursor:pointer; color:#fff; }

        /* No-results message */
        .no-results {
            color:#bbb; background:#0d0d0d; border:1px solid rgba(255,255,255,0.02);
            padding:12px; border-radius:8px; margin-top:10px; text-align:center;
        }

        /* Video overlay (keeps page behind intact) - includes controls, channel and comments below */
        .video-overlay { position:fixed; inset:0; display:none; align-items:flex-start; justify-content:center; background:linear-gradient(180deg, rgba(0,0,0,0.85), rgba(0,0,0,0.95)); z-index:3000; padding-top:44px; }
        .video-sheet { width:100%; max-width:920px; border-radius:12px; overflow:hidden; background:#0a0a0a; border:1px solid rgba(255,255,255,0.03); transform:translateY(6px); opacity:0; transition:transform .18s, opacity .18s; }
        .video-sheet.show { transform:translateY(0); opacity:1; }
        .overlay-player { width:100%; height:calc(100vw * 9/16); max-height:480px; background:#000; display:block; }

        /* Controls row positioned immediately below player in requested order */
        .overlay-controls { display:flex; gap:10px; align-items:center; padding:10px 12px; border-top:1px solid rgba(255,255,255,0.02); }
        .control-btn {
            display:inline-flex; align-items:center; gap:8px; padding:8px 12px; border-radius:8px; background:rgba(255,255,255,0.02);
            border:1px solid rgba(255,255,255,0.03); cursor:pointer; color:#fff; font-weight:700;
        }
        .control-btn.like.active { background:linear-gradient(90deg,#ff7b8a,#ff4757); color:#fff; }
        .control-btn .icon { width:18px; height:18px; display:inline-block; }

        /* Channel row sits below the controls, with visit & subscribe buttons */
        .channel-row { display:flex; align-items:center; gap:12px; padding:12px; border-top:1px solid rgba(255,255,255,0.02); }
        .channel-avatar { width:44px; height:44px; border-radius:50%; background:#111; border:1px solid rgba(255,255,255,0.03); display:inline-block; cursor:pointer; }
        .channel-meta { flex:1; }
        .channel-meta .name { font-weight:800; font-size:1rem; cursor:pointer; }
        .channel-meta .subs { color:#bbb; font-size:0.9rem; }

        .subscribe-btn { padding:8px 12px; border-radius:999px; background:#ff8b2f; border:0; color:#111; font-weight:800; cursor:pointer; }

        /* Comments area immediately below channel row as requested */
        .comments-section { padding:12px; border-top:1px solid rgba(255,255,255,0.02); max-height:260px; overflow:auto; }
        .comment { display:flex; gap:10px; margin-bottom:10px; }
        .comment .avatar { width:36px; height:36px; border-radius:50%; background:#111; }
        .comment .body { }
        .comment .author { font-weight:700; color:#ff8b98; }
        .comment-input { display:flex; gap:8px; margin-top:8px; }
        .comment-input input { flex:1; padding:8px 10px; border-radius:8px; background:#060606; border:1px solid rgba(255,255,255,0.03); color:#fff; }

        /* Recommended below comments */
        .recommended { padding:12px; border-top:1px solid rgba(255,255,255,0.02); display:flex; gap:8px; overflow:auto; }
        .rec-item { min-width:160px; max-width:160px; background:#0f0f0f; border-radius:8px; padding:6px; cursor:pointer; border:1px solid rgba(255,255,255,0.03); }
        .rec-item img { width:100%; height:88px; object-fit:cover; border-radius:6px; display:block; }

        /* Subscription modal styles reused */
        .modal-backdrop {
            position:fixed; left:0; top:0; right:0; bottom:0; background:rgba(0,0,0,0.72);
            display:none; align-items:center; justify-content:center; z-index:2000;
        }
        .modal {
            background:#0f0f0f; padding:18px; border-radius:12px; width: 100%; max-width: 560px; color:#fff;
            box-shadow:0 12px 40px rgba(0,0,0,0.8);
        }

        /* Liked modal + channel + auth modal reuse modal-backdrop but separate ids below */
        .modal-list { max-height:380px; overflow:auto; margin-top:8px; display:flex; flex-direction:column; gap:8px; }
        .modal-list .liked-entry { display:flex; gap:8px; align-items:center; background:#0d0d0d; padding:8px; border-radius:8px; border:1px solid rgba(255,255,255,0.02); }
        .liked-entry img { width:96px; height:56px; object-fit:cover; border-radius:6px; }
        .liked-entry .meta { flex:1; }

        /* Channel modal specific */
        .channel-stats { display:flex; gap:12px; margin-top:8px; color:#ccc; }
        .channel-stats .stat { font-weight:800; color:#fff; }

        /* Small utilities */
        .btn { background:#ff4757; color:#fff; padding:10px 14px; border-radius:20px; border:0; cursor:pointer; font-weight:700; }
        .btn.secondary { background:#222; color:#ddd; border:1px solid rgba(255,255,255,0.03); }

        /* Responsive tweaks */
        @media (max-width:520px) {
            .overlay-player { max-height:320px; }
            .rec-item { min-width:120px; max-width:120px; }
            .floating-search { top:72px; left:50%; transform:translateX(-50%); }
        }
        /* mark highlight style */
        mark { background:#ffea; color:#000; border-radius:4px; padding:0 4px; }
    </style>
</head>
<body>
    <!-- AGE GATE: confirm majority age before using site -->
    <div id="age-gate" role="dialog" aria-modal="true" aria-labelledby="age-gate-title" style="display:none; position:fixed; inset:0; align-items:center; justify-content:center; z-index:5000; background:rgba(0,0,0,0.75);">
        <div style="max-width:560px;margin:0 auto;background:#121212;padding:28px;border-radius:12px; box-shadow:0 12px 40px rgba(0,0,0,0.8);">
            <h2 id="age-gate-title" style="margin-bottom:8px;">Confirmación de Mayoría de Edad</h2>
            <p style="color:#ccc;margin-bottom:12px;">Este sitio contiene material para adultos. Debes ser mayor de 18 años para entrar.</p>
            <label style="color:#ddd;display:block;margin-bottom:12px;"><input id="age-check" type="checkbox" /> Declaro que tengo 18 años o más.</label>
            <div style="display:flex;gap:8px;justify-content:center;">
                <button class="btn" id="confirm-age">Entrar</button>
                <a class="btn secondary" id="exit-site" href="https://www.google.com" target="_blank" rel="noopener">Salir</a>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="header-inner">
            <div class="left">
                <button id="menu-toggle" class="menu-toggle" aria-label="Abrir menú" aria-controls="side-menu" aria-expanded="false">
                    <span class="bar" aria-hidden="true"></span>
                </button>
            </div>

            <div class="center">
                <div class="brand" id="brand">SexZone</div>
            </div>

            <div class="right" style="position:relative;">
                <div style="width:100%;max-width:520px;" class="search-bar">
                    <div id="search-icon" class="search-icon" aria-hidden="true" title="Buscar">
                        <!-- simple magnifier SVG -->
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M21 21l-4.35-4.35" stroke="#ddd" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/><circle cx="11" cy="11" r="5" stroke="#ddd" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    </div>
                    <input id="search-input" type="search" placeholder="Buscar" aria-label="Buscar" />
                </div>

                <!-- Profile circle -->
                <div style="margin-left:8px; position:relative;">
                    <button id="profile-btn" class="profile-btn" aria-haspopup="true" aria-expanded="false" aria-controls="profile-menu" title="Perfil">
                        <span class="profile-dot" aria-hidden="true"></span>
                    </button>
                    <div id="profile-menu" class="profile-menu" role="menu" aria-hidden="true">
                        <!-- profile-email inserted dynamically when logged in -->
                        <button id="profile-account" role="menuitem">Cuenta</button>
                        <button id="liked-videos" role="menuitem">Videos que te gustaron</button>
                        <button id="upload-open" role="menuitem">Subir</button>
                        <button id="profile-logout" role="menuitem">Cerrar sesión</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Primary nav (desktop) -->
        <nav id="primary-nav" class="container" aria-label="Navegación principal">
            <div class="nav-item" role="link" tabindex="0" data-href="#videos">Videos</div>
            <div class="nav-item" role="link" tabindex="0" data-href="#categorias">Categorías</div>
            <div class="nav-item" role="link" tabindex="0" data-href="#mas-vistos">Más Vistos</div>
            <div class="nav-item" role="link" tabindex="0" data-href="#suscripcion">Suscripción</div>
        </nav>
    </header>

    <!-- Floating search that appears when clicking the magnifier -->
    <div id="floating-search" class="floating-search" role="dialog" aria-hidden="true" style="display:none;">
        <div class="fs-text">Buscar</div>
        <input id="floating-search-input" type="search" placeholder="Escribe para buscar..." aria-label="Buscar" />
        <button id="floating-search-close" class="btn secondary" style="padding:6px 10px;">Cerrar</button>
    </div>

    <!-- Side menu (mobile) -->
    <div id="side-overlay" class="side-overlay" style="display:none;"></div>
    <aside id="side-menu" class="side-menu" aria-hidden="true">
        <div style="margin-bottom:12px;">
            <strong style="font-size:1.05rem;">Menú</strong>
        </div>
        <a class="side-item" href="#videos">Videos</a>
        <a class="side-item" href="#categorias">Categorías</a>
        <a class="side-item" href="#mas-vistos">Más Vistos</a>
        <a class="side-item" href="#suscripcion">Suscripción</a>
        <div style="margin-top:18px;">
            <button class="side-item" id="side-login">Entrar / Crear cuenta</button>
            <button class="side-item" id="side-subscribe">Suscribirse</button>
        </div>
    </aside>

    <!-- Main -->
    <main class="container" id="site-main" aria-live="polite">
        <section id="videos">
            <h2 style="margin-bottom:10px;">Inicio</h2>

            <div class="grid" id="videos-grid">
                <article class="video-item" tabindex="0" data-id="v1" data-title="Video 1 Título" data-src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" data-poster="placeholder-video1.jpg" data-channel="JockPussy" data-description="Escena íntima en exteriores">
                    <img class="video-thumbnail" src="placeholder-video1.jpg" alt="Miniatura del video 1" loading="lazy" />
                    <div class="video-info">
                        <h3>Video 1 Título</h3>
                        <p>1.2M vistas</p>
                    </div>
                </article>

                <article class="video-item" tabindex="0" data-id="v2" data-title="Video 2 Título" data-src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" data-poster="placeholder-video2.jpg" data-channel="JockPussy" data-description="Actuación apasionada en habitación">
                    <img class="video-thumbnail" src="placeholder-video2.jpg" alt="Miniatura del video 2" loading="lazy" />
                    <div class="video-info">
                        <h3>Video 2 Título</h3>
                        <p>850K vistas</p>
                    </div>
                </article>

                <article class="video-item" tabindex="0" data-id="v3" data-title="Video 3 Título" data-src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" data-poster="placeholder-video3.jpg" data-channel="OtherChannel" data-description="Montaje recopilatorio viral">
                    <img class="video-thumbnail" src="placeholder-video3.jpg" alt="Miniatura del video 3" loading="lazy" />
                    <div class="video-info">
                        <h3>Video 3 Título</h3>
                        <p>2.5M vistas</p>
                    </div>
                </article>
            </div>

            <!-- No-results message area for searches -->
            <div id="search-no-results" class="no-results" style="display:none;">
                No hay resultados de su búsqueda.
            </div>
        </section>

        <section id="categorias" style="margin-top:12px;">
            <h2>Categorías Populares</h2>
            <div class="category-pills" role="toolbar" aria-label="Filtros">
                <button class="pill" data-cat="gay">Gay</button>
                <button class="pill" data-cat="lesbianas">Lesbianas</button>
                <button class="pill" data-cat="hetero">Hetero</button>
                <button class="pill" data-cat="trans">Trans</button>
                <button class="pill" data-cat="recomendados">Recomendados</button>
            </div>

            <div class="grid" style="margin-top:8px;">
                <div class="video-item" tabindex="0" role="button">
                    <img class="video-thumbnail" src="placeholder-category1.jpg" alt="Categoría Amateur" loading="lazy" />
                    <div class="video-info"><h3>Categoría Amateur</h3></div>
                </div>
                <div class="video-item" tabindex="0" role="button">
                    <img class="video-thumbnail" src="placeholder-category2.jpg" alt="Categoría MILF" loading="lazy" />
                    <div class="video-info"><h3>MILF</h3></div>
                </div>
            </div>
        </section>

        <section id="mas-vistos" style="margin-top:12px;">
            <h2>Más Vistos</h2>
            <div class="grid" style="margin-top:8px;">
                <article class="video-item" tabindex="0"><img class="video-thumbnail" src="placeholder-video3.jpg" alt="Miniatura video 3" loading="lazy" /><div class="video-info"><h3>Video 3 Título</h3><p>2.5M vistas</p></div></article>
            </div>
        </section>

        <section id="suscripcion" style="margin-top:12px;">
            <h2>Suscripción Premium</h2>
            <div style="margin-top:8px; padding:12px; background:#0f0f0f; border-radius:10px; border:1px solid rgba(255,255,255,0.03);">
                <div style="display:flex; align-items:center; justify-content:space-between;">
                    <div><strong style="font-size:1.05rem;">Accede a contenido exclusivo</strong><div style="color:#bbb;margin-top:6px;">$8.05 / mes</div></div>
                    <div><button class="btn" id="subscribe-cta">Suscribirme</button></div>
                </div>
            </div>
        </section>
    </main>

    <footer style="padding:14px 0; text-align:center; border-top:1px solid rgba(255,255,255,0.02);">
        <div style="color:#bbb;">&copy; <span id="year"></span> SexZone. Contenido solo para mayores de 18 años.</div>
    </footer>

    <!-- Video overlay: player + controls + channel + comments + recommended -->
    <div id="video-overlay" class="video-overlay" aria-hidden="true" style="display:none;">
        <div class="video-sheet" role="dialog" aria-modal="true" aria-labelledby="overlay-title">
            <div style="display:flex;justify-content:space-between;align-items:center;padding:10px 12px;">
                <strong id="overlay-title">Título del video</strong>
                <button id="close-overlay" class="btn secondary">Cerrar</button>
            </div>

            <video id="overlay-player" class="overlay-player" controls playsinline preload="auto" src=""></video>

            <!-- Controls row: like, compartir, reportar (ordered as requested) -->
            <div class="overlay-controls" role="toolbar" aria-label="Controles del video">
                <button id="like-btn" class="control-btn like" title="Me gusta">
                    <span class="icon" aria-hidden="true">👍</span><span id="like-count">0</span>
                </button>

                <button id="share-btn" class="control-btn" title="Compartir">
                    <span class="icon" aria-hidden="true">🔗</span>Compartir
                </button>

                <button id="report-btn" class="control-btn" title="Reportar">
                    <span class="icon" aria-hidden="true">🚩</span>Reportar
                </button>

            </div>

            <!-- Channel row with access & subscribe (below the three control buttons) -->
            <div class="channel-row" aria-label="Información del canal">
                <div class="channel-avatar" id="channel-avatar" aria-hidden="true"></div>
                <div class="channel-meta">
                    <div class="name" id="channel-name">Canal</div>
                    <div class="subs" id="channel-subs">0 suscriptores</div>
                </div>

                <div style="display:flex;gap:8px;align-items:center;">
                    <button id="visit-channel-btn" class="control-btn" title="Ir al canal">Ir al canal</button>
                    <button id="subscribe-channel-btn" class="subscribe-btn" title="Suscribirse">Suscribirse</button>
                </div>
            </div>

            <!-- Comments immediately below channel row -->
            <div class="comments-section" id="comments-wrapper">
                <div id="comments-list" aria-live="polite">
                    <!-- comments inserted here -->
                </div>

                <div style="padding-top:8px;">
                    <div class="comment-input">
                        <input id="comment-input" type="text" placeholder="Añadir un comentario..." aria-label="Añadir comentario" />
                        <button id="comment-send" class="btn">Publicar</button>
                    </div>
                </div>
            </div>

            <!-- Recommended below comments -->
            <div style="padding:8px 12px;">
                <strong style="display:block;margin-bottom:8px;">Recomendado</strong>
                <div class="recommended" id="recommended-list" aria-label="Videos recomendados">
                    <!-- recommended items inserted dynamically -->
                </div>
            </div>
        </div>
    </div>

    <!-- Liked videos modal (accessed from profile menu) -->
    <div id="liked-modal" class="modal-backdrop" aria-hidden="true" style="display:none; z-index:3500;">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="liked-modal-title" tabindex="-1">
            <h3 id="liked-modal-title">Videos que te gustaron</h3>
            <div id="liked-list" class="modal-list">
                <!-- liked videos inserted here -->
            </div>
            <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:12px;">
                <button class="btn secondary" id="liked-close">Cerrar</button>
            </div>
        </div>
    </div>

    <!-- Channel modal (shows channel videos, seguidos, seguidores) -->
    <div id="channel-modal" class="modal-backdrop" aria-hidden="true" style="display:none; z-index:3600;">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="channel-modal-title" tabindex="-1">
            <h3 id="channel-modal-title">Canal</h3>
            <div id="channel-info" style="margin-top:8px;">
                <div style="display:flex;align-items:center;gap:12px;">
                    <div style="width:72px;height:72px;border-radius:50%;background:#111;border:1px solid rgba(255,255,255,0.03)"></div>
                    <div>
                        <div id="ch-name" style="font-weight:800;font-size:1.1rem;"></div>
                        <div class="channel-stats" style="margin-top:6px;">
                            <div class="stat" id="ch-videos-count"></div>
                            <div class="stat" id="ch-following-count"></div>
                            <div class="stat" id="ch-followers-count"></div>
                        </div>
                    </div>
                </div>
                <div style="display:flex;gap:8px;margin-top:10px;">
                    <button id="ch-follow-btn" class="btn">Seguir</button>
                    <button id="ch-close-btn" class="btn secondary">Cerrar</button>
                </div>
                <div style="margin-top:12px;">
                    <strong>Videos del canal</strong>
                    <div id="ch-videos" class="modal-list" style="margin-top:8px;"></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Auth modal (Entrar / Crear cuenta) -->
    <div id="auth-modal" class="modal-backdrop" aria-hidden="true" style="display:none; z-index:3700;">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="auth-modal-title" tabindex="-1">
            <h3 id="auth-modal-title">Entrar / Crear cuenta</h3>
            <div style="margin-top:8px; display:flex;gap:8px;">
                <button id="show-login" class="btn">Iniciar sesión</button>
                <button id="show-register" class="btn secondary">Registrarse</button>
            </div>

            <div id="auth-forms" style="margin-top:12px;">
                <!-- Login form -->
                <div id="login-form" style="display:none;">
                    <label style="display:block;margin-bottom:6px;color:#ccc;">Correo</label>
                    <input id="login-email" type="email" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:8px;" />
                    <label style="display:block;margin-bottom:6px;color:#ccc;">Contraseña</label>
                    <input id="login-pass" type="password" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:8px;" />
                    <div style="display:flex;gap:8px;justify-content:flex-end;">
                        <button id="login-submit" class="btn">Entrar</button>
                    </div>
                </div>

                <!-- Register form -->
                <div id="register-form" style="display:none;">
                    <label style="display:block;margin-bottom:6px;color:#ccc;">Correo</label>
                    <input id="reg-email" type="email" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:8px;" />
                    <label style="display:block;margin-bottom:6px;color:#ccc;">Contraseña</label>
                    <input id="reg-pass" type="password" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:8px;" />
                    <div style="display:flex;gap:8px;justify-content:flex-end;">
                        <button id="reg-submit" class="btn">Crear cuenta</button>
                    </div>
                </div>
            </div>

            <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:12px;">
                <button id="auth-close" class="btn secondary">Cerrar</button>
            </div>
        </div>
    </div>

    <!-- Account / Creator tools modal -->
    <div id="account-modal" class="modal-backdrop" aria-hidden="true" style="display:none; z-index:3800;">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="account-modal-title" tabindex="-1">
            <h3 id="account-modal-title">Cuenta y Herramientas de Creador</h3>

            <div style="margin-top:8px;">
                <strong>Datos de la cuenta</strong>
                <div style="margin-top:8px;">
                    <label style="display:block;color:#ccc;margin-bottom:6px;">Apodo (nickname)</label>
                    <input id="acct-nickname" type="text" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;" />
                    <div style="height:8px;"></div>

                    <label style="display:block;color:#ccc;margin-bottom:6px;">Cambiar contraseña (opcional)</label>
                    <input id="acct-current-pass" type="password" placeholder="Contraseña actual" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:6px;" />
                    <input id="acct-new-pass" type="password" placeholder="Nueva contraseña" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:6px;" />
                    <input id="acct-new-pass-confirm" type="password" placeholder="Confirmar nueva contraseña" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;margin-bottom:6px;" />
                    <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:8px;">
                        <button id="acct-save" class="btn">Guardar</button>
                        <button id="acct-cancel" class="btn secondary">Cerrar</button>
                    </div>
                </div>

                <div style="height:12px;"></div>

                <strong>Herramientas de creador</strong>
                <div style="margin-top:8px;color:#ccc;">
                    <label style="display:flex;align-items:center;gap:8px;"><input id="acct-is-creator" type="checkbox" /> Activar herramientas de creador</label>
                    <div id="creator-tools" style="margin-top:10px; display:none;">
                        <div style="display:flex;gap:8px;">
                            <button id="creator-upload" class="btn">Subir contenido</button>
                            <button id="creator-manage" class="btn secondary">Ver mis contenidos</button>
                        </div>
                        <div style="margin-top:8px;color:#aaa;font-size:0.9rem;">Nota: Subidas demo se almacenan localmente en tu navegador.</div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Subscription modal (payment removed: simplified demo subscription) -->
    <div id="modal-backdrop" class="modal-backdrop" aria-hidden="true">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="modal-title" tabindex="-1">
            <div id="modal-content"></div>
        </div>
    </div>

    <!-- Hidden upload input (triggered from profile menu or creator tools) -->
    <input id="file-input" type="file" accept="video/*,image/*" style="display:none" />

    <!-- Profile Upload modal (simple) -->
    <div id="upload-modal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.7); z-index:4000; align-items:center; justify-content:center;">
        <div style="background:#0f0f0f;padding:16px;border-radius:12px; width:calc(100% - 40px); max-width:560px;">
            <h3 style="margin-bottom:8px;">Subir contenido</h3>
            <p style="color:#bbb;margin-bottom:10px;">Selecciona una opción para subir desde tu dispositivo.</p>
            <div style="display:flex;gap:8px;flex-wrap:wrap;">
                <button id="upload-from-device" class="btn">Desde dispositivo</button>
                <button id="upload-cancel" class="btn secondary">Cancelar</button>
            </div>
        </div>
    </div>

    <script>
        document.getElementById('year').textContent = new Date().getFullYear();

        // Age gate logic: require confirmation before interacting with site
        const AGE_KEY = 'sz_age_confirmed';
        const ageGate = document.getElementById('age-gate');
        try {
            if (localStorage.getItem(AGE_KEY) === 'true') { ageGate.style.display='none'; }
            else { ageGate.style.display='flex'; document.getElementById('confirm-age').focus(); }
        } catch(e) { ageGate.style.display='flex'; }

        document.getElementById('confirm-age').addEventListener('click', () => {
            const ck = document.getElementById('age-check');
            if (!ck.checked) { alert('Debes confirmar que eres mayor de 18 años.'); ck.focus(); return; }
            try { localStorage.setItem(AGE_KEY,'true'); } catch(e){}
            ageGate.style.display='none';
        });

        // Side menu mobile
        const menuToggle = document.getElementById('menu-toggle');
        const sideMenu = document.getElementById('side-menu');
        const sideOverlay = document.getElementById('side-overlay');
        menuToggle.addEventListener('click', () => {
            const open = sideMenu.classList.toggle('open');
            sideOverlay.style.display = open ? 'block' : 'none';
            menuToggle.setAttribute('aria-expanded', String(open));
            if (open) sideMenu.setAttribute('aria-hidden','false'); else sideMenu.setAttribute('aria-hidden','true');
        });
        sideOverlay.addEventListener('click', () => { sideMenu.classList.remove('open'); sideOverlay.style.display='none'; menuToggle.setAttribute('aria-expanded','false'); });

        // Primary nav items (desktop) clickable
        document.querySelectorAll('#primary-nav .nav-item').forEach(el => {
            el.addEventListener('click', () => {
                const href = el.getAttribute('data-href');
                if (href) location.hash = href;
            });
            el.addEventListener('keydown', (e) => { if (e.key === 'Enter') el.click(); });
        });

        // Overlay elements
        const videoOverlay = document.getElementById('video-overlay');
        const videoSheet = document.querySelector('.video-sheet');
        const overlayPlayer = document.getElementById('overlay-player');
        const overlayTitle = document.getElementById('overlay-title');
        const closeOverlay = document.getElementById('close-overlay');

        // Controls
        const likeBtn = document.getElementById('like-btn');
        const likeCountEl = document.getElementById('like-count');
        const shareBtn = document.getElementById('share-btn');
        const reportBtn = document.getElementById('report-btn');

        // Comments & channel
        const commentsWrapper = document.getElementById('comments-wrapper');
        const commentsList = document.getElementById('comments-list');
        const commentInput = document.getElementById('comment-input');
        const commentSend = document.getElementById('comment-send');

        const channelNameEl = document.getElementById('channel-name');
        const channelSubsEl = document.getElementById('channel-subs');
        const subscribeChannelBtn = document.getElementById('subscribe-channel-btn');
        const visitChannelBtn = document.getElementById('visit-channel-btn');

        const recommendedList = document.getElementById('recommended-list');

        // Floating search elements
        const searchIcon = document.getElementById('search-icon');
        const floatingSearch = document.getElementById('floating-search');
        const floatingSearchInput = document.getElementById('floating-search-input');
        const floatingSearchClose = document.getElementById('floating-search-close');

        // Liked modal elements
        const likedModal = document.getElementById('liked-modal');
        const likedList = document.getElementById('liked-list');
        const likedClose = document.getElementById('liked-close');
        const likedBtnInMenu = document.getElementById('liked-videos');

        // Auth modal elements
        const authModal = document.getElementById('auth-modal');
        const sideLoginBtn = document.getElementById('side-login');
        const showLoginBtn = document.getElementById('show-login');
        const showRegisterBtn = document.getElementById('show-register');
        const loginForm = document.getElementById('login-form');
        const registerForm = document.getElementById('register-form');
        const loginSubmit = document.getElementById('login-submit');
        const regSubmit = document.getElementById('reg-submit');
        const authClose = document.getElementById('auth-close');

        // Account modal elements
        const accountModal = document.getElementById('account-modal');
        const acctNickname = document.getElementById('acct-nickname');
        const acctCurrentPass = document.getElementById('acct-current-pass');
        const acctNewPass = document.getElementById('acct-new-pass');
        const acctNewPassConfirm = document.getElementById('acct-new-pass-confirm');
        const acctSave = document.getElementById('acct-save');
        const acctCancel = document.getElementById('acct-cancel');
        const acctIsCreator = document.getElementById('acct-is-creator');
        const creatorTools = document.getElementById('creator-tools');
        const creatorUpload = document.getElementById('creator-upload');
        const creatorManage = document.getElementById('creator-manage');

        // Channel modal elements
        const channelModal = document.getElementById('channel-modal');
        const chTitle = document.getElementById('channel-modal-title');
        const chNameEl = document.getElementById('ch-name');
        const chVideosCount = document.getElementById('ch-videos-count');
        const chFollowingCount = document.getElementById('ch-following-count');
        const chFollowersCount = document.getElementById('ch-followers-count');
        const chVideosContainer = document.getElementById('ch-videos');
        const chFollowBtn = document.getElementById('ch-follow-btn');
        const chCloseBtn = document.getElementById('ch-close-btn');

        // Utilities for storage keys
        function likesKey(videoId){ return 'likes_' + videoId; }
        function commentsKey(videoId){ return 'comments_' + videoId; }
        function reportedKey(){ return 'reported_videos'; }
        function subscribedChannelsKey(){ return 'subscribed_channels'; }
        function likedVideosKey(){ return 'liked_videos'; }
        function channelFollowersKey(channel){ return `channel_${channel}_followers`; }
        function channelFollowingKey(channel){ return `channel_${channel}_following`; }
        function uploadedVideosKeyForUser(userId){ return `sz_uploaded_videos_${userId}`; }

        // Build recommended list
        function buildRecommended(videoId){
            recommendedList.innerHTML = '';
            const all = Array.from(document.querySelectorAll('.video-item'));
            all.forEach(item => {
                const id = item.dataset.id || item.getAttribute('data-title');
                if (id === videoId) return;
                const thumb = item.querySelector('img')?.src || '';
                const title = item.dataset.title || item.querySelector('h3')?.textContent || 'Video';
                const rec = document.createElement('div');
                rec.className = 'rec-item';
                rec.tabIndex = 0;
                rec.innerHTML = `<img src="${thumb}" alt="${title}"><div style="margin-top:6px;font-weight:700;font-size:0.9rem;">${title}</div>`;
                rec.addEventListener('click', ()=> loadVideoToOverlay(item));
                rec.addEventListener('keydown', (e)=> { if (e.key === 'Enter') loadVideoToOverlay(item); });
                recommendedList.appendChild(rec);
            });
        }

        // Load comments
        function loadComments(videoId){
            commentsList.innerHTML = '';
            const raw = localStorage.getItem(commentsKey(videoId)) || '[]';
            let arr = [];
            try { arr = JSON.parse(raw); } catch(e){ arr = []; }
            if (arr.length === 0){
                commentsList.innerHTML = `<div style="color:#bbb;padding:8px;">Sé el primero en comentar.</div>`;
                return;
            }
            arr.forEach(c => {
                const el = document.createElement('div');
                el.className = 'comment';
                el.innerHTML = `<div class="avatar" aria-hidden="true"></div><div class="body"><div class="author">${escapeHtml(c.author)}</div><div style="color:#ccc;font-size:0.95rem;">${escapeHtml(c.text)}</div><div style="color:#777;font-size:0.8rem;margin-top:6px;">${new Date(c.when).toLocaleString()}</div></div>`;
                commentsList.appendChild(el);
            });
            commentsList.scrollTop = commentsList.scrollHeight;
        }

        // Save comment
        function saveComment(videoId, author, text){
            const key = commentsKey(videoId);
            let arr = [];
            try { arr = JSON.parse(localStorage.getItem(key) || '[]'); } catch(e){ arr = []; }
            arr.push({author: author || 'Anon', text, when: new Date().toISOString()});
            try { localStorage.setItem(key, JSON.stringify(arr)); } catch(e){}
            loadComments(videoId);
        }

        // Liked videos helpers
        function getLikedVideos(){
            try { return JSON.parse(localStorage.getItem(likedVideosKey()) || '[]'); } catch(e){ return []; }
        }
        function saveLikedVideos(arr){
            try { localStorage.setItem(likedVideosKey(), JSON.stringify(arr)); } catch(e){}
        }
        function addToLiked(videoObj){
            const arr = getLikedVideos();
            if (!arr.find(v => v.id === videoObj.id)) {
                arr.push(videoObj);
                saveLikedVideos(arr);
            }
        }
        function removeFromLiked(videoId){
            let arr = getLikedVideos();
            arr = arr.filter(v => v.id !== videoId);
            saveLikedVideos(arr);
        }

        // Like toggle (now also updates a liked_videos list)
        function toggleLike(videoId){
            const k = likesKey(videoId);
            let data = {count:0, liked:false};
            try { data = JSON.parse(localStorage.getItem(k) || JSON.stringify(data)); } catch(e){}
            data.liked = !data.liked;
            data.count = data.liked ? (data.count || 0) + 1 : Math.max(0, (data.count || 1) - 1);
            try { localStorage.setItem(k, JSON.stringify(data)); } catch(e){}
            likeBtn.classList.toggle('active', data.liked);
            likeCountEl.textContent = data.count;

            // Update liked videos list
            const el = Array.from(document.querySelectorAll('.video-item')).find(x => (x.dataset.id || x.dataset.title) === videoId);
            const vidObj = {
                id: videoId,
                title: el?.dataset.title || el?.querySelector('h3')?.textContent || 'Video',
                src: el?.dataset.src || '',
                poster: el?.dataset.poster || el?.querySelector('img')?.src || '',
                channel: el?.dataset.channel || ''
            };
            if (data.liked) addToLiked(vidObj);
            else removeFromLiked(videoId);
        }

        // Report
        function reportVideo(videoId){
            const raw = localStorage.getItem(reportedKey()) || '[]';
            let arr = [];
            try { arr = JSON.parse(raw); } catch(e){ arr = []; }
            if (!arr.includes(videoId)) arr.push(videoId);
            try { localStorage.setItem(reportedKey(), JSON.stringify(arr)); } catch(e){}
            alert('Gracias. El video ha sido marcado para revisión (simulación).');
        }

        // Subscribe channel
        function toggleSubscribe(channelName){
            let arr = [];
            try { arr = JSON.parse(localStorage.getItem(subscribedChannelsKey()) || '[]'); } catch(e){ arr = []; }
            const idx = arr.indexOf(channelName);
            if (idx === -1){
                arr.push(channelName);
                subscribeChannelBtn.textContent = 'Suscrito';
                subscribeChannelBtn.style.background = '#9be8b6';
                subscribeChannelBtn.style.color = '#072';
            } else {
                arr.splice(idx,1);
                subscribeChannelBtn.textContent = 'Suscribirse';
                subscribeChannelBtn.style.background = '#ff8b2f';
                subscribeChannelBtn.style.color = '#111';
            }
            try { localStorage.setItem(subscribedChannelsKey(), JSON.stringify(arr)); } catch(e){}
            channelSubsEl.textContent = `${(100 + (Math.floor(Math.random()*900))).toLocaleString()} suscriptores`;
        }

        // Visit channel (open channel modal)
        function visitChannel(channelName){
            openChannelModal(channelName);
        }

        // Robust event delegation to open videos (works even if items added later)
        const videosGrid = document.getElementById('videos-grid');
        videosGrid.addEventListener('click', function(e){
            const item = e.target.closest('.video-item');
            if (!item) return;
            loadVideoToOverlay(item);
        });
        videosGrid.addEventListener('keydown', function(e){
            if (e.key === 'Enter' || e.key === ' ') {
                const item = e.target.closest('.video-item');
                if (item) { e.preventDefault(); loadVideoToOverlay(item); }
            }
        });

        // Load a video item into overlay (keeps page unchanged)
        function loadVideoToOverlay(item){
            const videoId = item.dataset.id || item.dataset.title || 'unknown';
            const title = item.dataset.title || item.querySelector('h3')?.textContent || 'Video';
            const src = item.dataset.src || '';
            const poster = item.dataset.poster || item.querySelector('img')?.src || '';
            const channel = item.dataset.channel || ('Canal de ' + title);

            overlayTitle.textContent = title;
            overlayPlayer.src = src;
            overlayPlayer.poster = poster;

            // load likes
            try {
                const lk = JSON.parse(localStorage.getItem(likesKey(videoId)) || '{"count":0,"liked":false}');
                likeCountEl.textContent = lk.count || 0;
                likeBtn.classList.toggle('active', !!lk.liked);
            } catch(e){
                likeCountEl.textContent = '0';
                likeBtn.classList.remove('active');
            }

            // load comments
            loadComments(videoId);

            // channel
            channelNameEl.textContent = channel;
            channelNameEl.dataset.channel = channel;
            channelSubsEl.textContent = `${(100 + (Math.floor(Math.random()*900))).toLocaleString()} suscriptores`;
            const subs = JSON.parse(localStorage.getItem(subscribedChannelsKey()) || '[]');
            if (subs.includes(channel)){
                subscribeChannelBtn.textContent = 'Suscrito';
                subscribeChannelBtn.style.background = '#9be8b6';
                subscribeChannelBtn.style.color = '#072';
            } else {
                subscribeChannelBtn.textContent = 'Suscribirse';
                subscribeChannelBtn.style.background = '#ff8b2f';
                subscribeChannelBtn.style.color = '#111';
            }

            videoOverlay.dataset.currentVideo = videoId;
            videoOverlay.dataset.currentChannel = channel;

            buildRecommended(videoId);

            // show overlay
            videoOverlay.style.display = 'flex';
            requestAnimationFrame(()=> videoSheet.classList.add('show'));
            // Try to play only if there's a src; otherwise user can press play
            if (src) overlayPlayer.play().catch(()=>{});
            // SHOW comments by default as requested
            commentsWrapper.style.display = 'block';
        }

        // Controls events
        likeBtn.addEventListener('click', () => {
            const vid = videoOverlay.dataset.currentVideo;
            if (!vid) return;
            toggleLike(vid);
            // update liked modal if open
            if (likedModal.style.display === 'flex') renderLikedModal();
        });

        shareBtn.addEventListener('click', async () => {
            const vid = videoOverlay.dataset.currentVideo;
            const title = overlayTitle.textContent;
            const url = location.href + '#video=' + encodeURIComponent(vid);
            if (navigator.share) {
                try { await navigator.share({ title, url }); } catch(e){}
            } else {
                try { await navigator.clipboard.writeText(url); alert('Enlace copiado al portapapeles (demo).'); } catch(e){ prompt('Copia el enlace:', url); }
            }
        });

        reportBtn.addEventListener('click', () => {
            const vid = videoOverlay.dataset.currentVideo;
            if (!vid) return;
            if (confirm('¿Deseas reportar este video?')) reportVideo(vid);
        });

        commentSend.addEventListener('click', () => {
            const vid = videoOverlay.dataset.currentVideo;
            if (!vid) return;
            const text = commentInput.value.trim();
            if (!text) return;
            let user = 'You';
            try { const u = JSON.parse(localStorage.getItem('sz_user') || 'null'); if (u && u.email) user = u.email.split('@')[0]; } catch(e){}
            saveComment(vid, user, text);
            commentInput.value = '';
        });

        // channel buttons
        subscribeChannelBtn.addEventListener('click', () => {
            const channel = videoOverlay.dataset.currentChannel || channelNameEl.textContent;
            toggleSubscribe(channel);
        });
        visitChannelBtn.addEventListener('click', () => {
            const channel = videoOverlay.dataset.currentChannel || channelNameEl.textContent;
            visitChannel(channel);
        });

        // Also open channel if clicking the channel name inside the overlay
        channelNameEl.addEventListener('click', () => {
            const channel = channelNameEl.dataset.channel || channelNameEl.textContent;
            openChannelModal(channel);
        });

        // Close overlay
        closeOverlay.addEventListener('click', closeVideoOverlay);
        videoOverlay.addEventListener('click', (e) => { if (e.target === videoOverlay) closeVideoOverlay(); });
        function closeVideoOverlay(){
            overlayPlayer.pause();
            overlayPlayer.currentTime = 0;
            overlayPlayer.src = '';
            videoSheet.classList.remove('show');
            setTimeout(()=> videoOverlay.style.display='none', 200);
        }

        // Profile menu toggling + actions (upload flow unchanged)
        const profileBtn = document.getElementById('profile-btn');
        const profileMenu = document.getElementById('profile-menu');
        profileBtn.addEventListener('click', (e)=> {
            const open = profileMenu.classList.toggle('show');
            profileBtn.setAttribute('aria-expanded', String(open));
            profileMenu.setAttribute('aria-hidden', String(!open));
            if (open) profileMenu.querySelector('button')?.focus();
        });
        document.addEventListener('click', (e) => {
            if (!profileBtn.contains(e.target) && !profileMenu.contains(e.target)) {
                profileMenu.classList.remove('show');
                profileBtn.setAttribute('aria-expanded', 'false');
                profileMenu.setAttribute('aria-hidden', 'true');
            }
        });

        // Upload modal
        const uploadOpenBtn = document.getElementById('upload-open');
        const uploadModal = document.getElementById('upload-modal');
        const fileInput = document.getElementById('file-input');
        uploadOpenBtn.addEventListener('click', ()=> {
            profileMenu.classList.remove('show');
            uploadModal.style.display = 'flex';
            uploadModal.setAttribute('aria-hidden','false');
            document.getElementById('upload-from-device').focus();
        });
        document.getElementById('upload-cancel').addEventListener('click', ()=> { uploadModal.style.display='none'; });
        document.getElementById('upload-from-device').addEventListener('click', ()=> { uploadModal.style.display='none'; fileInput.click(); });

        // When file selected we create a demo video item and persist metadata for this user (creator)
        fileInput.addEventListener('change', (e)=> {
            const files = e.target.files;
            if (!files || files.length === 0) return;
            // allow multiple but create an item per file
            const user = JSON.parse(localStorage.getItem('sz_user') || 'null');
            const profile = JSON.parse(localStorage.getItem('sz_profile') || 'null') || {};
            const ownerName = profile && user ? (profile[user.email.split('@')[0]]?.nickname || user.email.split('@')[0]) : 'AnonCreator';

            const created = [];
            for (let i=0;i<files.length;i++){
                const f = files[i];
                // Create object URL so it can be played in overlay
                const url = URL.createObjectURL(f);
                const id = 'u_' + Math.random().toString(36).slice(2,9);
                // create DOM node
                const art = document.createElement('article');
                art.className = 'video-item';
                art.tabIndex = 0;
                art.dataset.id = id;
                art.dataset.title = f.name.replace(/\.[^/.]+$/, '');
                art.dataset.src = url;
                art.dataset.poster = ''; // no poster in demo
                art.dataset.channel = ownerName;
                art.dataset.description = 'Subido por ' + ownerName + ' (demo)';
                art.innerHTML = `<img class="video-thumbnail" src="placeholder-video1.jpg" alt="${escapeHtml(f.name)}" loading="lazy" /><div class="video-info"><h3>${escapeHtml(art.dataset.title)}</h3><p>Subido por ${escapeHtml(ownerName)}</p></div>`;
                // append to grid
                videosGrid.prepend(art);
                created.push({id: art.dataset.id, title: art.dataset.title, src: art.dataset.src, poster: art.dataset.poster, channel: art.dataset.channel});
            }

            // persist created list in localStorage keyed by user (demo)
            const userId = (user && user.email) ? user.email.split('@')[0] : 'anon';
            try {
                const key = uploadedVideosKeyForUser(userId);
                const prev = JSON.parse(localStorage.getItem(key) || '[]');
                const merged = prev.concat(created);
                localStorage.setItem(key, JSON.stringify(merged));
            } catch(e){}

            alert(`Has subido ${files.length} archivo(s). (demo, almacenado localmente)`);
            fileInput.value = '';
        });

        // Side menu demo buttons
        document.getElementById('side-subscribe').addEventListener('click', () => {
            openSubscribeModal();
            sideMenu.classList.remove('open'); sideOverlay.style.display='none';
        });
        document.getElementById('side-login').addEventListener('click', ()=> {
            openAuthModal();
            sideMenu.classList.remove('open'); sideOverlay.style.display='none';
        });

        // Make logout button actually log out and close menus
        const profileLogoutBtn = document.getElementById('profile-logout');
        profileLogoutBtn.addEventListener('click', () => {
            profileMenu.classList.remove('show');
            logout();
        });

        // Category pills click (filter emulation)
        document.querySelectorAll('.pill').forEach(p => {
            p.addEventListener('click', () => {
                document.getElementById('categorias').scrollIntoView({behavior:'smooth', block:'start'});
                document.querySelectorAll('.pill').forEach(x=> x.style.opacity=1);
                p.style.opacity = 1;
            });
        });

        // ----------------------------------------
        // Floating search: show when clicking magnifier
        // ----------------------------------------
        searchIcon.addEventListener('click', (e) => {
            const shown = floatingSearch.style.display === 'flex';
            if (shown) {
                closeFloatingSearch();
            } else {
                floatingSearch.style.display = 'flex';
                floatingSearch.setAttribute('aria-hidden','false');
                floatingSearchInput.focus();
            }
        });
        floatingSearchClose.addEventListener('click', closeFloatingSearch);
        function closeFloatingSearch(){
            floatingSearch.style.display = 'none';
            floatingSearch.setAttribute('aria-hidden','true');
        }
        // When pressing Enter in floating search, perform search
        floatingSearchInput.addEventListener('keydown', (e) => {
            if (e.key === 'Enter') {
                const v = floatingSearchInput.value.trim();
                closeFloatingSearch();
                performSearch(v);
            }
        });

        // Press Enter in main search input to search
        const mainSearchInput = document.getElementById('search-input');
        mainSearchInput.addEventListener('keydown', (e) => {
            if (e.key === 'Enter') {
                performSearch(mainSearchInput.value.trim());
            }
        });

        // Perform search across titles and descriptions (simple substring match, case-insensitive)
        function performSearch(q){
            const query = (q || '').trim().toLowerCase();
            const items = Array.from(document.querySelectorAll('.video-item'));
            const noResultsEl = document.getElementById('search-no-results');
            // reset highlights and visibility if empty query
            if (!query) {
                items.forEach(it => { it.style.display = ''; const h = it.querySelector('h3'); if (h) h.innerHTML = escapeHtml(h.textContent); });
                noResultsEl.style.display = 'none';
                return;
            }
            let any = false;
            items.forEach(it => {
                const title = (it.dataset.title || it.querySelector('h3')?.textContent || '').toLowerCase();
                const desc = (it.dataset.description || it.querySelector('.video-info p')?.textContent || '').toLowerCase();
                const channel = (it.dataset.channel || '').toLowerCase();
                const matched = title.includes(query) || desc.includes(query) || channel.includes(query);
                it.style.display = matched ? '' : 'none';
                if (matched) {
                    any = true;
                    // simple highlight in title
                    const h = it.querySelector('h3');
                    if (h) {
                        const raw = h.textContent;
                        const idx = raw.toLowerCase().indexOf(query);
                        if (idx !== -1) {
                            const before = escapeHtml(raw.slice(0, idx));
                            const match = escapeHtml(raw.slice(idx, idx+query.length));
                            const after = escapeHtml(raw.slice(idx+query.length));
                            h.innerHTML = `${before}<mark>${match}</mark>${after}`;
                        } else {
                            h.innerHTML = escapeHtml(raw);
                        }
                    }
                } else {
                    const h = it.querySelector('h3');
                    if (h) h.innerHTML = escapeHtml(h.textContent);
                }
            });
            if (!any) {
                noResultsEl.style.display = 'block';
            } else {
                noResultsEl.style.display = 'none';
            }
        }

        // ----------------------------------------
        // Liked videos modal behavior
        // ----------------------------------------
        function renderLikedModal(){
            const arr = getLikedVideos();
            likedList.innerHTML = '';
            if (!arr || arr.length === 0){
                likedList.innerHTML = `<div style="color:#bbb;padding:8px;">No hay videos que te hayan gustado aún.</div>`;
                return;
            }
            arr.forEach(v => {
                const el = document.createElement('div');
                el.className = 'liked-entry';
                el.innerHTML = `<img src="${escapeHtml(v.poster || '')}" alt="${escapeHtml(v.title)}"><div class="meta"><div style="font-weight:800;">${escapeHtml(v.title)}</div><div style="color:#ccc;font-size:0.9rem;">${escapeHtml(v.channel || '')}</div></div><div style="display:flex;flex-direction:column;gap:6px;"><button class="btn" data-id="${escapeHtml(v.id)}">Reproducir</button><button class="btn secondary" data-unlike="${escapeHtml(v.id)}">Eliminar</button></div>`;
                const playBtn = el.querySelector('button[data-id]');
                const unlikeBtn = el.querySelector('button[data-unlike]');
                playBtn.addEventListener('click', () => {
                    // attempt to find the original item and open it
                    const orig = Array.from(document.querySelectorAll('.video-item')).find(x => (x.dataset.id || x.dataset.title) === v.id);
                    if (orig) loadVideoToOverlay(orig);
                    else {
                        // create a temporary item-like object for playing
                        const temp = document.createElement('div');
                        temp.dataset.id = v.id;
                        temp.dataset.title = v.title;
                        temp.dataset.src = v.src || '';
                        temp.dataset.poster = v.poster || '';
                        temp.dataset.channel = v.channel || '';
                        loadVideoToOverlay(temp);
                    }
                    likedModal.style.display = 'none';
                });
                unlikeBtn.addEventListener('click', () => {
                    removeFromLiked(v.id);
                    // Also update per-video like state
                    try {
                        const lk = JSON.parse(localStorage.getItem(likesKey(v.id)) || '{"count":0,"liked":false}');
                        lk.liked = false;
                        localStorage.setItem(likesKey(v.id), JSON.stringify(lk));
                    } catch(e){}
                    renderLikedModal();
                });
                likedList.appendChild(el);
            });
        }
        likedBtnInMenu.addEventListener('click', () => {
            profileMenu.classList.remove('show');
            openLikedModal();
        });
        function openLikedModal(){
            renderLikedModal();
            likedModal.style.display = 'flex';
            likedModal.setAttribute('aria-hidden','false');
        }
        likedClose.addEventListener('click', () => { likedModal.style.display='none'; likedModal.setAttribute('aria-hidden','true'); });

        // ----------------------------------------
        // Authentication (Entrar / Crear cuenta) - simple client-side demo
        // ----------------------------------------
        function openAuthModal(){
            // default to login view
            showLogin();
            authModal.style.display = 'flex';
            authModal.setAttribute('aria-hidden','false');
        }
        function closeAuthModal(){
            authModal.style.display = 'none';
            authModal.setAttribute('aria-hidden','true');
        }
        sideLoginBtn.addEventListener('click', openAuthModal);
        showLoginBtn.addEventListener('click', showLogin);
        showRegisterBtn.addEventListener('click', showRegister);
        authClose.addEventListener('click', closeAuthModal);

        function showLogin(){
            loginForm.style.display = '';
            registerForm.style.display = 'none';
        }
        function showRegister(){
            loginForm.style.display = 'none';
            registerForm.style.display = '';
        }

        // Simple account storage: list of accounts stored in 'sz_accounts' (demo only)
        function getAccounts(){
            try { return JSON.parse(localStorage.getItem('sz_accounts') || '[]'); } catch(e){ return []; }
        }
        function saveAccounts(a){ try { localStorage.setItem('sz_accounts', JSON.stringify(a)); } catch(e){} }

        loginSubmit.addEventListener('click', () => {
            const email = (document.getElementById('login-email') || {}).value || '';
            const pass = (document.getElementById('login-pass') || {}).value || '';
            if (!email || !pass) { alert('Ingresa correo y contraseña.'); return; }
            const accounts = getAccounts();
            const acc = accounts.find(x => x.email === email && x.pass === pass);
            if (acc) {
                localStorage.setItem('sz_user', JSON.stringify({email: acc.email}));
                alert('Has iniciado sesión (demo).');
                closeAuthModal();
                refreshAccountUI();
            } else {
                alert('Credenciales incorrectas (demo).');
            }
        });

        regSubmit.addEventListener('click', () => {
            const email = (document.getElementById('reg-email') || {}).value || '';
            const pass = (document.getElementById('reg-pass') || {}).value || '';
            if (!email || !pass) { alert('Ingresa correo y contraseña.'); return; }
            const accounts = getAccounts();
            if (accounts.find(x => x.email === email)) { alert('Ya existe una cuenta con ese correo (demo).'); return; }
            accounts.push({email, pass});
            saveAccounts(accounts);
            localStorage.setItem('sz_user', JSON.stringify({email}));
            alert('Cuenta creada e iniciada (demo).');
            closeAuthModal();
            refreshAccountUI();
        });

        function logout(){
            try { localStorage.removeItem('sz_user'); } catch(e){}
            alert('Has cerrado sesión (demo).');
            refreshAccountUI();
        }

        // Update profile menu & side-login text based on current user
        function refreshAccountUI(){
            const u = JSON.parse(localStorage.getItem('sz_user') || 'null');
            // If logged in, display email on profile menu and adjust side button
            const existingEmailEl = profileMenu.querySelector('.profile-email');
            if (u && u.email){
                if (!existingEmailEl){
                    const span = document.createElement('div');
                    span.className = 'profile-email';
                    span.textContent = u.email;
                    profileMenu.insertBefore(span, profileMenu.firstChild);
                } else {
                    existingEmailEl.textContent = u.email;
                }
                sideLoginBtn.textContent = 'Cuenta: ' + u.email.split('@')[0];
            } else {
                if (existingEmailEl) existingEmailEl.remove();
                sideLoginBtn.textContent = 'Entrar / Crear cuenta';
            }
        }
        // run initial refresh
        refreshAccountUI();

        // ----------------------------------------
        // Account modal wiring
        // ----------------------------------------
        const profileAccountBtn = document.getElementById('profile-account');
        profileAccountBtn.addEventListener('click', () => {
            profileMenu.classList.remove('show');
            openAccountModal();
        });

        function openAccountModal(){
            const user = JSON.parse(localStorage.getItem('sz_user') || 'null');
            if (!user) {
                // encourage login
                if (confirm('Debes iniciar sesión para editar tu cuenta. ¿Deseas iniciar sesión ahora?')) {
                    openAuthModal();
                }
                return;
            }
            // load profile for this user
            const uid = user.email.split('@')[0];
            let profile = {};
            try { profile = JSON.parse(localStorage.getItem('sz_profile') || '{}'); } catch(e){ profile = {}; }
            const perUser = (profile && profile[uid]) ? profile[uid] : (profile || {});
            acctNickname.value = perUser.nickname || uid;
            acctIsCreator.checked = !!perUser.isCreator;
            creatorTools.style.display = acctIsCreator.checked ? '' : 'none';
            accountModal.style.display = 'flex';
            accountModal.setAttribute('aria-hidden','false');
        }

        acctCancel.addEventListener('click', () => {
            accountModal.style.display = 'none';
            accountModal.setAttribute('aria-hidden','true');
        });

        acctIsCreator.addEventListener('change', () => {
            creatorTools.style.display = acctIsCreator.checked ? '' : 'none';
        });

        acctSave.addEventListener('click', () => {
            const user = JSON.parse(localStorage.getItem('sz_user') || 'null');
            if (!user) { alert('Debes iniciar sesión.'); return; }
            const uid = user.email.split('@')[0];
            // load saved profile object (allow multi-user)
            let profileObj = {};
            try { profileObj = JSON.parse(localStorage.getItem('sz_profile') || '{}'); } catch(e){ profileObj = {}; }
            const target = profileObj[uid] || {};
            // nickname
            const newNick = (acctNickname.value || '').trim();
            if (newNick) target.nickname = newNick;

            // password change if requested
            const cur = (acctCurrentPass.value || '').trim();
            const np = (acctNewPass.value || '').trim();
            const npc = (acctNewPassConfirm.value || '').trim();
            if (np || npc) {
                if (!cur) { alert('Ingresa tu contraseña actual para cambiarla.'); return; }
                if (np !== npc) { alert('La nueva contraseña y la confirmación no coinciden.'); return; }
                // validate against accounts
                const accounts = getAccounts();
                const accIdx = accounts.findIndex(a => a.email === user.email && a.pass === cur);
                if (accIdx === -1) { alert('Contraseña actual incorrecta (demo).'); return; }
                accounts[accIdx].pass = np;
                saveAccounts(accounts);
                alert('Contraseña actualizada (demo).');
            }

            // creator toggle
            target.isCreator = !!acctIsCreator.checked;

            // persist
            profileObj[uid] = target;
            try { localStorage.setItem('sz_profile', JSON.stringify(profileObj)); } catch(e){}
            alert('Perfil actualizado (demo).');
            // clear password fields
            acctCurrentPass.value = '';
            acctNewPass.value = '';
            acctNewPassConfirm.value = '';
            accountModal.style.display = 'none';
            accountModal.setAttribute('aria-hidden','true');
            refreshAccountUI();
        });

        // Creator tools: wire to upload and to manage user's uploaded videos
        creatorUpload.addEventListener('click', () => {
            accountModal.style.display = 'none';
            uploadModal.style.display = 'flex';
            document.getElementById('upload-from-device').focus();
        });

        creatorManage.addEventListener('click', () => {
            // open a simple list of user's uploaded videos using the channel modal for convenience
            const user = JSON.parse(localStorage.getItem('sz_user') || 'null');
            if (!user) { alert('Debes iniciar sesión.'); return; }
            const uid = user.email.split('@')[0];
            const profileObj = JSON.parse(localStorage.getItem('sz_profile') || '{}') || {};
            const nickname = (profileObj[uid] && profileObj[uid].nickname) ? profileObj[uid].nickname : uid;
            accountModal.style.display = 'none';
            openChannelModal(nickname);
        });

        // ----------------------------------------
        // Channel modal: show videos uploaded by channel and followers/seguidos
        // ----------------------------------------
        function openChannelModal(channelName){
            if (!channelName) return;
            channelModal.style.display = 'flex';
            channelModal.setAttribute('aria-hidden','false');

            chTitle.textContent = 'Canal: ' + channelName;
            chNameEl.textContent = channelName;

            // gather videos by channel
            const vids = Array.from(document.querySelectorAll('.video-item')).filter(x => (x.dataset.channel || '') === channelName).map(x => {
                return {
                    id: x.dataset.id || x.dataset.title || ('tmp_' + Math.random().toString(36).slice(2,6)),
                    title: x.dataset.title || x.querySelector('h3')?.textContent || 'Video',
                    poster: x.dataset.poster || x.querySelector('img')?.src || '',
                    src: x.dataset.src || ''
                };
            });

            chVideosCount.textContent = `${vids.length} videos`;
            // seguidos: channels this channel follows (for demo keep a number stored)
            let following = [];
            try { following = JSON.parse(localStorage.getItem(channelFollowingKey(channelName)) || '[]'); } catch(e){ following = []; }
            let followers = [];
            try { followers = JSON.parse(localStorage.getItem(channelFollowersKey(channelName)) || '[]'); } catch(e){ followers = []; }

            chFollowingCount.textContent = `${following.length} seguidos`;
            chFollowersCount.textContent = `${followers.length} seguidores`;

            // render videos
            chVideosContainer.innerHTML = '';
            if (vids.length === 0) {
                chVideosContainer.innerHTML = `<div style="color:#bbb;padding:8px;">Este canal aún no ha subido videos.</div>`;
            } else {
                vids.forEach(v => {
                    const entry = document.createElement('div');
                    entry.className = 'liked-entry';
                    entry.innerHTML = `<img src="${escapeHtml(v.poster)}" alt="${escapeHtml(v.title)}"><div class="meta"><div style="font-weight:800;">${escapeHtml(v.title)}</div></div><div style="display:flex;flex-direction:column;gap:6px;"><button class="btn" data-play="${escapeHtml(v.id)}">Reproducir</button></div>`;
                    entry.querySelector('button[data-play]').addEventListener('click', () => {
                        // find original element to play
                        const orig = Array.from(document.querySelectorAll('.video-item')).find(x => (x.dataset.id || x.dataset.title) === v.id);
                        if (orig) loadVideoToOverlay(orig);
                        else {
                            const temp = document.createElement('div');
                            temp.dataset.id = v.id;
                            temp.dataset.title = v.title;
                            temp.dataset.src = v.src || '';
                            temp.dataset.poster = v.poster || '';
                            temp.dataset.channel = channelName;
                            loadVideoToOverlay(temp);
                        }
                        channelModal.style.display = 'none';
                    });
                    chVideosContainer.appendChild(entry);
                });
            }

            // follow/unfollow toggle: current user follows channel?
            const user = JSON.parse(localStorage.getItem('sz_user') || 'null');
            const userId = user?.email || 'anon';
            if (followers.includes(userId)){
                chFollowBtn.textContent = 'Dejar de seguir';
                chFollowBtn.style.background = '#222';
            } else {
                chFollowBtn.textContent = 'Seguir';
                chFollowBtn.style.background = '';
            }

            // wire follow button
            chFollowBtn.onclick = () => {
                let f = [];
                try { f = JSON.parse(localStorage.getItem(channelFollowersKey(channelName)) || '[]'); } catch(e){ f = []; }
                if (!f.includes(userId)){
                    f.push(userId);
                    localStorage.setItem(channelFollowersKey(channelName), JSON.stringify(f));
                    chFollowersCount.textContent = `${f.length} seguidores`;
                    chFollowBtn.textContent = 'Dejar de seguir';
                } else {
                    f = f.filter(x => x !== userId);
                    localStorage.setItem(channelFollowersKey(channelName), JSON.stringify(f));
                    chFollowersCount.textContent = `${f.length} seguidores`;
                    chFollowBtn.textContent = 'Seguir';
                }
            };

            chCloseBtn.onclick = () => { channelModal.style.display='none'; channelModal.setAttribute('aria-hidden','true'); };
        }

        // ----------------------------------------
        // Subscription modal: simplified (no payment fields)
        // ----------------------------------------
        const SUB_PRICE = 8.05;
        const modalBackdrop = document.getElementById('modal-backdrop');
        const modalContent = document.getElementById('modal-content');

        function openSubscribeModal(){
            const html = `
                <h3 id="modal-title">Suscribirse a SexZone Premium</h3>
                <div style="color:#ccc;margin-bottom:8px;">Precio: <strong>$${SUB_PRICE.toFixed(2)}</strong> / mes. Pago recurrente. (Demo)</div>

                <div class="form-row" style="margin-bottom:8px;">
                    <label for="sub-email">Correo electrónico</label>
                    <input id="sub-email" type="email" placeholder="correo@ejemplo.com" style="width:100%;padding:8px;border-radius:8px;background:#060606;border:1px solid rgba(255,255,255,0.03);color:#fff;" />
                </div>

                <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:12px;">
                    <button class="btn" id="btn-pay">Suscribirme (demo)</button>
                    <button class="btn secondary" id="btn-cancel">Cancelar</button>
                </div>

                <div style="margin-top:10px;color:#999;font-size:0.85rem;">
                    AVISO: Esto es una demo cliente-lado. En producción integra un gateway real y procesa pagos en servidor.
                </div>
            `;
            modalContent.innerHTML = html;
            modalBackdrop.style.display = 'flex';
            modalBackdrop.setAttribute('aria-hidden','false');

            modalBackdrop.querySelector('#btn-cancel').addEventListener('click', closeModalBackdrop);
            modalBackdrop.querySelector('#btn-pay').addEventListener('click', handleSubscriptionPaymentSimple);
        }

        function closeModalBackdrop(){
            modalBackdrop.style.display = 'none';
            modalBackdrop.setAttribute('aria-hidden','true');
            modalContent.innerHTML = '';
        }

        function handleSubscriptionPaymentSimple(){
            const email = (modalBackdrop.querySelector('#sub-email') || {}).value || '';
            if (!email || !/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email)) { alert('Por favor ingresa un correo válido.'); modalBackdrop.querySelector('#sub-email').focus(); return; }
            const btn = modalBackdrop.querySelector('#btn-pay');
            btn.textContent = 'Procesando...';
            btn.disabled = true;
            setTimeout(() => {
                finishSubscription(email, 'demo');
            }, 900);
        }

        function finishSubscription(email, method){
            const now = new Date();
            const next = new Date(now.getTime()); next.setMonth(next.getMonth()+1);
            const subscription = {
                email,
                method,
                price: SUB_PRICE,
                start: now.toISOString(),
                expires: next.toISOString(),
                status:'active',
                id: 'sub_' + Math.random().toString(36).slice(2,9)
            };
            try { localStorage.setItem('sz_subscription', JSON.stringify(subscription)); } catch(e){}
            alert('¡Suscripción (demo) activada!');
            closeModalBackdrop();
            refreshAccountUI && refreshAccountUI();
        }

        // Modal close on backdrop click
        modalBackdrop.addEventListener('click', (e) => { if (e.target === modalBackdrop) closeModalBackdrop(); });

        // Helpers
        function escapeHtml(s){ return String(s).replace(/[&<>"']/g, function(m){ return ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":"&#39;"})[m]; }); }

        // Close overlays on Escape
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                if (profileMenu.classList.contains('show')) { profileMenu.classList.remove('show'); profileBtn.setAttribute('aria-expanded','false'); }
                if (sideMenu.classList.contains('open')) { sideMenu.classList.remove('open'); sideOverlay.style.display='none'; menuToggle.setAttribute('aria-expanded','false'); }
                if (videoOverlay.style.display === 'flex') closeVideoOverlay();
                if (modalBackdrop.style.display === 'flex') closeModalBackdrop();
                if (uploadModal.style.display === 'flex') uploadModal.style.display = 'none';
                if (likedModal.style.display === 'flex') { likedModal.style.display = 'none'; likedModal.setAttribute('aria-hidden','true'); }
                if (authModal.style.display === 'flex') { authModal.style.display = 'none'; authModal.setAttribute('aria-hidden','true'); }
                if (channelModal.style.display === 'flex') { channelModal.style.display = 'none'; channelModal.setAttribute('aria-hidden','true'); }
                if (floatingSearch.style.display === 'flex') closeFloatingSearch();
                if (accountModal.style.display === 'flex') { accountModal.style.display = 'none'; accountModal.setAttribute('aria-hidden','true'); }
            }
        });

        // Minimal initialization for recommended list empty state
        recommendedList.innerHTML = '';

        // Close liked modal on backdrop click
        likedModal.addEventListener('click', (e) => { if (e.target === likedModal) { likedModal.style.display='none'; likedModal.setAttribute('aria-hidden','true'); } });

        // Close auth modal on backdrop click
        authModal.addEventListener('click', (e) => { if (e.target === authModal) { authModal.style.display='none'; authModal.setAttribute('aria-hidden','true'); } });

        // Close account modal on backdrop click
        accountModal.addEventListener('click', (e) => { if (e.target === accountModal) { accountModal.style.display='none'; accountModal.setAttribute('aria-hidden','true'); } });

        // Close channel modal on backdrop click
        channelModal.addEventListener('click', (e) => { if (e.target === channelModal) { channelModal.style.display='none'; channelModal.setAttribute('aria-hidden','true'); } });

    </script>
</body>
</html>
