# Absolve
_əbˈzɒlv_
A customisable theme overlay snippet for **Obsidian.md**.

![](Absolve%20Cover.png)

_Absolve_ is a CSS snippet designed to overlay your current theme and add features, preferences, and various tweaks. With good support for mobile, desktop, and Publish, you'll find that the sky's the limit with making your favourite theme **perfect for you**.

___

### Demonstration
![](Absolve%20Demo.gif)

### Setup
Setting up Absolve is a cinch! First off, make sure you have [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) installed.

Once you have the plugin required, go to the [releases page](https://github.com/mulfok/obsidian-absolve/releases) of the snippet's [Github Repo](https://github.com/mulfok/obsidian-absolve), and download `absolve.css`. Once you have it downloaded, navigate to your vault's and find the snippet folder (_yourvaultname/.obsidian/snippets_) and place the CSS file in the folder.

![](Installing%20Absolve.gif)

Once that’s done, go to the settings pane in Obsidian. Navigate to Appearance, CSS Snippets, and then click the reload button. Absolve should appear, and then you can turn it on.

![](Absolve%20In%20CSS.png)

Your setup is complete! To make use of Absolve’s [features](#Features), just go into your Style Settings menu, and tweak what you like. Have fun!

### Features

#### Admonition Columns
Admonition columns are a neat little way of sorting and displaying information. Pulled from Rainbell’s [extensive homepage resources](https://github.com/Rainbell129/Obsidian-Homepage), you can enable them through the “_Tweaks_” header in Style Settings.

To set them up, make sure you have javalent’s [Admonitions Plugin](https://github.com/valentine195/obsidian-admonition) installed. If you have/once you do, go to the settings tab and create custom admonitions `col1-4`.

![](https://cdn.discordapp.com/attachments/667421695841402910/944391020102172682/unknown.png)

It doesn’t matter what’s in the block, as long as it follows the name scheme `colX`. Once that’s all done, you can create your blocks normally. Below are some examples.

`````markdown
````ad-col3
title: 
```ad-note
title: Catatan2 Yang Bagus
- Satu
- Dua
- Tiga
- Empat
- Lima
```

```ad-bug
Roses are red,
Violets are blue,
Missing ')' at line 32.
```

```ad-warning
Floor slippery when wet!
```
````
`````

![](https://cdn.discordapp.com/attachments/667421695841402910/944392662813900800/unknown.png)

#### Image Grid
> NOTE:
> Image grid is _very_ finicky with kepano’s Minimal Theme.
> If you _do_ want to use it with Minimal, make sure to turn off _Maximise Media_ in the Minimal Settings Plugin.

The image grid is useful for when you need to present a gallery of images quickly within your notes. To enable them, open Absolve’s settings, navigate to _Aesthetics_, and turn on _Image Grids_.

To arrange your images into a grid, places images next to each other, and link to a heading `#grid`. If you are linking to an external image (_which I don’t recommend by the way; it doesn’t really work_), you can make the alt text `> grid`. Separate rows with line breaks.

```markdown
![[your_image_1.png#grid]]![[your_image_2.png#grid]]
![[your_image_3.png#grid]]![[your_image_4.png#grid]]![[your_image_5.png#grid]]
```

Below is an example of how I might use image grids.

![](https://cdn.discordapp.com/attachments/667421695841402910/944393379058425906/unknown.png)

#### Kanban Lists
Absolve offers its own style of Kanban Lists, with heading and subheading classes to emphasise topics within the lists you might create. They work nicely on Publish sites, and I regularly use them in my TTRPG notes. Below is an example source, and what it would make.

The line breaks after the HTML style implementation _is important_. The lists won’t render correctly unless with the line breaks like so.

```html
- <h5 class=head>Section One</h5>
	
	- Some notes…
	- Lorem ipsum dolor sit amet…
- <h5 class=head>Section Two</h5>

	- ![[dd-identicon.png]]
	- <h6 class=sub>Sub Section</h6>
	- Lorem ipsum dolor sit amet, consectetur adipiscing elit…
- <h5 class=head>Section Three</h5>

	- [ ] Todo
	- [x] Done!
	- [ ] Todo
```

Alternatively, through the _Markdown Attributes_ plugin, where the line breaking doesn’t matter.

```markdown
- ##### Section One {.head}
	- Some notes
	- Lorem ipsum dolor sit amet…
- ##### Section Two {.head}
	- ![[dd-identicon.png]]
	- ###### Sub Section {.sub}
		- Lorem ipsum dolor sit amet, consectetur adipiscing elit…
- ##### Section Three {.head}
	- [ ] Todo
	- [x] Done!
	- [ ] Todo
```

![](https://cdn.discordapp.com/attachments/667421695841402910/944393458242699284/Pasted_image_20220216222710.png)

#### officerhalf’s Handwritten Letters

### Checklist
- [ ] Aesthetics
	- [ ] Caret
		- [ ] Fill Colour
		- [ ] Outline Colour (Transparent for none)
		- [ ] Caret Style
			- [ ] Block
			- [ ] Pipe (Default)
	- [ ] Colours
		- [x] Accents ✅ 2022-02-11
			- [x] Text ✅ 2022-02-09
			- [x] Text Hover ✅ 2022-02-09
			- [x] Interactive ✅ 2022-02-09
			- [x] Interactive Hover ✅ 2022-02-09
		- [ ] Workspace
			- [x] Light Mode Colour Schemes ✅ 2022-02-11
				- [x] Notepad ✅ 2022-02-11
			- [x] Dark Mode Colour Schemes ✅ 2022-02-13
				- [x] Gruvbox ✅ 2022-02-13
			- [ ] File Navigation
	- [x] brimwats’ Fancy Blockquotes ✅ 2022-02-14
	- [x] brimwats’ Prism List Items (Edit Mode) ✅ 2022-02-14
	- [ ] brimwats’ Prism List Items (Preview Mode)
- [x] Design Schemes ✅ 2022-02-09
	- [x] Academia ✅ 2022-02-09
	- [x] TTRPG ✅ 2022-02-09
	- [x] Viridian ✅ 2022-02-09
- [ ] External Theme Features
	- [ ] Minimal Theme
		- [x] Toggle Checkboxes ✅ 2022-02-12
			- [ ] Checkbox Shape
	- [x] Sanctum ✅ 2022-02-11
		- [x] Toggle Aside Tags ✅ 2022-02-11
	- [ ] Shimmering Focus
		- [x] Toggle Footnote Indicators ✅ 2022-02-11
		- [ ] Toggle Unresolved Link Indicators
- [x] Highlighter ✅ 2022-02-12
- [x] mulfok-style Kanban ✅ 2022-02-12
- [x] Tweaks ✅ 2022-02-10
	- [x] Toggle Compact Admonitions ✅ 2022-02-09
	- [x] Toggle Rainbell’s Column Admonitions ✅ 2022-02-09
	- [x] Toggle Image Desaturation ✅ 2022-02-10
	- [x] Toggle No Nonsense Note Embeds ✅ 2022-02-11
	- [x] Resize Mermaid Graphs ✅ 2022-02-18
	- [x] Wrap Filenames ✅ 2022-02-18
	- [x] Hide Title bar text ✅ 2022-02-18
	- [x] Footnote tweaks ✅ 2022-02-18
- [x] Typography ✅ 2022-02-16
	- [x] Font Preferences ✅ 2022-02-09
		- [x] Preview Mode Font ✅ 2022-02-09
		- [x] Edit Mode Font ✅ 2022-02-09
		- [x] Header Font ✅ 2022-02-09
		- [x] Accent Font ✅ 2022-02-09
		- [x] User Interface Font ✅ 2022-02-09
	- [x] Font Sizes ✅ 2022-02-11
		- [x] File Navigation Font Size ✅ 2022-02-09
	- [x] Font Feature Settings ✅ 2022-02-09
		- [x] Toggle Ligatures ✅ 2022-02-09
		- [x] Toggle Slashed Zeroes ✅ 2022-02-09
		- [x] Toggle Alternate Glyphs ✅ 2022-02-09
	- [x] Headers ✅ 2022-02-11
		- [x] Header Colours ✅ 2022-02-11
		- [x] H1 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
		- [x] H2 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
		- [x] H3 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
		- [x] H4 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
		- [x] H5 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
		- [x] H6 Toggle: Italics, Text Transform, Font Variant; Change: Size, Align ✅ 2022-02-11
	- [x] Links ✅ 2022-02-16
		- [x] Toggle External Links Icon ✅ 2022-02-10
		- [x] Toggle Underline External Links ✅ 2022-02-10
		- [x] Toggle Underline Internal Links ✅ 2022-02-10
		- [x] Choose External Link Colour ✅ 2022-02-16

### Changelog
#### v2.4.0-beta
✨ **New**
- Added image grids > Aesthetics
- Added toggle for footnote changes > Tweaks

👾 **Bugfixes**
- Instead of targeting `img` within CSS, Absolve now targets `img[src]`. This should avoid an issue in upcoming Obsidian & Insider versions

🔧 **Changes**
- Removed “Colours” header. Now Accents, Caret, and Workspace colouring can be found easier
- Sanctum’s aside tags will now have a width of 50%. This is to avoid strange text wrapping on mobile

#### v2.3.1-beta
👾 **Bugfixes**
- officerhalf Handwritten Letters can now be applied through `cssclass: handwritten-letter`

❗ **Known Issues**
- Globally applied Handwritten Letters clash with brimwats’ Fancy Blockquotes

#### v2.3.0-beta
✨ **New**
- Added font “Lora” to bundled fonts.
- Added brimwats’ fancy blockquotes > Aesthetics
- Added brimwats’ prism list indicators > Aesthetics
- Choose external link colour > Aesthetics > Links

🔧 **Changes**
- Underline option on external/internal links now for _disabling_ pre-existing setting
- The Viridian design scheme preview mode text will now use “Lora”

👾 **Bugfixes**
- officerhalf’s handwritten letters should now render with the proper font

#### v2.2.0-beta
✨ **New**
- Added “Wrap Filenames” toggle > Tweaks
- Added “Resize Mermaid Graphs” & toggle > Tweaks
- Added table alignment option > Aesthetics
- Added “Font Accent” toggle > Typography > Fonts
- Added “Simpler Cites” toggle > Aesthetics
- Added “Hide Titlebar Text” toggle > Tweaks

👾 **Bugfixes**
- Fixed “Compact Ad~~om~~nitions” spelling error

🔧 **Changes**
- Added emojis preceding first-level headers