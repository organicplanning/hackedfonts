some modified monospace fonts for my personal use
------------------------------------

#### summary of modifications

- added a slashed zero to [GNU Unifont](http://www.unifoundry.com/unifont.html)
- added euro signs and some CE characters to some [classic DOS / BIOS fonts](http://int10h.org/oldschool-pc-fonts/)
- added dotted zero to [Lekton](http://luc.devroye.org/fonts-43679.html)
- set missing monospace flag for [Skyhook Mono](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)

### table of bitmap fonts in .ttf format


| font                 | *must* be set to size | rough equivalent   | serif | zero    | "feel"    |  
| -------------------- | --------------------- | ------------------ |------ | ------- |---------- |
| Envy Code B 10pt     | 10                    | Dina 9             |  no   | slashed | allround  |
| Px437 IBM ISO 9      | 12                    | Raize 12           |  no   | dotted  | allround  |
| Px437 IBM PS2 thin2  | 12                    | Camingo Code 1     |  no   | dotted  | technical |
| Px437 IBM PS2 thin4  | 12                    | Raize 11           |  no   | slashed | allround  |
| GNU Unifont          | 12                    | Liberation Mono 11 |  no   | slashed | clean     |
| Px437 Compaq 8x16    | 12                    | PT Mono 10         |  yes  | dotted  | laid back |
| Px437 Toshiba LCD    | 12                    | Go Mono 10	    |  yes  | slashed | ambitious |

#### Table of regular .ttf fonts
| font                 | rough equivalent | zero    | "feel"     |  
| -------------------- | ---------------- | ------- |----------- |
| Lekton               | Ubuntu Mono      | dotted  | fancy      |
| Skyhook Mono         | Tamsyn 10x20     | slashed | futuristic |                  

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
- By the slight stretching, PragmataPro feels more refined."designed". Personally, I prefer GNU Unifont most of the time.
  I like the feel, but surprisingly I like the feel of GNU Unicode better. 
- GNU Unifont supports east asian characters, unlike PragmataPro.
- [Iosevka](https://be5invis.github.io/Iosevka/) is an agreeable Pragmata Pro replacement for antialiased rendering.
- [Liberation Mono](https://www.fontsquirrel.com/fonts/Liberation-Mono) by RedHat is a little broader, but has a similar feel to GNU Unifont.


   

#### [Envy Code B 10 ttf](https://damieng.com/typography/envy-code-b)
- a bit like the also very useable [Dina 9](http://www.dcmembers.com/jibsen/download/61/)
  but with larger line spacing which can be good sometimes.
- by DamienG who has a lot more to offer (e.g. [8-bit retro fonts](https://damieng.com/blog/2011/02/20/typography-in-8-bits-system-fonts) and the cheerful [DamienTypewriter](http://2ttf.com/UjZ3WtVC))
- now added turkish characters dotless i, capital dotted I and soft g
- have not modified the .fon version yet

#### [Lekton](http://luc.devroye.org/fonts-43679.html)
- has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** and **Klartext Mono**
- now with dotted zero in order to distinguish letter oh and number zero
- still to be done: setting correct monospace flag with ttx
 
#### [Skyhook Mono Regular](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)
- futurisic monospace font, regular size is free, other styles available as paid offers
- had to correct the monospace bit with **ttx** from python pip fonttools to be able to use the font w/o workarounds.
- Personally I would prefer it when the author just sets the bit himself, after all it's supposed to be professional.
- I might not actually be allowed to offer it here. Fix it and I take it down.


#### [Vintage IBM fonts](http://int10h.org/oldschool-pc-fonts/)
- pixel sharp bitmap fonts as .ttf files, only useable at 12pt
- modded: added Euro sign and some turkish characters 
- to do for later: "unbreak" the pipe symbol
- IBM now offers [IBM Plex Mono](https://github.com/IBM/plex), but this is good only from 14pt upwards. Currently I still prefer the old ones.


'### vintage serif monospace fonts
- pixel sharp bitmap fonts as .ttf files, only useable at 12pt
- from http://int10h.org/oldschool-pc-fonts/ 

### Px437 Compaq 8x16
- good narrow allround mono serif font
- added Euro sign and some turkish characters: dotless i, capital dotted I, soft g

### Px437 ToshibaLCD
- slim and very clear

#### other serif monospace suggestions

- [PT Mono](https://www.fontsquirrel.com/fonts/list/foundry/paratype) by Paratype (includes cyrillic and greek, has wide range of pixel sharp small sizes)
- [Px437 IBM Thin1](http://int10h.org/oldschool-pc-fonts/) (relaxed feel, not yet modified) 
- [Go Mono](https://blog.golang.org/go-fonts) (quite slim, needs anti-aliasing)
- [Nimbus Mono](https://www.fontsquirrel.com/fonts/nimbus-mono) (somehow, this one calms me down)
- [Selectric](https://www.dafont.com/selectric.font) by Paradox (has nonslashed but distinguishable zero)
- [Damien Typewriter](http://2ttf.com/UjZ3WtVC) by DamienG (the Comic Sans of terminal fonts...)
- various **vintage typewriter fonts** by [Lukas Krakora](https://www.dafont.com/lukas-krakora.d1281) and [Peter Wiegel](https://www.dafont.com/peter-wiegel.d689)
  e.g. [Erica Type](https://www.1001fonts.com/erica-type-font.html) and [Oceanside Typewriter](https://www.dafont.com/oceanside-typewriter.font)


  

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
