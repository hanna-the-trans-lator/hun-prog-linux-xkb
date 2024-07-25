# ENGLISH INSTRUCTIONS AT THE END
# Magyar (Programozói) billentyűzetkiosztás @adopc233 által, átírva Windowsról Linuxra (xkb formátum)
Nincs semmi köze a Hewlett-Packardhoz.
Köszönöm ezeket a fejlesztőket, mivel felhasználtam munkájukat: <br />
Az eredeti kiosztás adopc233tól: https://github.com/adopc233/Hungarian-Programmers-keyboard-layout <br />
Ezen cikk a Kavaliertől: https://www.kavalier.tv/blog/custom-keyboard-layout-for-coding-on-ubuntu-linux <br />
@alexkriss -tól a keyboard layout converter: https://github.com/alexriss/keyboard-layout-converter <br />
<br />
# telepítési útmutató:
1. Töltse le a 'hp' fáljt erről az oldalról <br />
2. Másolja át a fáljt a "/usr/share/X11/xkb/symbols/" mappába. (Ehez kell root engedély!) <br /> 
3. Nyissa meg a /usr/share/X11/xkb/symbols/evdev.xml dokumentumot a kedvenc szövegszerkeztő alkalmazással. (Ehez is kell root engedély.) <br />
4. Keresse meg (ctrl + f) ezt a szövegsort: \</layoutList\>
5. E fölött látható egy "custom" szöveg.
6. Itt duplikálja (ctrl + c, ctrl + v, ctrl+ v) a legközelebbi "\<layout\>" és "\</layout\>" közötti területet (azokkal együtt).
7. Az új területen a \<name\> közötti "custom" szöveget írja át "hp"-ra.
8. A \<shortDescription\> közötti "custom" feliratot is.
9. A \<description\> Között írd azt hogy "Magyar (Programozói)" vagy "Hungarian (Programmers)", ízlés szerint.
10. Az \<iso639Id\> közöttit arra hogy "HU".
11. Ezek után valahogy így kell kinéznie:
![image](https://github.com/user-attachments/assets/3b9ba5b6-b7b1-4b3f-a8c9-f2bd04583590)
12. Indítsa újra a rendszert.
13. Adja hozzá a kiosztást normálisan.
14. Állítsa át az "Alternatív karakterek billentyű"-t a Jobb Altra (AltGr).
15. Kész!

# A port of the Hungarian (Programmers) keyboard layout by @adopc233 from Windows to Linux (xkb).
no relation to Hewlett-Packard.
tools used: <br />
the original files from adopc233: https://github.com/adopc233/Hungarian-Programmers-keyboard-layout <br />
this guide by kavalier: https://www.kavalier.tv/blog/custom-keyboard-layout-for-coding-on-ubuntu-linux <br />
keyboard layout converter by @alexkriss: https://github.com/alexriss/keyboard-layout-converter <br />
<br />
# installation instructions:

1. Download the "hp' file from this repository <br />
2. Copy the file to "/usr/share/X11/xkb/symbols/". (this requires root perms.) <br /> 
3. Open /usr/share/X11/xkb/symbols/evdev.xml with your text editor of choice. (this also requires root perms.) <br />
4. Find (ctrl + f) this word: \</layoutList\>
5. There is a "custom" field visible above here.
6. Duplicate (ctrl + c, ctrl + v, ctrl+ v) the field between the closest "\<layout\>" and "\</layout\>" (including these).
7. In this new field change the \<name\> variable from "custom" to "hp".
8. Also \<shortDescription\>.
9. Change \<description\> to "Magyar (Programozói)" or "Hungarian (Programmers)", to taste.
10. Change \<iso639Id\> to "HU".
11. The file should look something like this afterwards:
![image](https://github.com/user-attachments/assets/3b9ba5b6-b7b1-4b3f-a8c9-f2bd04583590)
12. Restart your computer.
13. Add the layout as normal.
14. Change the "Alternate Characters Key" to Right Alt (AltGr).
15. You're done!
