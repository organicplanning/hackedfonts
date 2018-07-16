some modified monospace fonts for my personal use
------------------------------------

#### summary of modifications

- added a slashed zero to [GNU Unifont](http://www.unifoundry.com/unifont.html)
- added euro signs and some CE characters to some [classic DOS / BIOS fonts](http://int10h.org/oldschool-pc-fonts/)
- added some CE characters to [Envy Code B 10pt TTF](https://damieng.com/typography/envy-code-b)
- added dotted zero and missing monospace flag to [Lekton](http://luc.devroye.org/fonts-43679.html)
- set missing monospace flag for [Skyhook Mono](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)
- added missing monospace flag to [fs-regulate](https://fontstruct.com/fontstructions/show/947828/fs_regulate), 
  [fn0t](https://www.dafontfree.net/freefonts-fn0t-f99496.htm) and [Generic Mono II](http://luc.devroye.org/fonts-75172.html).

#### table of bitmap fonts in .ttf format


| font                 | *must* be set to size | rough equivalent   | serif | zero    | "feel"    |  
| -------------------- | --------------------- | ------------------ |------ | ------- |---------- |
| Envy Code B 10pt     | 10                    | Dina 9             |  no   | slashed | allround  |
| Px437 IBM ISO 9      | 12                    | Raize 12           |  no   | dotted  | allround  |
| Px437 IBM PS2 thin2  | 12                    | Camingo Code 11    |  no   | dotted  | technical |
| Px437 IBM PS2 thin4  | 12                    | Raize 11           |  no   | slashed | allround  |
| GNU Unifont          | 12                    | Liberation Mono 11 |  no   | slashed | clean     |
| Px437 Compaq 8x16    | 12                    | PT Mono 10         |  yes  | dotted  | laid back |
| Px437 Toshiba LCD    | 12                    | Go Mono 10	    |  yes  | slashed | ambitious |

#### Table of regular .ttf fonts
| font                 | rough equivalent | zero    | "feel"     |  
| -------------------- | ---------------- | ------- |----------- |
| Lekton               | Ubuntu Mono      | dotted  | fancy      |
| Skyhook Mono         | Tamsyn 10x20     | slashed | futuristic |                  
| Generic Mono II      | Bitstream Vera   | slashed | clear      |                  
| fn0t		       | Skyhook Mono	  | (not distinguished)	| fancy	|
| fs-regulate	       | Quinze, AD Mono  | dotted | ornamental  |			 		   	


#### [GNU Unifont](http://www.unifoundry.com/unifont.html) 
- GNU Unifont is a bitmap font with wide Unicode coverage, only good at (nominally) 12px. 
- I've added a slashed zero.
- On the original page, Unix Bitmap formats are also available. I haven't modified these yet.
- Probably to *extreme range of characters*, conversion to "real monospace" with python fonttools ttx has failed so far.
- this is why it has to be selected as a variable pitch font in some terminals, see below for howto.
 
**Trivia**
- Personally I have a strong feeling that GNU Unifont closely "inspired" commercial font **PragmataPro**, although I haven't seen it acknowledged ... 
- this would be a real GPL issue anyway, especially as it is one of the most expensive fonts available.
  and the author even tried to raise money to "make it public domain." 
- GNU Unifont's only size fits right into PragmataPro's larger than usual size step between 10 and 11 pixels.
- PragmataPro has a larger i-dot. smaller line spacing and it seems stretched by one pixel compared with GNU Unifont.
- [Luculent](http://eastfarthing.com/luculent/) also has the large i-dot, is also pixel sharp between 7 and 14px and includes zodiac signs and [sparklines](https://aur.archlinux.org/packages/sparklines-git/).
- By the slight stretching, PragmataPro feels more refined/"designed". Personally, I prefer GNU Unifont most of the time.
  I like the feel, but surprisingly I like the feel of GNU Unicode better. 
- GNU Unifont supports east asian characters, unlike PragmataPro.
- [Iosevka](https://be5invis.github.io/Iosevka/) is an agreeable Pragmata Pro replacement for antialiased rendering.
- [Liberation Mono](https://www.fontsquirrel.com/fonts/Liberation-Mono) by RedHat is a little broader, but has a similar feel to GNU Unifont.

   

#### [Envy Code B 10 ttf](https://damieng.com/typography/envy-code-b)
- a bit like the also very useable [Dina 9](http://www.dcmembers.com/jibsen/download/61/)
  but with larger line spacing which can be good sometimes.
- now added turkish characters dotless i, capital dotted I and soft g

#### [Generic Mono II](http://luc.devroye.org/fonts-75172.html)
- sans-serif monospace font in the vein of Vera, with a friendly feel
- zero slash has lower angle than most
- now with corrected monospace bit (done with ttx)

#### [Lekton](http://luc.devroye.org/fonts-43679.html)
- has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** and **Klartext Mono**
- now with dotted zero in order to distinguish letter oh and number zero
- also done: setting correct monospace flag with ttx
 
#### [Skyhook Mono Regular](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)
- futurisic monospace font, regular size is free, other styles available as paid offers
- had to correct the monospace bit with **ttx** from python pip fonttools to be able to use the font w/o workarounds.
- Personally I would prefer it when the author just sets the bit himself, after all it's supposed to be professional.
- I might not actually be allowed to offer it here. Fix it and I take it down.

#### [fn0t](https://www.dafontfree.net/freefonts-fn0t-f99496.htm) 
- fancy / futuristic monospace font
- now with correct monospace flag

#### [Vintage IBM fonts](http://int10h.org/oldschool-pc-fonts/)
- pixel sharp bitmap fonts as .ttf files, only useable at 12pt
- modded: added Euro sign and some turkish characters 
- to do for later: "unbreak" the pipe symbol
- IBM now offers [IBM Plex Mono](https://github.com/IBM/plex), but this is good only from 14pt upwards. Currently I still prefer the old ones.



### vintage serif monospace fonts
- pixel sharp bitmap fonts as .ttf files, only useable at 12pt
- from http://int10h.org/oldschool-pc-fonts/ 

#### Px437 Compaq 8x16
- good narrow allround mono serif font
- added Euro sign and some turkish characters: dotless i, capital dotted I, soft g

#### Px437 ToshibaLCD
- slim and very clear

 

### HOWTO: Using "variable width fonts" in Putty / MobaXTerm

#### workaround
due to missing flags, some fonts are **not listed as monospace fonts**, meaning they are not visible in normal selection

- **right-click on an open terminal window** 
- select "change terminal settings" / "Window/Apperance"
- check the box **"allow selection of variable width fonts"**
- click the "change" button
- now, all available fonts are listed

#### correction

- The missing flags could possibly corrected with **ttx** from *python fonttools*
- After correction, those fonts are also selectable in [Xshell](https://www.netsarang.com/products/xsh_overview.html), which doesn't offer the workaround.


### font recommendations

*beside of what is available here* (because I modified it), **I'd like to make you aware of the following fonts**

#### other sans-serif monospace pixel suggestions

- [Tamsyn](http://www.fial.com/~scott/tamsyn-font/)
  - Tamsyn 10x20 has that futuristic "square" feel of quadra-style fonts like [White Rabbit](https://www.dafont.com/white-rabbit.font), [Earth 2073](https://www.dafont.com/earth-2073.font) or [Otonokizaka Mono II](https://fontstruct.com/fontstructions/show/1399210/otonokizaka-std-ii-1) or maybe  [Lekton](http://luc.devroye.org/fonts-43679.html) - but it is pixel sharp.
    The jagged "s" might feel nervous or energetic. Try it in pure green on black...
  - Tamsyn 7x13 is a quite small font that still feels relaxed.
- [Raize](http://www.raize.com/DevTools/Tools/RzFont.asp). 
  - 12px is a *good standard font* that can be replaced with *IBM ISO 9* for less edge.
  - 11px is small, broad and edgy, just like [Triskeline](http://www.netalive.org/tinkering/triskweline/) is small, broad and round.
- [Dina](http://www.dcmembers.com/jibsen/download/61/) 
  - Dina 9 is nearly equivalent to Envy Code B 10 TTF modified above, has less line spacing and maybe feels a little more joyful.
  - Dina 8 feels more relaxed than Tamsyn 7x14. 
  - Dina 6 is broader than Luculent 7. Size comparable to Sheldon / Sheldon Narrow.
- [Triskweline](http://www.netalive.org/tinkering/triskweline/) quite small, calm and broad. 
- [Luculent](http://eastfarthing.com/luculent/) is quite narrow, has a large dotted i and a wide range of characters. There are individual fonts for each pixel size. The zero is "backslashed" ...
  - Luculent 14 has single pixel width stems, which is unusual for that size and reminds me of plotter and DIN stencil fonts.
  - Luculent 12 is fancy but readable, not unlike Ubuntu Mono 13 
  - Luculent 11 is a size that I always come back to.
  - Luculent 9/10 is in same territory as Envy Code B 10px and Dina 9, but more rounded and with large i-dot
  - Luculent 7 is surprisingly readable for the size (smaller than Dina 6) though feeling a little strained.
- [Sheldon Narrow](https://web.archive.org/web/20170203072652/http://tobiasjung.name/profont/index.php) (a ProFont replacement by Sheldon Simms) and especially the more widely spaced **Sheldon** are very small but quite readable and good for side-by-side comparison of code.
- [zevv-peep](http://zevv.nl/play/code/zevv-peep/): both beautiful and good to read though sadly lacking character range. Somewhere between Luculent and Ubuntu Mono / Lekton. Listed as "peep" in font list.

#### other serif monospace suggestions

##### pixel sharp fonts

- [PT Mono](https://www.fontsquirrel.com/fonts/list/foundry/paratype) by Paratype: Medium width serif font that has wide range of pixel sharp small sizes and includes cyrillic and greek
- [Px437 IBM Thin1](http://int10h.org/oldschool-pc-fonts/) (relaxed feel, not yet modified) 
- [Nimbus Mono](https://www.fontsquirrel.com/fonts/nimbus-mono) somehow, this one calms me down. Broad and thin. pixel sharp in 14px

#### needing anti-aliasing

- [Go Mono](https://blog.golang.org/go-fonts): quite narrow, needs anti-aliasing
- [Luxi Mono](https://www.fontsquirrel.com/fonts/Luxi-Mono): not bad but lacks zero-oh distinction.
- [Selectric](https://www.dafont.com/selectric.font) by Paradox: Very good Courier replacement. Has nonslashed but distinguishable zero.
- [Courier Prime Code](https://www.fontsquirrel.com/fonts/courier-prime-code). West coast calm but needs anti-aliasing.
- [Damien Typewriter](http://2ttf.com/UjZ3WtVC) by DamienG: the Comic Sans of terminal fonts... could use some additional characters.
- various **vintage typewriter fonts** by [Lukas Krakora](https://www.dafont.com/lukas-krakora.d1281) and [Peter Wiegel](https://www.dafont.com/peter-wiegel.d689)
  e.g. [Erica Type](https://www.1001fonts.com/erica-type-font.html) and [Oceanside Typewriter](https://www.dafont.com/oceanside-typewriter.font)

