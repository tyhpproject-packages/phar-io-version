<!-- tyhp-readme:start -->
# tyhpdef/phar-io-version

Tyhp type definitions for `phar-io/version` `3.2.1`.

```bash
composer require --dev tyhpdef/phar-io-version:3.2.1
```

This is a metapackage. Composer also installs `tyhpdef/phar-io-version-impl` (type files).
Require **this** name, not `tyhpdef/phar-io-version-impl`.

See https://tyhplang.com.

## Maintain `phar-io/version`? Ship the types yourself

If you are a Packagist maintainer of `phar-io/version`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phar-io-version-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phar-io/version` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phar-io-version": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phar-io/version` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phar-io/version` with a real constraint,
   `"replace": { "tyhpdef/phar-io-version": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phar-io/version` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phar-io-version` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
