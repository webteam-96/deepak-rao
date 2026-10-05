# Deepak Rao ESP — website redesign sample

Homepage design sample for [deepakrao-esp.com](https://www.deepakrao-esp.com/). Dark luxury, cinematic, fully animated.

**Every word on the page is copied verbatim from the current website.** Only the design changes: no text, number, name or link has been rewritten. A checking script compared every visible text node against the captured site and found 0 changes.

## View it

- Open `index.html` in a browser (an internet connection is needed for the fonts, animation library and videos), or
- Enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root) and open `https://webteam-96.github.io/deepak-rao/`.

## What's in the page

- Cinematic hero: stage photo fading into black, moving spotlight beams, drifting light dust, letter-by-letter title reveal, floating "Asia's Only" seal.
- Infinite gold marquee of real client names.
- The Show, with the ESP Mind Show poster (tilts with the mouse).
- Stats band, VIP wall where the 14-panel poster pans while each dignitary lights up on scroll.
- Pinned horizontal gallery of event photos.
- Video grid that plays in a lightbox (only videos whose owner allows embedding), testimonials slider, the book, The 7th Sense, contact.
- Smooth scrolling (Lenis), scroll animations (GSAP + ScrollTrigger), custom cursor, magnetic buttons. Reduced-motion users get a static page; without JavaScript all content still shows.

## Pages

`index.html` (home), `clients.html` (699 event records, A–Z + search), `clients-list.html` (482 client names), `testimonials.html`, `audience-feedback.html` (218 letters, year index + search), `videos.html`, `show.html`, `mental-abilities.html`, `profile.html`, `esp-book.html`, `book-launches.html`, `secrets-revealed.html`, `contact.html`, `404.html`. All linked from the header, menu and footer. Inner pages are generated from the verified content models, so their text is verbatim too.

## Checked

Chrome at 1440, 768 and 390px wide: no sideways scrolling, 0 console errors, no broken images, one H1. Video lightbox, phone menu and testimonial slider tested.

## Notes

- 20 of the site's 56 YouTube videos have embedding disabled by the channel owner; those open on YouTube instead of in the lightbox.
- The original photos are low resolution. The final build should use the client's original high-res photos (and ideally a stage video for the hero).
- Images are the site's originals, unoptimised. The production build will serve compressed AVIF/WebP versions.
