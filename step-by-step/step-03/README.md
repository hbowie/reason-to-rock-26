# Step 03 — Add Web Fonts

The first thing to do here is to select some appropriately classy fonts for your website. 

I recommend [Butterick's Practical Typography](https://practicaltypography.com as an important educational resource on this topic.

In fact, I can also recommend the professional fonts designed and sold by Matthew Butterick, which can be found at [MBType.com](https://mbtype.com).

This is a little table I put together that lists his fonts, along with some of their key characteristics. 

| Name          | Serif | Sans | Semi | All-Caps | Monospaced |
| ------------- | ----- | ---- | ---- | -------- | ---------- |
| Advocate      |       |      |      | All-Caps |            |
| Century Supra | Serif |      |      |          |            |
| Concourse     |       | Sans |      |          |            |
| Equity        | Serif |      |      |          |            |
| Heliotrope    |       |      | Semi |          |            |
| Hermes Maia   |       | Sans |      |          |            |
| Triplicate    |       |      |      |          | Monospaced | 
| Valkyrie      | Serif |      |      |          |            |

After you've decided on the fonts to use, and made appropriate purchases, the following distinct steps needed to be followed in order to use the fonts. 

First, I created a `fonts` folder within the `web` folder. 

Next I copied the `.woff2` files for my selected fonts into the new `fonts` folder. 

Next I modified the `styles.css` file to pull in the selected font faces, using code like the following for each `.woff2` file. 

```
@font-face {
font-family: heliotrope_3;
font-style: normal;
font-weight: normal;
font-stretch: normal;
font-display: auto;
src: url('../fonts/heliotrope_3_regular.woff2') format('woff2');
}
```

With Butterick's fonts, I just edited the provided `sample.css` file for each font, copied his sample code, and pasted it into my `styles.css` file. (I like to place this code at the bottom of the `css` file.) 

The one adjustment that needs to be made to the sample code is to insert `../fonts/` before each of the file names, to add the relative path needed, based on the file placement I'm using.  

Finally, I had to adjust my `font-family` names in my `styles.css` file to pull in the web fonts, as opposed to using the system fonts installed on my Mac. This ensures that everyone will see the selected fonts once the site is finally uploaded to the web from my local machine. In the case of the Butterick fonts, this meant changing uppercase letters to lowercase, and replacing spaces with underscores. 

One important note about professional fonts: if you're storing your web project on GitHub, in a public repo, make sure to tell Git to ignore the font files, since these are protected by copyright, and should not be uploaded to any public repo on the web. 
