
+ 0.4.2 [Feb ? 2013]

  - helpers are now included via `helper` method - [#ab2063461](https://github.com/espresso/espresso/commit/ab2063461)
  - `link_to` helper [#db51c839](https://github.com/espresso/espresso/commit/db51c839cf2e1165bceb5d394b3706e53c59f0b4)
  - make index action to serve /index URL [#fb763c64](https://github.com/espresso/espresso/commit/fb763c644092577627321a0d672e3cc060f9c9cf)
  - Added `reject_automount!` for controllers that should not be mounted at automount [f5ce4723a](https://github.com/espresso/espresso/commit/f5ce4723a)
  - Fixed RDoc generation on Ruby 2.0.0 - [0ad4bbe951](https://github.com/espresso/espresso/commit/0ad4bbe951)
  - trap INT and TERM signals to gracefully stop web server - [#fcbebf974](https://github.com/espresso/espresso/commit/fcbebf9740a49065b31ad8d65dcc0d31cf80247b)

<hr>

+ 0.4.1 [Feb 18 2013]

  - support for various streaming backends - [#bd844acf](https://github.com/espresso/espresso/commit/bd844acf)
  - added transfer_encoding setup - [#e6f4805f4](https://github.com/espresso/espresso/commit/e6f4805f478050df9a7a1206e7ed8ae9b94da039)

<hr>

+ 0.4.0 [Feb 11 2013] - First Stable Release

  - Created a handy generator to easily generate projects, controllers, routes etc.
  - Path to templates are now resolved by controller name, not by base URL
  - Verbified actions has priority over verbless ones, regardless defining order
  - Removing Appetite dependency
  - Writing a new router crafted for specific Espresso needs. Also it tends to be faster than Rack::URLMap
  - Rewrite rules can now be defined inside controllers
  - Splitting codebase into `e-core` and `e-more`
  - Moved monkey-patches to e-ext
  - `format` now accepts only formats, not action names.
  - Added `format_for` to define formats for specific action.
  - Added `disable_format_for` to disable formats for specific action.
  - Sprockets support
  - `assets_loader` renamed to `assets_mapper`
  - Added tag helpers like `js_tag`, `css_tag`, `png_tag` etc.
  - Slim engine are now automatically registered without errors
  - Dropped support for inter-controller rendering
  - Added `render_file` method
  - Fixed Crudifier to work well with ActiveRecord models
  - `route` are now RESTful friendly
  - Allow to include actions from modules
  - Accept multiple controllers at mount
  - `invoke` and `fetch` will NOT pass actual params. Only `pass` will do.
  - Considerable code cleanup and refactoring. Special thanks to @mindreframer.
