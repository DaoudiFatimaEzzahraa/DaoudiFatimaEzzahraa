<svg width="1600" height="450"
xmlns="http://www.w3.org/2000/svg">

<defs>

<linearGradient id="bg" x1="0" y1="0" x2="0" y2="1">
<stop offset="0%" stop-color="#0b1025"/>
<stop offset="100%" stop-color="#05070f"/>
</linearGradient>

<linearGradient id="purple">
<stop offset="0%" stop-color="#7d5fff"/>
<stop offset="100%" stop-color="#00d4ff"/>
</linearGradient>

<filter id="glow">
<feGaussianBlur stdDeviation="5"/>
</filter>

</defs>

<rect width="1600" height="450" fill="url(#bg)"/>

<!-- Stars -->

<g fill="#ffffff">

<circle cx="200" cy="50" r="2">
<animate attributeName="opacity"
values="0;1;0"
dur="2s"
repeatCount="indefinite"/>
</circle>

<circle cx="600" cy="80" r="2">
<animate attributeName="opacity"
values="1;0;1"
dur="3s"
repeatCount="indefinite"/>
</circle>

<circle cx="900" cy="60" r="2">
<animate attributeName="opacity"
values="0;1;0"
dur="4s"
repeatCount="indefinite"/>
</circle>

<circle cx="1300" cy="70" r="2">
<animate attributeName="opacity"
values="1;0;1"
dur="2.5s"
repeatCount="indefinite"/>
</circle>

</g>

<!-- Rain -->

<g stroke="#6C63FF55">

<line x1="100" y1="-50" x2="90" y2="20">
<animateTransform
attributeName="transform"
type="translate"
from="0 0"
to="0 520"
dur="1.2s"
repeatCount="indefinite"/>
</line>

<line x1="400" y1="-150" x2="390" y2="-80">
<animateTransform
attributeName="transform"
type="translate"
from="0 0"
to="0 620"
dur="1s"
repeatCount="indefinite"/>
</line>

<line x1="800" y1="-100" x2="790" y2="-30">
<animateTransform
attributeName="transform"
type="translate"
from="0 0"
to="0 600"
dur="1.4s"
repeatCount="indefinite"/>
</line>

<line x1="1200" y1="-120" x2="1190" y2="-40">
<animateTransform
attributeName="transform"
type="translate"
from="0 0"
to="0 650"
dur="1.1s"
repeatCount="indefinite"/>
</line>

</g>

<!-- City -->

<g fill="#111a35">

<rect x="0" y="240" width="80" height="210"/>
<rect x="120" y="180" width="100" height="270"/>
<rect x="280" y="120" width="90" height="330"/>
<rect x="430" y="170" width="120" height="280"/>
<rect x="620" y="90" width="80" height="360"/>
<rect x="760" y="150" width="120" height="300"/>
<rect x="930" y="100" width="100" height="350"/>
<rect x="1090" y="140" width="90" height="310"/>
<rect x="1260" y="170" width="120" height="280"/>
<rect x="1450" y="110" width="100" height="340"/>

</g>

<!-- Hologram -->

<circle cx="800" cy="170"
r="70"
fill="none"
stroke="url(#purple)"
stroke-width="3">

<animateTransform
attributeName="transform"
type="rotate"
from="0 800 170"
to="360 800 170"
dur="20s"
repeatCount="indefinite"/>

</circle>

<circle
cx="800"
cy="170"
r="90"
fill="none"
stroke="#6C63FF44"/>

<text
x="800"
y="190"
text-anchor="middle"
font-size="90"
font-family="Arial"
font-weight="bold"
fill="white">

FD

</text>

<!-- Name -->

<text
x="800"
y="315"
text-anchor="middle"
font-size="46"
fill="white"
font-family="Arial">

FED

</text>

<text
x="800"
y="350"
text-anchor="middle"
font-size="18"
fill="#8fb9ff"
font-family="Arial">

Building Intelligent Systems

</text>

<!-- Status -->

<rect
x="1220"
y="40"
rx="12"
width="300"
height="150"
fill="#111827"
stroke="#6C63FF"/>

<text
x="1250"
y="75"
fill="#ffffff"
font-size="24"
font-family="monospace">

SYSTEM STATUS

</text>

<text
x="1250"
y="110"
fill="#00ff88"
font-family="monospace">

AI Core ● ONLINE

</text>

<text
x="1250"
y="140"
fill="#66ccff"
font-family="monospace">

Creativity ████████

</text>

<text
x="1250"
y="170"
fill="#ff66ff"
font-family="monospace">

Bug Counter 0

</text>

</svg>
