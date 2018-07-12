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
- GNU Unifont is a bitmap font, only good at 12Px. On the original page, Unix Bitmap formats are also available. I haven't modified these.
- looks like it inspired commercial font **PragmataPro**, although I haven't seen it acknowledged ... 
  this would be a real GPL issue anyway, especially as it is one of the most expensive fonts available
  and the "author" even tried to raise money to "make it public domain."
- He'll probably get away with it because he stretched the font vertically by one pixel, so it's "really different". Actually, it feels more "designed" then.
- Compared with GNU Unifont, Pragmata Pro has better visibility for the i-dot, quite comparable with [Luculent](http://eastfarthing.com/luculent/).

- Pragmata Pro has real merit for adding a variety of sharp pixel sizes to the 12px-only Unifont.
- Things I prefer with Unifont to Pragmata Pro is the larger line spacing and the wider (!) range of Unicode characters
  as well as for the freedom to share it.
- Iosevka is an agreeable Pragmata Pro replacement for antialiased rendering.
- Liberation Mono feels similar to GNU Unifont
- Probably to extreme size / range of characters, conversion to "real monospace" with python fonttools ttx has failed so far.
- *To use GNU Unifont with MobaXterm* (Windows)
  - right-click on an open terminal window, 
  - select "change terminal settings" 
  - click on "Window/Apperance"
  - check the box "allow selection of variable width fonts"
  - click the "change" button
  - now select "Unifont", size 12  
   

### [Envy Code B 10 ttf](https://damieng.com/typography/envy-code-b)

- a bit like [Dina 9](http://www.dcmembers.com/jibsen/download/61/)
  but with larger line spacing which can ce good sometimes.
- now added turkish characters dotless i, capital dotted I and soft g

#### [Lekton](http://luc.devroye.org/fonts-43679.html)
- has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** and **Klartext Mono**
- now with dotted zero in order to distinguish letter oh and number zero
- still to be done: setting correct monospace flag with ttx
 
#### [Skyhook Mono Regular](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)
- futurisic monospace font, regular size is free
- now corrected monospace bit with **ttx** from python pip fonttools 
  in order to be directly selectable in MobaXTerm et al (w/o detour "allow selection of variable pitch fonts")


#### [Vintage IBM fonts](http://int10h.org/oldschool-pc-fonts/)

- I believe these are still superior to [IBM Plex Mono](https://github.com/IBM/plex), especially at small sizes. 
- bitmap fonts in TTF format, pixel sharp, must be selected as (nominally) 12pt
- modded: added Euro sign and some turkish characters 
- to do for later: "unbreak" the pipe symbol

*characteristics*
- IBM PS/2 thin2: smaller-than-usual numerals (compare CamingoCode font) and feels quite technical.
- IBM PS/2 thin4: good allround font
- IBM ISO 9: good allround font

not yet modified
- IBM PS/2 thin1 is a serif font with a relaxed feel and large i dots
- IBM PS/2 thin3 is a quadra-style font with a scifi / retro future feel

### Serif Monospace
- from http://int10h.org/oldschool-pc-fonts/ 
- only usable at nominally 12pt
- pixel sharp bitmap fonts as .ttf files

Px437 Compaq 8x16
- good narrow allround mono serif font
- added Euro sign and some turkish characters: dotless i, capital dotted I, soft g

Px437 ToshibaLCD
- slim and very clear

*other serif monospace suggestions:* 
- Px437 IBM Thin1 (not yet modified) 
- PT Mono (quite complete already, wide range of pixel sharp small sizes)

