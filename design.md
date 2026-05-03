version	alpha
name	Crunchyroll
description	A high-energy, content-forward streaming ecosystem built on a deep "Cinematic Black" canvas and "Crunchyroll Orange" (#ff6400), the signature electric hue used for primary CTAs, progress bars, and premium indicators. The design language utilizes "Crunchyroll Sans" at bold, heavy weights to mirror the intensity of shonen anime, while maintaining a clean, accessibility-focused layout. UI elements favor sharp, functional corners over the "friendly" curves of general marketplaces—using subtle rounding ({rounded.sm} ~4px) only to soften interactive surfaces. The interface prioritizes immersive artwork and high-contrast metadata to ensure legibility in low-light viewing environments across web, mobile, and living room devices.
colors	
primary	primary-active	primary-disabled	premium-gold	success	error	ink	body	muted	hairline	canvas	surface-soft	surface-card	surface-strong	on-primary	on-dark	scrim
#ff6400
#ff8233
#cc5000
#fab918
#2abdb3
#f33
#ffffff
#f2f2f2
#a0a0a0
#333333
#000000
#141519
#23252b
#212121
#000000
#ffffff
#000000
typography	
display-xl	display-lg	display-md	display-sm	title-md	title-sm	body-md	body-sm	caption	badge	micro-label	button-md	button-sm	nav-link
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', 'Helvetica Neue', helvetica, sans-serif
40px
900
1.1
-0.02em
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
32px
800
1.2
-0.01em
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
24px
700
1.25
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
20px
700
1.3
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
18px
600
1.4
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
16px
600
1.4
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
16px
400
1.5
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
14px
400
1.5
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
12px
500
1.4
0.02em
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing	textTransform
'Crunchyroll Sans', 'Lato', sans-serif
11px
700
1.1
0.05em
uppercase
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
10px
600
1.2
0
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing	textTransform
'Crunchyroll Sans', 'Lato', sans-serif
14px
700
1.2
0.05em
uppercase
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing	textTransform
'Crunchyroll Sans', 'Lato', sans-serif
12px
700
1.2
0.05em
uppercase
fontFamily	fontSize	fontWeight	lineHeight	letterSpacing
'Crunchyroll Sans', 'Lato', sans-serif
16px
700
1.0
0
rounded	
none	xs	sm	md	lg	full
0px
2px
4px
8px
12px
9999px
spacing	
xxs	xs	sm	md	base	lg	xl	xxl	section
4px
8px
12px
16px
24px
32px
48px
64px
80px
components	
button-primary	button-primary-active	button-secondary	button-ghost	hero-cta-play	global-nav	nav-item-active	content-card	premium-badge	episode-progress	search-bar-input	footer-dark
backgroundColor	textColor	typography	rounded	padding	height
{colors.primary}
{colors.on-primary}
{typography.button-md}
{rounded.sm}
12px 24px
48px
backgroundColor	textColor	rounded
{colors.primary-active}
{colors.on-primary}
{rounded.sm}
backgroundColor	textColor	typography	rounded	padding	height
{colors.surface-card}
{colors.ink}
{typography.button-md}
{rounded.sm}
12px 24px
48px
backgroundColor	textColor	typography	rounded	padding
transparent
{colors.ink}
{typography.button-md}
{rounded.none}
0px
backgroundColor	textColor	typography	rounded	padding	height
{colors.primary}
{colors.on-primary}
{typography.button-md}
{rounded.sm}
12px 32px
56px
backgroundColor	textColor	height	borderBottom
{colors.canvas}
{colors.ink}
72px
4px solid {colors.primary} (bottom-active)
backgroundColor	textColor	typography
transparent
{colors.primary}
{typography.nav-link}
backgroundColor	textColor	typography	rounded
{colors.surface-soft}
{colors.ink}
{typography.title-sm}
{rounded.sm}
backgroundColor	textColor	typography	rounded	padding
{colors.premium-gold}
{colors.on-primary}
{typography.badge}
{rounded.xs}
2px 6px
backgroundColor	height	position
{colors.primary}
4px
absolute-bottom
backgroundColor	textColor	typography	rounded	padding
{colors.surface-card}
{colors.ink}
{typography.body-sm}
{rounded.sm}
8px 16px
backgroundColor	textColor	padding
{colors.canvas}
{colors.muted}
48px 24px
Overview
Crunchyroll is a high-contrast, immersive entertainment platform. Unlike marketplace-style designs, it utilizes a "Dark Mode by Default" philosophy to make anime artwork pop. The primary brand color is Crunchyroll Orange ({colors.primary} — #ff6400), used strategically for active states, calls to action, and the iconic "Premium" crown iconography.

Typography is bold and expressive, utilizing Crunchyroll Sans. Headlines often use heavy weights (800-900) to match the energetic tone of the content. Visual hierarchy is established through size and color contrast rather than whitespace, as the platform favors a "lean-back" experience where content density is high.

Key Characteristics:
- **Cinematic Canvas:** A pure black ({colors.canvas}) or deep grey ({colors.surface-soft}) background is mandatory for all viewing surfaces.
- **Orange Accents:** Used for the "Play" buttons, "Subscribe" CTAs, and progress bars.
- **Card-Based Browsing:** Content is organized in "Posters" (vertical 2:3) or "Thumbnails" (horizontal 16:9) with minimal rounding.
- **Premium Tiering:** A distinct Gold token ({colors.premium-gold}) marks member-only content.
