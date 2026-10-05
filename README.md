<!-- tyhp-readme:start -->
# tyhpdef/hashids-hashids

Tyhp type definitions for `hashids/hashids` `5.0.2`.

```bash
composer require --dev tyhpdef/hashids-hashids:5.0.2
```

This is a metapackage. Composer also installs `tyhpdef/hashids-hashids-impl` (type files).
Require **this** name, not `tyhpdef/hashids-hashids-impl`.

See https://tyhplang.com.

## Maintain `hashids/hashids`? Ship the types yourself

If you are a Packagist maintainer of `hashids/hashids`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/hashids-hashids-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `hashids/hashids` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/hashids-hashids": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `hashids/hashids` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `hashids/hashids` with a real constraint,
   `"replace": { "tyhpdef/hashids-hashids": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `hashids/hashids` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/hashids-hashids` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
