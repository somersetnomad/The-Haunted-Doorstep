# The Haunted Doorstep

An interactive Halloween website. Light real-feeling candles, meet a watching owl, draw a sigil that fractals into a portal, knock on a door and see what answers. It is one self-contained HTML file with no build step and no dependencies to install.

**Live page:** https://claude.ai/artifact/W7V3AKB9vs56im4e4hjLys (private until shared from the page's Share menu)

## What is on the page

| Section | What you can do |
| --- | --- |
| **Hero** | Candlelit portrait, spiders crawling by the pumpkins that scatter when your cursor gets close, and a daily omen with your visit streak. |
| **Meet the watcher** | A real owl on a falconry glove, filmed by the site owner. Tap it for eight owl facts. |
| **The coven** | Five witch scenes. Tap one and the coven casts: a sigil draws itself, fractals outward and opens a portal. Draw your own sigil on the pad and save it as a picture. |
| **Ravens** | Red-eyed ravens fly across the page. Click them as they pass. |
| **The apple oracle** | Tap an apple to cut it across the middle, then touch the star inside to cast a spell. Ask the oracle for a fortune. |
| **Wax works** | Five candles that burn down, pool and drip. Bring the cursor near and a flame leans away. Light all five for a séance. |
| **The pumpkin patch and carving table** | Six pumpkin varieties, each with its own story. Choose a pumpkin, eyes and mouth, then light the candle inside. |
| **Inside a spider's web** | A real orb-weaver photo with five numbered hotspots to inspect. |
| **Spooky facts** | Six cards that flip and glow. |
| **The skeleton crew** | Nine photos, each hiding a myth-or-truth Halloween fact. |
| **Knock knock** | A wooden door that swings open on a different treat or trick every time. |
| **Until Halloween night** | A large live countdown to 6pm on 31 October that grows more ominous as the date nears. |

## Keeps you coming back

- **Collection:** 19 achievements, each with a hint, in a drawer opened from the 📖 button in the top bar. Progress is saved in your browser.
- **Streak and omen:** a visit streak counter and a different omen each day.
- **Midnight mode:** reaching 10 finds unlocks a moonlit blue version of the whole page.
- **Save my sigil:** renders the sigil you drew as a shareable poster image.

## Sound, accessibility and phones

- Sound is **off** by default. The 🔇/🔊 button switches on sound effects and a quiet ambient drone.
- Respects the reduced-motion setting: the roaming spiders, bats, ravens and crawlers are not started.
- Keyboard focus outlines, 44px touch targets on phones, and screen-reader labels on the main interactive pieces.
- The video loads only when you scroll to it.

## Technical notes

- A single `haunted-doorstep.html` file, around 3 MB. Photos are embedded as WebP; the owl film is embedded as MP4 and decoded to a blob URL in the browser.
- Plain HTML, CSS and JavaScript. Canvas 2D draws the sigils and portal; SVG draws the spiders, ravens, pumpkins and treats; the Web Audio API synthesises every sound, so there are no audio files.
- Fonts are Fraunces and Lora from Google Fonts. Without a connection the page falls back to Georgia.
- State saved in `localStorage`: `hd_score`, `hd_got`, `hd_mid`, `hd_last`, `hd_streak`. Clear site data to reset everything.
- The sigil download uses the claude.ai viewer's save prompt when hosted there and falls back to a normal download elsewhere.

## Editing it

Open the file in any text editor. The page is organised in this order: styles (with later sections overriding earlier ones), the HTML sections, then a single script. Large `data:` URIs hold the images and video, so search by section id (`#coven`, `#knockS`, `#webs`, `#orchard`, `#count`) rather than scrolling.

## Credits

**Photography (Pexels):** skeleton crew, Charles Parker. Orb-weaver spider, Ankit Rainloure. Cobweb window, Karola G. Candles, jahratreza. Pumpkins, kubiko. Witches and orchard scenes, viktoriyadr. Black-and-white bird, lebele. Bird portrait, Matt Richmond. The owl film and the photo of hands holding apples were supplied by the site owner.

**Fonts:** Fraunces and Lora (Google Fonts).

## A note on the facts

Fact text is written from general knowledge of Halloween history, folklore and natural history. It has not been checked line by line against primary sources, so verify anything before you repeat it. Good places to start: Encyclopaedia Britannica and Smithsonian Magazine on Halloween history, Historic Royal Palaces on the Tower of London ravens, and the Barn Owl Trust on owls. The "ravens" in the photographs are dark birds that may be crows.
