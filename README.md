some modified fonts for my personal use
------------------------------------

- adding a distinguishable zero
- adding the Euro sign
- etc


### Monospace Fonts

- added a slashed zero to **GNU Unifont**
  https://en.wikipedia.org/wiki/GNU_Unifont
  http://www.unifoundry.com/unifont.html

  GNU Unifont looks like it inspired commercial font **PragmataPro**, although I haven't seen it acknowledged ... this would be a GPL issue anyway. 
  Although PragmataPro surely is nice, I actually prefer Unifont for the larger line spacing and the wider (!) range of Unicode characters
  as well as for the freedom to share it.

  GNU Unifont is a bitmap font in TTF format and is only good at 12pt. On the original page, Unix Bitmap formats are also available.

  To use GNU Unifont with **MobaXterm** (Windows)
  -  right-click on an open terminal window, 
  - select "change terminal settings" 
  - click on "Window/Apperance"
  - check the box "allow selection of variable width fonts" (MobaXterm doesn't recognise some monospace fonts as such, compare e.g. *Skyhook Mono*)
  - click the "change" button
  - now select "Unifont", size 12  
  
 
- added a dotted zero to **Lekton** http://luc.devroye.org/fonts-43679.html

  Lekton has a similar feel to **Ubuntu Mono** or maybe **Share Tech Mono** .

- added Euro signs to **IBM ISO9**, **IBM PS/2 thin2** and **IBM PS/2 thin4** from http://int10h.org/oldschool-pc-fonts/
  
  These are bitmap fonts in TTF format and are only good at 12pt

  **IBM Plex Mono** (available on https://github.com/IBM/plex) is a nice, modern and complete font, however for small sizes I prefer those old fonts I've modded.
  
  - IBM PS/2 thin2 has smaller numerals, like CamingoCode and some other fonts. It has a dotted zero.
  - IBM PS/2 thin4 is similar, more conventional, but reads quite well. The pipe symbol is "broken bar" in both, maybe I'll change that later https://en.wikipedia.org/wiki/Vertical_bar#Solid_vertical_bar_vs_broken_bar
  - IBM ISO 9 is larger (comparable to Bitstream Vera Sans Mono 11) and has a dotted zero.



#### sizes


<pre><code>
| font			       | rough reference size        | 
| IBM ISO 9 (select 12pt)      | Bitstream Vera Sans Mono 11 |
| IBM PS2 thin2  (select 12pt) | Bitstream Vera Sans Mono 10 |
| IBM PS2 thin4  (select 12pt) | Bitstream Vera Sans Mono 10 |
| GNU Unifont (select 12pt)    | Ubuntu Mono 12              |
</pre></code>
