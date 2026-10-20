# Octavo

Octavo is the official theme of the [`umono/page@v0.1`](https://umono.dev/registry/v1/contracts/umono/page/v0.1) contract for [Umono](https://github.com/umono-cms/umono). It is modern and plain: a white page, a neutral sans serif, one column for the content, and a header and footer that span the page.

| | |
| --- | --- |
| Theme ID | `umono/octavo` |
| Contract | `umono/page@v0.1` (the `page` layout) |
| Requires | Umono v0.9 or later |
| License | MIT, with the Inter font under the SIL Open Font License 1.1 ([LICENSE](LICENSE)) |

## Install

Download the `.umono-theme` file from the [latest release](https://github.com/umono-cms/theme-octavo/releases/latest) and install it in your Umono project:

```sh
umono theme install umono_octavo_0.1.0.umono-theme
```

Then activate it in the admin panel under **Settings → Themes**, and bind your pages to the `page` layout of `umono/page v0.1`.

## Design

- **Type.** Text is set in [Inter](https://github.com/rsms/inter), a variable sans serif with optical sizes. The Latin and Latin Extended subsets are included, in `assets/fonts/`. Code is set in the system's monospace font.
- **Page.** Body text is 16px on small screens and 17px from 48rem up, with a line height of 1.7, in a column of 42rem. The header and footer span the page and align their content with the column.
- **Colors and sizes** are custom properties on the root in `assets/theme.css` (`--surface`, `--text`, `--accent`, `--column` and the rest).
- **Menu.** Submenus open on hover and on keyboard focus where the pointer can hover. On touch screens they are shown under their item.
- **Direction.** The theme uses logical properties and works in right-to-left languages.

`attributes.toml` sets `sizes` on the images of the `page` layout.

## Development

```sh
umono theme dev     # live development at http://localhost:8990
umono theme build   # checks the theme and writes dist/umono_octavo_<version>.umono-theme
```

See the [Umono CLI](https://github.com/umono-cms/cli) for the details of `dev` and `build`.
