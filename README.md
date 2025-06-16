# https://github.com/farshid-azady/class-Css

- ##### -white space when we have a space that smaller than our text size, it will be white.

### white-space: nowrap;

- 1-white-space: nowrap;
- 2-overflow: hidden;
- 3-text-overflow: ellipsis;
- 4-text-decoration: none;
- 5-word-wrap: none;
- 6-word-break: normal;
- 7-text-align: justify;
- 8-cursor: pointer

### vendor prefix for this property is -ms- or -o- or -moz- or -webkit- or -khtml-

- #### A vendor prefixes is a special prefix added to a CSS property. Each rendering engine has it's own prefix which will only apply the property to that particular browser. Vender Prefixes in 2017. Much less necessary, but still used. if you use the Old Browser Like IE6/IE7/IE8 then you should add this vendor prefixes.

- ### Directions
  - - directions : the name of our custom class with vendor prefix
  - .directions{
  -         writing-mode: vertical-lr;
  -        -webkit-writing-mode: vertical-lr;
  -        -ms-writing-mode: vertical-lr;
    }

# Times To practices

- .google-logo{
-        width: 100px;
-         height: 100px;
-        border: 1px solid black;

}

- img{
-      width: 100%;
-      height: 100%;
-     object-fit: cover;
-     vertical-align: middle; */
-     Uncomment the following line to apply a filter effect */
-     filter: grayscale(100%);   */
  }
- .google-logo:hover{
-     transform: scale(1.1); */
-     transition: transform 0.3s ease; */
-     opacity: 0.8; */
-     Uncomment the following line to apply a filter effect */
-     filter: brightness(0.8); */
  }

> # Font Face Tutorials

- #### source font vazir-font : https://github.com/rastikerdar/vazirmatn?tab=readme-ov-file

- ## Local
- 1- local impeliment in your computer

````css

  @font-face {
    font-family: 'Vazirmatn';
    src: url('fonts/webfonts/Vazirmatn[wght].woff2') format('woff2 supports variations'),
    url('fonts/webfonts/Vazirmatn[wght].woff2') format('woff2-variations');
    font-weight: 100 900;
    font-style: normal;
    font-display: swap;
  }
  ````
 


- ## CDN

 
 

 -    2- CDN impliment without Downloadin in your computer.Means your fonts download from internet

````css

 @font-face {
  font-family: 'Vazirmatn RD';
  src: url('https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Round-Dots/fonts/webfonts/Vazirmatn-RD[wght].- woff2') format('woff2 supports variations'),
  url('https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Round-Dots/fonts/webfonts/Vazirmatn-RD[wght].woff2') format('woff2-variations');
  font-weight: 100 900;
  font-style: normal;
  font-display: swap;
 }
```



````
- ### Notice : this is very importany UX 
>  **__font-display__: swap** 
- in CSS is a property that controls how a web font is displayed while it's loading. 
- When set to swap, it instructs the browser to immediately display text using a fallback font. 
- while the custom web font is being downloaded. 
- Once the custom font is loaded, the browser swaps it in, 
- replacing the fallback font. This approach prioritizes immediate content visibility, 
- preventing the "flash of invisible text" (FOIT) that can occur when a custom font takes time to load, 
- and instead offers a "flash of unstyled text" (FOUT) as the fallback font is used initially. 

------------------------------------------------------------------------------------



