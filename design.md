version: alphaname: Crunchyrolldescription: A high-energy, content-forward streaming ecosystem built on a deep "Cinematic Black" canvas and "Crunchyroll Orange" (#ff6400), the signature electric hue used for primary CTAs, progress bars, and premium indicators. The design language utilizes "Crunchyroll Sans" at bold, heavy weights to mirror the intensity of shonen anime, while maintaining a clean, accessibility-focused layout.colors:primary: "#ff6400"primary-active: "#ff8233"primary-disabled: "#cc5000"premium-gold: "#fab918"success: "#2abdb3"error: "#f33"ink: "#ffffff"body: "#f2f2f2"muted: "#a0a0a0"hairline: "#333333"canvas: "#000000"surface-soft: "#141519"surface-card: "#23252b"surface-strong: "#212121"on-primary: "#000000"on-dark: "#ffffff"scrim: "#000000"typography:display-xl:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 40pxfontWeight: 900lineHeight: 1.1letterSpacing: -0.02emdisplay-lg:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 32pxfontWeight: 800lineHeight: 1.2letterSpacing: -0.01emdisplay-md:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 24pxfontWeight: 700lineHeight: 1.25letterSpacing: 0title-md:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 18pxfontWeight: 600lineHeight: 1.4letterSpacing: 0body-md:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 16pxfontWeight: 400lineHeight: 1.5letterSpacing: 0button:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 14pxfontWeight: 700lineHeight: 1.2letterSpacing: 0.05emtextTransform: uppercasebadge:fontFamily: "'Crunchyroll Sans', 'Lato', sans-serif"fontSize: 11pxfontWeight: 700lineHeight: 1.1letterSpacing: 0.05emtextTransform: uppercaserounded:none: 0pxxs: 2pxsm: 4pxmd: 8pxlg: 12pxfull: 9999pxspacing:xxs: 4pxxs: 8pxsm: 12pxmd: 16pxbase: 24pxlg: 32pxxl: 48pxsection: 80pxcomponents:
button-primary:
backgroundColor: "{colors.primary}"
textColor: "{colors.on-primary}"
typography: "{typography.button}"
rounded: "{rounded.sm}"
padding: 12px 24px
height: 48px
button-primary-active:
backgroundColor: "{colors.primary-active}"
textColor: "{colors.on-primary}"
rounded: "{rounded.sm}"
hero-cta-play:
backgroundColor: "{colors.primary}"
textColor: "{colors.on-primary}"
typography: "{typography.button}"
rounded: "{rounded.sm}"
padding: 12px 32px
height: 56px
content-card:
backgroundColor: "{colors.surface-soft}"
textColor: "{colors.ink}"
typography: "{typography.title-md}"
rounded: "{rounded.sm}"
premium-badge:
backgroundColor: "{colors.premium-gold}"
textColor: "{colors.on-primary}"
typography: "{typography.badge}"
rounded: "{rounded.xs}"
padding: 2px 6px
global-nav:
backgroundColor: "{colors.canvas}"
textColor: "{colors.ink}"
height: 72px
episode-progress:
backgroundColor: "{colors.primary}"
height: 4px
position: absolute-bottomOverviewCrunchyroll is a high-contrast, immersive entertainment platform. Unlike general marketplaces, it utilizes a "Dark Mode by Default" philosophy to make anime artwork pop. The base atmosphere is Cinematic Black ({colors.canvas}), punctuated by the signature Crunchyroll Orange ({colors.primary}) used for active states, playback controls, and the brand wordmark.Type runs "Crunchyroll Sans," a custom typeface designed for high-impact readability. The system leans heavily on extra-bold weights (800-900) for display sizes to mirror the intense, energetic nature of shonen anime. Shape language is functional and sharp; rounding is kept at a minimum ({rounded.sm} — 4px) to ensure the interface feels technical and sleek rather than "soft."Key Characteristics:Cinematic Canvas: The page floor is always {colors.canvas} (#000000) or deep grey {colors.surface-soft}.The Orange Voltage: {colors.primary} (#ff6400) carries every primary CTA ("Start Free Trial," "Watch Now"), progress bars, and active navigation indicators.Premium Tiering: A distinct Gold token ({colors.premium-gold}) is used for the "Crown" icon and badges to signal subscriber-only content.Content-First Grid: The layout is dominated by 2:3 vertical posters or 16:9 thumbnails with high-density metadata overlays.ColorsBrand & AccentPrimary ({colors.primary} — #ff6400): The iconic "Crunchyroll Orange." Used for Play buttons, active underlines in navigation, and progress sliders.Premium Gold ({colors.premium-gold} — #fab918): Used exclusively for premium membership features and content locking indicators.SurfaceCanvas ({colors.canvas} — #000000): The deep black background used for viewing and browsing.Surface Soft ({colors.surface-soft} — #141519): The secondary grey used for card backgrounds and search bars to provide subtle separation from the canvas.TextInk ({colors.ink} — #ffffff): Pure white, used for headlines and active button labels.Body ({colors.body} — #f2f2f2): Off-white for readability in long-form descriptions.Muted ({colors.muted} — #a0a0a0): Used for metadata like episode counts, genre tags, and timestamps.TypographyHierarchyTokenSizeWeightLine HeightLetter SpacingUse{typography.display-xl}40px9001.1-0.02emHero titles on browse pages{typography.display-lg}32px8001.2-0.01emSeries Detail page titles{typography.display-md}24px7001.250Section headers ("New Episodes"){typography.title-md}18px6001.40Episode titles{typography.body-md}16px4001.50Series descriptions{typography.button}14px7001.20.05emUppercase CTA labels{typography.badge}11px7001.10.05em"PREMIUM" and "DUB" tagsComponentsbutton-primary — The main "Start Free Trial" or "Subscribe" CTA. Background {colors.primary}, text {colors.on-primary}, uppercase {typography.button}, and minimal {rounded.sm} corner.content-card — The base unit for browsing. Typically a 2:3 aspect ratio poster. It uses {rounded.sm} corners and a {colors.surface-soft} background until the image loads. Metadata (Title, Rating, Category) is stacked immediately below the image.premium-badge — A small gold lozenge sitting top-left on content cards. Uses {colors.premium-gold} background with black text. It signals value and exclusivity at a glance.global-nav — A 72px tall bar at the top of the screen. Remains {colors.canvas} black with orange underlines for active routes.Do's and Don'tsDoUse pure black for the background in video-heavy areas.Keep typography weights high for headers—the brand is "loud" by nature.Reserve {colors.primary} for interactive elements only.Don'tDon't use large radius corners. The system should feel sharp and modern, not bubbly.Don't use white or light backgrounds for major page sections.Don't use lowercase for primary CTA buttons.
