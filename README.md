# Card

A site theme for [Modulento](https://github.com/alex01at/modulento): a
clean, trustworthy SaaS look - a light grey ground, dark slate ink, a
confident blue accent, modest rounded shapes. Built for the [card
extension](https://github.com/alex01at/modulento-ext-card) (a digital
business card per account), but works with any Modulento installation.

It brings a layout, a home page (a hero, an editable feature list, a
"already on board" list of recent providers, and a closing call to
action), card partials for the provider directory, and a stylesheet.
System fonts only - no font file to vendor or license. Every other page
comes from Modulento's `default` theme and only looks different.

**Not part of this theme**: the four card designs themselves (classic,
modern, professional, playful) - those belong to the card extension and
apply to the public `/card/{slug}` page, which renders full-page, without
any site theme around it. This theme covers the marketing and account
side: the home page, the header/footer, the pricing page, the provider
directory.

Like the rest of the home page, every block is edited in place
(**Administration → Home page**, or directly on the page itself when
signed in with that permission): click into a heading or text to change
it, add pictures, reorder or remove blocks, or add a new one. Nothing
about this theme changes how that editor works - it only draws the blocks
differently.

The theme has a dark scheme. It follows the device, unless an account has
chosen "light" or "dark" in its settings. Every colour in `assets/theme.css`
is a variable; the dark values are in the two blocks below `:root`.

A logo uploaded under **Administration → Themes → Branding** replaces the
decorative mark and the site's name in the header and footer; a separate
logo for the dark scheme, where there is one, is swapped in by CSS. A
favicon and the description set under **Administration → Settings** are
linked and tagged (including Open Graph and Twitter tags) without any
further setup.

## Installing

In Modulento, open **Administration → Packages**, enter
`alex01at/modulento-theme-card` and install. Then choose "Card" under
**Administration → Themes**. New versions appear on the Packages page.

By hand: unpack a release into `themes/card/` of the installation.

## Changing the colours

Everything in `assets/theme.css` is a CSS custom property on `:root`
(light) and repeated with dark values below it. The accent is `#1d4dd8`;
changing `--accent`/`--accent-dark`/`--accent-text`/`--accent-strong`/
`--accent-soft`/`--accent-line` together covers it everywhere a button,
link or highlight uses it.
