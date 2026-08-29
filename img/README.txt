QIZU website images
===================

shot-*.webp    Screenshots taken on an Android emulator at 1440x3200 /
               density 560 and exported at 1080x2400 — twice the 540x1200 slot
               index.html gives each <img>, so they stay sharp on HiDPI. Not
               made here: the app repo's store/build_screenshots.py writes them
               with `python store/build_screenshots.py --site <this folder>`,
               from the same raw frames the Play screenshots use, so the site
               and the store listing can never drift apart.

               The demo library they show is built by
               integration_test/seed_demo_test.dart in the app repo — run it
               armed (--dart-define=QIZU_SEED_DEMO=true) against a throwaway
               account. Re-captured 2026-08-29 on 1.1.0+16 with QIZU+ active.

               No hand-retouching any more: the AVD now runs hw.keyboard=no, so
               shot-type.webp shows the real soft keyboard instead of the
               floating toolbar that used to be painted out, and the composer
               itself blanks the one status-bar slot where the emulator's
               ethernet glyph flickers between frames.

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

buddy.webp     assets/illustrations/test_buddy_2.webp (1500x1000), cropped to
               the art's bounds and resized to 440x310 — the companion drawn
               inside the hand-built hero phone. Keep the aspect ratio when
               regenerating: an earlier square resize stretched the mascot.

og.png         Rendered natively at 1200x630 by the app repo's
               tool/generate_feature_graphic.ps1 (same answer-line design as
               the Play feature graphic, not a rescale of it). Link preview
               image only; no page loads it.

Sources live in the app repo (Flutter-PROJECTS/qizu). Nothing here is generated
at request time — the site is fully static.
