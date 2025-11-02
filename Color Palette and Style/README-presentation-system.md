# Gospel Doctrine Presentation System
**Pantone Color Palette & Reusable Styles**

## Quick Start

### For New Lessons:
1. Copy `lesson-template.html` and rename it (e.g., `dc-125-lesson.html`)
2. Make sure `gospel-doctrine-styles.css` is in the same folder
3. Edit the HTML content but keep the class names
4. Open the HTML file in any browser to present

### File Structure:
```
your-lessons-folder/
├── gospel-doctrine-styles.css    (Your color palette & styles)
├── lesson-template.html           (Template for new lessons)
├── dc-124-temple-presentation.html (Example completed lesson)
└── images/                        (Folder for lesson images)
```

## Color Palette Reference

Your Pantone colors are saved as CSS variables:

| Color Name    | Hex Code | CSS Variable        | Used For                    |
|---------------|----------|---------------------|-----------------------------|
| Tendril       | #89A06B  | `--tendril`         | Secondary/green accents     |
| Cornflower    | #7391C8  | `--cornflower`      | Primary brand color         |
| Viola         | #A692BA  | `--viola`           | Accent/purple tones         |
| Rose Tan      | #D19C97  | `--rose-tan`        | Question boxes              |
| Mocha Mousse  | #A47864  | `--mocha-mousse`    | Warm accents, quotes        |
| Cobblestone   | #A89A8E  | `--cobblestone`     | Content boxes               |
| Willow        | #9A8B4F  | `--willow`          | Quotes, earth tones         |
| Gardenia      | #F1E9DF  | `--gardenia`        | Background                  |

## Available CSS Classes

### Slide Types:
- `class="title-slide"` - Blue gradient title slides
- `class="principle-slide"` - Purple gradient principle headers
- Regular sections - Gardenia background

### Content Boxes:
- `class="scripture-box"` - Blue gradient for scriptures
- `class="question-box"` - Rose Tan gradient for discussion
- `class="content-box"` - Cobblestone gradient for lists
- `class="video-container"` - For video links

### Text Elements:
- `<span class="scripture-ref">` - Scripture references (white, bold)
- `<p class="invitation">` - "Let's Read:" prompts
- `<strong>` - White, bold, sans-serif emphasis
- `<em>` - Accent purple italics
- `<blockquote>` - Willow/Mocha gradient quotes
- `<small>` - Smaller secondary text

### Reveal.js Features:
- `class="fragment"` - Makes items appear one at a time
- `class="center-content"` - Centers content vertically

## Typography Sizes (for 60+ audience)

- **H1 (Title)**: 68-72px
- **H2 (Principles)**: 54-64px  
- **H3 (Subtitles)**: 44-48px
- **Body text**: 38-42px
- **Small text**: 28-32px

## How to Update the Website

To match your website's color palette, use the same CSS variables in your website's stylesheet:

```css
:root {
  --tendril: #89A06B;
  --cornflower: #7391C8;
  --viola: #A692BA;
  --rose-tan: #D19C97;
  --mocha-mousse: #A47864;
  --cobblestone: #A89A8E;
  --willow: #9A8B4F;
  --gardenia: #F1E9DF;
}
```

Then reference these variables throughout your website CSS just like in the presentations!

## Keyboard Shortcuts (During Presentation)

- **Arrow keys** - Navigate slides
- **F** - Fullscreen mode
- **B** - Blank screen (black)
- **Esc** - Overview mode (see all slides)
- **S** - Speaker notes (if added)
- **?** - Help menu

## Tips for Creating New Lessons

1. **Start with the template** - Don't start from scratch
2. **Use fragments** - Add `class="fragment"` to reveal content progressively
3. **Keep text large** - Minimum 32px for readability
4. **Limit bullet points** - 3-4 maximum per slide
5. **Balance boxes** - Don't use all three box types on one slide
6. **Add images** - Use the placeholder comments to note where images go
7. **Test beforehand** - Open in browser and click through before class

## Image Placeholder Format

When you want to add an image later, use this format in an HTML comment:

```html
<!-- IMAGE PLACEHOLDER: Description of image
     Location: images/filename.jpg
     Search Terms: "terms to search on churchofjesuschrist.org or Google"
     AI Prompt: "Detailed prompt for AI image generation"
     Recommended size: 1920x1080 or 1200x800 -->
```

## Customizing Colors

If you want to change colors in the future, edit `gospel-doctrine-styles.css`:

1. Find the `:root` section at the top
2. Change the hex codes for any colors
3. Save the file
4. All presentations using this stylesheet will automatically update!

## Getting Help

When asking Claude for help with future lessons, say:
"Use my gospel doctrine presentation styles from gospel-doctrine-styles.css"

Or simply:
"Create a new presentation using my Pantone color palette"

---

**Created:** November 2025  
**Version:** 1.0  
**Color Palette:** Custom Pantone Harmony
