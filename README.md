<!-- tyhp-readme:start -->
# tyhpdef/symfony-form

Tyhp type definitions for `symfony/form` `7.4.19`.

```bash
composer require --dev tyhpdef/symfony-form:7.4.19
```

This is a metapackage. Composer also installs `tyhpdef/symfony-form-impl` (type files).
Require **this** name, not `tyhpdef/symfony-form-impl`.

See https://tyhplang.com.

## Maintain `symfony/form`? Ship the types yourself

If you are a Packagist maintainer of `symfony/form`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-form-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/form` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-form": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/form` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/form` with a real constraint,
   `"replace": { "tyhpdef/symfony-form": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/form` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-form` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
