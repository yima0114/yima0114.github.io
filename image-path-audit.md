# Image Path Audit

Audit date: June 15, 2026

Project root: `G:\Yi_Artist_Site_v01`

## Summary

- Audited `index.html`, `works.html`, `research.html`, `cv.html`, `contact.html`, and `style.css`.
- Found 28 HTML image references in total.
- Found 9 image-reference occurrences whose code did not literally match the local path because spaces were written as `%20`.
- Found 19 image references that already matched the local filenames, extensions, letter case, and folders exactly.
- Found no CSS image references.
- `research.html`, `cv.html`, and `contact.html` contain no image references.
- No case differences, file-extension differences, or wrong folder names were found.
- The project root has no `.git` directory, so this local audit cannot confirm whether the image files were uploaded to the GitHub repository.

## Broken Or Non-Exact References

The entries below used URL-encoded spaces. `%20` is normally valid in a URL, but the paths were changed to literal spaces so the HTML strings now exactly match the real local filenames and folders.

| HTML file | Current path in code | Closest matching real file path | Issue |
| --- | --- | --- | --- |
| `index.html` | `images/01-oil-painting-scarf/01-13-2025%2072dpi/01%20%2010.8MB%20%2072dpi.JPG` | `images/01-oil-painting-scarf/01-13-2025 72dpi/01  10.8MB  72dpi.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/01-13-2025%2072dpi/01%20%2010.8MB%20%2072dpi.JPG` | `images/01-oil-painting-scarf/01-13-2025 72dpi/01  10.8MB  72dpi.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/01-13-2025%2072dpi/02%20%2010.8MB%20%2072dpi.JPG` | `images/01-oil-painting-scarf/01-13-2025 72dpi/02  10.8MB  72dpi.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/11-30-2022%2072%20dpi/283A0030%20copy.JPG` | `images/01-oil-painting-scarf/11-30-2022 72 dpi/283A0030 copy.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/11-30-2022%2072%20dpi/283A0041%20copy.JPG` | `images/01-oil-painting-scarf/11-30-2022 72 dpi/283A0041 copy.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/11-30-2022%2072%20dpi/283A0061%20copy.JPG` | `images/01-oil-painting-scarf/11-30-2022 72 dpi/283A0061 copy.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/11-30-2022%2072%20dpi/283A0098%20copy.JPG` | `images/01-oil-painting-scarf/11-30-2022 72 dpi/283A0098 copy.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/4-22-2022%20%2010.8MB%20%2072dpi/03%20copy.JPG` | `images/01-oil-painting-scarf/4-22-2022  10.8MB  72dpi/03 copy.JPG` | Spaces |
| `works.html` | `images/01-oil-painting-scarf/4-22-2022%20%2010.8MB%20%2072dpi/07%20copy.JPG` | `images/01-oil-painting-scarf/4-22-2022  10.8MB  72dpi/07 copy.JPG` | Spaces |

## Upload Note

All 19 metalwork and color-study image references exactly match real local files. If those images still show as broken after the corrected HTML is published, the likely issue is a missing upload rather than an HTML path mismatch. Confirm that the complete `images` folder, including all three subfolders and the nested painting folders, exists in the GitHub repository.
