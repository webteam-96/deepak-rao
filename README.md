# Deepak Rao ESP — website redesign

Redesign of [deepakrao-esp.com](https://www.deepakrao-esp.com/): dark luxury, cinematic, fully animated. Live at **https://webteam-96.github.io/deepak-rao/**.

**Every word on every page is copied verbatim from the current website.** Only the design changes: no text, number or name has been rewritten, and links point to the new pages. A checking script compares every visible text node on all 66 pages with the captured site and finds 0 changes. It also confirms that every line of each old page appears on its new page.

## Pages (66)

- `index.html`: the home page.
- 12 inner pages: `show.html`, `mental-abilities.html`, `clients.html` (699 event records, A–Z + search), `clients-list.html` (482 client names), `testimonials.html`, `audience-feedback.html` (218 letters, year index + search), `videos.html`, `profile.html`, `esp-book.html`, `book-launches.html`, `secrets-revealed.html` and `contact.html`.
- 52 video pages (`video-*.html`), one per video page of the old site, each with its title and caption. 29 play in the page. The other 23 link to YouTube, because their channel owner has turned off embedding.
- `404.html`.

The header, the phone menu and the footer link the main pages; each section's tabs link the rest.

## Design

- **Home.** A cinematic hero (stage photo, moving spotlight beams, drifting light dust, letter-by-letter title, floating "Asia's Only" seal), then:
  - two rows of client names that drift as you scroll;
  - the show poster, which tilts with the mouse;
  - a stats band;
  - a VIP wall whose 14-panel poster pans as you scroll;
  - a pinned horizontal gallery of 11 event photos;
  - videos in a lightbox, testimonials, the book, The 7th Sense;
  - a board of links to every section, and contact.
- **Inner pages.** Each page header has slowly turning gold rings and drifting light, and its title rises line by line. Images open up as they scroll into view. Short statements become cards, and the show's sequence becomes numbered steps. Cards catch a soft light under the pointer.
- **Directories.** The long pages have a sticky A–Z or year bar with live search.
- **Links.** Phone numbers and e-mail addresses are tappable, and every link opens in the same tab.
- **Motion.** Smooth scrolling uses Lenis; scroll animation uses GSAP + ScrollTrigger. People who ask for reduced motion get a still page.

## Checked

- **Chrome:** every page at 1440 and 390 px wide, and the pages linked from home at 768 too.
  - No sideways scrolling, 0 console errors, no broken images, one H1 per page.
- **Keyboard and screen readers:**
  - the skip link and the A–Z and year links move focus;
  - the phone menu behaves as a modal;
  - search results are announced;
  - content not yet scrolled into view can still be reached.
- **Without JavaScript,** every page still shows its content.

## Notes

- Photos are served as WebP made from the site's own files: 38 photos, 8.7 MB → 2.8 MB. The originals are low resolution, so the final build should use the client's high-res photos.
- The visit counter in the home footer is a snapshot taken when the site was captured. On the client's server it will be the live counter.
- An internet connection is needed for the fonts, the animation libraries and the videos.
