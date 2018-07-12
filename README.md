some modified monospace fonts for my personal use
------------------------------------

- added a slashed zero to GNU Unifont
- added euro signs and some CE characters to some classic DOS / BIOS fonts
- added dotted zero to Lekton
- set missing monospace flag for Skyhook Mono

#### [GNU Unifont](http://www.unifoundry.com/unifont.html) 
- GNU Unifont is a bitmap font, only good at 12Px. On the original page, Unix Bitmap formats are also available. I haven't modified these.
- looks like it inspired commercial font **PragmataPro**, although I haven't seen it acknowledged ... 
  this would be a real GPL issue anyway, especially as it is one of the most expensive fonts available
  and the "author" even tried to raise money to "make it public domain."
- He'll probably get away with it because he stretched the font vertically by one pixel, so it's "really different"
- Compared with GNU Unifont, Pragmata Pro has better visibility for the i-dot, quite comparable with Luculent-
- Pragmata Pro has real merit for adding a variety of sharp pixel sizes to the 12px-only Unifont.
- Things I prefer with Unifont to Pragmata Pro is the larger line spacing and the wider (!) range of Unicode characters
  as well as for the freedom to share it.
- Iosevka is an agreeable Pragmata Pro replacement for antialiased rendering.
- Probably to extreme size / range of characters, conversion to "real monospace" with python fonttools ttx has failed so far.
- *To use GNU Unifont with MobaXterm* (Windows)
  - right-click on an open terminal window, 
  - select "change terminal settings" 
  - click on "Window/Apperance"
  - check the box "allow selection of variable width fonts"
  - click the "change" button
  - now select "Unifont", size 12  
   

#### [Lekton](http://luc.devroye.org/fonts-43679.html)
- has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** and **Klartext Mono**
- now with dotted zero.
- to be done: set correct monospace flag
 
#### [Skyhook Mono Regular](https://www.myfonts.com/fonts/fontom-type/skyhook-mono/regular/)
- futurisic monospace font
- now corrected monospace bit with **ttx** from python pip fonttools 
  in order to be directly selectable in MobaXTerm et al (w/o detour "allow selection of variable pitch fonts")


#### Vintage IBM fonts

- I believe these are still superior to [IBM Plex Mono](https://github.com/IBM/plex), especially at small sizes. 
- bitmap fonts in TTF format, pixel sharp, must be selected as (nominally) 12pt
- modded: added Euro sign and some turkish characters 
- to do for later: "unbreak" the pipe symbol

*characteristics*
- IBM PS/2 thin2 has smaller-than-usual numerals (compare CamingoCode font) and feels quite technical.
- IBM PS/2 thin4 and the somewhat larger IBM ISO 9 seem like very good allround fonts.

not yet modified
- IBM PS/2 thin1 is a serif font with a relaxed feel and large i dots
- IBM PS/2 thin3 is a quadra-style font with a scifi / retro future feel

### Serif Monospace

Px437 Compaq 8x16
- from http://int10h.org/oldschool-pc-fonts/
- added Euro sign and some turkish characters: dotless i, capital dotted I, soft g

Px437 ToshibaLCD
- slim and very clear
- this is a bitmap font, only good at 12pt

*other serif monospace suggestions:* 
- Px437 IBM Thin1 (not yet modified) 
- PT Mono (quite complete already, wide range of pixel sharp small sizes)

#### font sizes for comparison


| font @ "12px"        | rough reference size            | serif | zero    |  
| -------------------- | ------------------------------- | ----- | ------- |
| Px437 IBM ISO 9      | Bitstream Vera Sans Mono 11     |  no   | dotted  |
| Px437 IBM PS2 thin2  | Bitstream Vera Sans Mono 10     |  no   | dotted  |
| Px437 IBM PS2 thin4  | Bitstream Vera Sans Mono 10     |  no   | slashed |
| GNU Unifont          | < PragmataPro 11                |  no   | slashed |
| Px437 Compaq 8x16    | PT Mono 10                      |  yes  | dotted  |
| Px437 Toshiba LCD    | PT Mono 10	                 |  yes  | slashed |
