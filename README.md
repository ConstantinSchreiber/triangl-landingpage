# triangl-landingpage
WS2018- ID_19 — Responsive Design - Assessment Submission by Constantin Schreiber

### Assets
- **Sketch File (Handed in via Google Form)**
- **GitHub repo containing the source files**
- **Live Version: https://triangl.io/ (Backup: http://triangl.cschreiber.io/)**

## Roadmap
The process can mainly be divided into three steps. Conception, Screen Design & Implementation.

### Conception
Against the current trend I actively decided to not develop mobile but rather desktop first because from a practical standpoint our customers being from the enterprise sector we reasoned they would most likely see the desktop version with a significantly higher probability. Because a desktop screen size has less boundaries in terms of creative freedom.  

| <img src="https://i.imgur.com/XpwXNMU.jpg" width="200"> | <img src="https://i.imgur.com/wIrnARB.jpg" width="200"> | <img src="https://i.imgur.com/DDbVdjJ.jpg" width="200"> |
|:---:|:---:|:---:|



### Screen Design
When implementing the design in sketch I tried to already think in grids to be able to adapt to smaller screen sizes more natrually.
<img src="https://i.imgur.com/g7566dW.png" width="200"> 

### Implementation

As the landingpage does not contain complex logic or will be subject to constant change in the future, I choose to develop the page without any JS framework or the like.<br/>
#### Structure
I used **SASS** as a precompiler for CSS to enable more advanced css syntax and easier structuring of files.<br/>
For structuring the files I used a slightly adapted version of the **7-1 Pattern** and tried to follow the **BEM** naming scheme as closly as possible.<br/>
<br/>
Altough browser compatibility has gotten way better for flexbox and css-grid, I choose to stick with the grid / float approch for creating the responsiveness of the website. Therefore I defined six breakpoints as a mixin. Another vital component plays the four column grid I created in ```/sass/layout/_grid.scss```.<br/>
<br/>
To help with fluidity I tried to use relative lengths wherever possible instead of absolute ones.
 
 #### Building
 While developing I used a npm package called 'live-server' and a SASS watcher to compile css and rerender the page on every change automatially.<br/>
 </br>
 For deployment I additionally used a autoprefixer to add vendor prefixes to css in order to ensure maximum browser compatabiliy. Last but not least I minified the production code to optimize loading speed.
