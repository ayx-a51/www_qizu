QIZU website images
===================

shot-*.webp    Screenshots taken on an Android emulator (1080x2400), scaled to
               half size. The demo library they show is built by
               integration_test/seed_demo_test.dart in the app repo — run it
               armed (--dart-define=QIZU_SEED_DEMO=true) against a throwaway
               account, then reinstall the app and sign in again.
               shot-type.webp has the emulator's floating keyboard toolbar
               painted out: on a real phone the keyboard fills that area.

qizu-mark.png  The current launcher icon (assets/icon/icon_512.png) at 192px —
               the header and footer mark on every page. favicon.ico and
               apple-touch-icon.png in the site root come from the same
               pipeline (app repo tool/generate_icon.ps1 → assets/icon/web/);
               copy them over whenever the icon changes. Since 2026-08-28 the
               icon is the "answer line" mark (check + yellow line + mint
               sparkle/period on deep magenta), not the smiley card.

flame-0..7     The D31 streak-flame colourways, in tier order (day 1 / 7 / 14 /
               30 / 90 / 180 / 365 / 730), from the app's own
               assets/illustrations/streak_flame*.webp, resized to 176px.

buddy.webp     assets/illustrations/test_buddy_2.webp, resized to 300px — the
               companion drawn inside the hand-built hero phone.

og.png         store/feature_graphic.png, scaled to 1200x630 and quantised.
               Link preview image only; no page loads it.

Sources live in the app repo (Flutter-PROJECTS/qizu). Nothing here is generated
at request time — the site is fully static.
