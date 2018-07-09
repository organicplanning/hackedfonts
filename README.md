some modified fonts for my personal use
------------------------------------

- adding a distinguishable zero
- adding the Euro sign
- etc


### Monospace Fonts


- added a slashed zero to **GNU Unifont**
  https://en.wikipedia.org/wiki/GNU_Unifont
  http://www.unifoundry.com/unifont.html
#### GNU Unifont 
- GNU Unifont is a bitmap font, only good at 12Px. On the original page, Unix Bitmap formats are also available. I haven't modified these.
- looks like it inspired commercial font **PragmataPro**, although I haven't seen it acknowledged ... 
  this would be a GPL issue anyway, especially as it is one of the most expensive fonts available
  and the "author" even tried to raise money to "make it public domain.
- Compared with GNU Unifont, Pragmata Pro has better visibility for the i-dot, quite comparable with Luculent
- Things I prefer with Unifont to Pragmata Pro is the larger line spacing and the wider (!) range of Unicode characters
  as well as for the freedom to share it.
- Probably to extreme size / range of characters, conversion to "real monospace" with python fonttools ttx has failed so far.
- *To use GNU Unifont with MobaXterm* (Windows)
  - right-click on an open terminal window, 
  - select "change terminal settings" 
  - click on "Window/Apperance"
  - check the box "allow selection of variable width fonts"
  - click the "change" button
  - now select "Unifont", size 12  
   

#### Lekton
- http://luc.devroye.org/fonts-43679.html
- has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** and ** Klartext Mono*
- I've added a dotted zero.
 
#### Skyhook
- futurisic monospace font
- now converted to "real monospace" with ttx from python pip fonttools 
  in order to be directly selectable in MobaXTerm et al (w/o detour "allow selection of variable pitch fonts")

### [Px series](http://int10h.org/oldschool-pc-fonts/) vintage IBM fonts
- I believe these are still superior to [IBM Plex Mono](https://github.com/IBM/plex), especially at small sizes. 
- These are pixel sharp bitmap fonts in TTF format and are only good at 12pt
- modification done: added Euro signs to **IBM ISO9**, **IBM PS/2 thin2** and **IBM PS/2 thin4** 
- intended modification for later: "unbreak" the pipe symbol

*characteristics*
- IBM PS/2 thin2 has smaller numerals, (compare e.g. CamingoCode) and a dotted zero.
- IBM PS/2 thin4 has conventinally sized numerals and slashed zero. 
- IBM ISO 9 is somewhat larger and has a dotted zero.

### Serif Monospace

Px437 Compaq 8x16
- from http://int10h.org/oldschool-pc-fonts/
- added Euro sign and some turkish characters: dotless i, capital dotted I, soft g
- this is a bitmap font, only good at 12pt

*other serif monospace suggestions:* 
- Px437 ToshibaLCD, Px437 IBM Thin1 (both not yet modified), 
- PT Mono (quite complete already, wide range of pixel sharp small sizes)

#### font sizes for comparison


| font @ "12px"        | rough reference size            | 
| -------------------- | ------------------------------- |
| Px437 IBM ISO    9   | Bitstream Vera Sans Mono 11     |
| Px437 IBM PS2 thin2  | Bitstream Vera Sans Mono 10     |
| Px437 IBM PS2 thin4  |  Bitstream Vera Sans Mono 10    |
| GNU Unifont          | Ubuntu Mono 12                  |
| Px437 Compaq 8x16    | PT Mono 10-11                   |
