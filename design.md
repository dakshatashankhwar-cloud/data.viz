# Editorial Design Notes

## Direction

The page uses a quiet print-editorial direction: warm paper, near-black ink, one rust accent, and oversized serif display type. The intentionally sparse composition gives the content room to feel like a small independent magazine or visual index.

## Layout

- The page is framed by generous responsive margins, like a printed spread.
- The title acts as the masthead and anchors the first viewport.
- The navigation is a compact, uppercase index separated by rules.
- The photo section uses an asymmetric two-column composition on larger screens and collapses to a single column on mobile.
- Rules and numbered details create rhythm without adding decorative panels.

## Typography

Display headings use an available old-style serif stack (`Iowan Old Style`, `Baskerville`, and `Times New Roman`) for a literary voice. Navigation uses a compact sans-serif stack for contrast, utility, and scanability.

## Color

- `--paper`: warm off-white page surface
- `--ink`: dark green-black text and rules
- `--muted`: secondary navigation text
- `--accent`: rust red for small points of emphasis

The subtle dot texture is created with CSS so the background feels tactile without requiring an image asset.

## Responsive behavior

The title and heading scale with `clamp()`. The navigation wraps naturally, and the photo section changes from a two-column editorial spread to a stacked mobile layout below `680px`.

## Accessibility and resilience

The stylesheet includes a box-sizing reset, responsive media defaults, visible text contrast, and a selection state. Images are constrained to their containers and retain a neutral background when an asset is missing. The HTML should still be updated with a meaningful page title, alt text for every image, and valid relative asset paths before publishing.