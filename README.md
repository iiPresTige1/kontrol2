# KONTROL GoldHEN UI / Cache Fixed Package

This package fixes the KONTROL frontend packaging only:

- adds a valid `manifest.appcache`;
- links the manifest from `index.html`;
- removes the automatic redirect to `cache.html`;
- keeps all asset paths relative;
- keeps `bundle.js` and `payload.bin` byte-for-byte unchanged.

The files `alert.mjs`, `psfree.mjs`, and `payload.js` from the supplied archive were HTML fallback pages rather than JavaScript and were intentionally not included. They were not referenced by the current `index.html`/`bundle.js` path.

This is not a rebuilt exploit or a guarantee of payload compatibility. Test only on hardware you own, with the source and firmware compatibility independently verified.
