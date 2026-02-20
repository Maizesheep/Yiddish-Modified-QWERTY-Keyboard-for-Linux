# Yiddish-Modified-QWERTY-Keyboard-for-Linux

This keyboard is a phonetic keyboard for Yiddish based off the US English QWERTY keyboard and Isaac Bleaman's Yiddish Klal keyboard for Mac, with some modifications that are mildly intuitive to me, with the principle that common letters should be easily typeable and the Shift key should modify letters or give Hebrew equivalents. Thank you to <a href="https://people.uleth.ca/~daniel.odonnell/Blog/custom-keyboard-in-linuxx11">Daniel O'Donnell</a> for creating the page that helped me understand how this works on Linux. Also, thank you to <a href="https://github.com/roelandmoors/azerty">roelandmoors</a> for the example of the xml file.

Most letters are phonetically equivalent, with exceptions including:
<ul>
  <li>i for י</li>
  <li>w for ש</li>
  <li>x for כ</li>
  <li>etc.</li>
</ul>

Shift + [key] includes these results:
<ul>
  <li>I for יִ</li>
  <li>W for שׂ</li>
  <li>X for ך</li>
  <li>etc.</li>
</ul>

Alt + [key] gives the combining diacritics for certain keys, as shown below with the symbols in the top right

Here's how to install YiddishQ (at least on Ubuntu, I just started using Kubuntu and that's all I know, check with your own distro if it's different)

1. Download the file I put in /symbols
2. Put this file in /usr/share/X11/xkb/symbols (you need to open as administrator to do this)
3. Go to /usr/share/X11/xkb/rules
4. Open both base.lst and evdev.lst and add the text from the file I named `lst.txt` at the bottom of the `! layout` section. 
You can find that section by Control + F and searching for `! variant`. Paste in the text below `Wolof` or below `custom`, whichever you prefer
5. Open both base.xml and evdev.xml and add the text from the file I named `xml.txt` before the end of the `layoutList` section.
You can find that section by Control + F and searching for `layoutList` and going to the second instance in the file. Paste in the text below `Wolof` or below `custom`, whichever you prefer
6. Consult the links below (especially the last one) if it doesn't work, and consult my chart for the locations of each letter. Happy typing!

<a href="https://www.youtube.com/watch?v=c_2ZEviudXY">YouTube</a>
<a href="https://help.ubuntu.com/community/Custom%20keyboard%20layout%20definitions">Ubuntu Forums</a>
<a href="https://ubuntu-mate.community/t/make-your-own-custom-keyboard-layout-for-linux/19733">Ubuntu Mate</a>

![keyboard-layout-linux](https://github.com/Maizesheep/Yiddish-Modified-QWERTY-Keyboard-for-Linux/assets/96145017/3d490904-595e-4e94-abd7-7bd6836e5d3e)
