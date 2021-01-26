# c172-xpndr
SIM Cessna 172 - Transpondeur Bendix King KT 76C - DIY
<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/bendix-KT76C.jpg' />
<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/bendix-KT76C-back.jpg' />
<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/xpndr-with-mega2560R3-bottom.png?raw=true' />
<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/xpndr-with-mega2560R3-left.png?raw=true' />
<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/xpndr-with-mega2560R3-top.png?raw=true' />

Build your own transponder for simulation cockpit cessna 172.<BR />
Format 159x41 mm for 6.25" stack<BR />
Electronics are design with EasyEDA.<BR />
3D parts are design with SolidWorks.<BR />

PCB are sold by JLCPCB, you can use directly Gerber files --> <a href='https://jlcpcb.com/'>JLCPCB</a><BR />

Only electronics, you can choose the microcontroller of your choice, the base design have addtionnal card for Mega2560R3.

For mine i use Mega2560R3 and Mobiflight on MSFS2020--> <a href='https://www.mobiflight.com/en/index.html'>MOBIFLIGHT</a><BR />
For others controllers you need to design the support for the card, or add wires to link them.
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/C172-XPNDR-shematics.png" />
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/PCB.png" />

Capacitor C3 to C18 are optionnals, they just do debounce for switch, but work fine wihtout on mobiflight.<BR/>

Parts list:

MAX7219 x1 --> <a href='https://fr.aliexpress.com/item/32874536319.html?spm=a2g0s.9042311.0.0.27426c37hpiJs6'>Aliexpress</a><BR />
Selector 2P6T x1 --> <a href='https://fr.aliexpress.com/item/32949497961.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
Screen 7 Seg 4 digits x2 --> <a href='https://fr.aliexpress.com/item/32673704841.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
Switch 8x8m x11 --> <a href='https://fr.aliexpress.com/item/32467872702.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
LED red 3mm x2 --> <a href='https://fr.aliexpress.com/item/4000968613440.html?spm=a2g0o.productlist.0.0.7b686c77RyIwIB&algo_pvid=null&algo_expid=null&btsid=2100bdcf16100179468078167e6eca&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Capacitor 10nF x16--> <a href='https://fr.aliexpress.com/item/32971478818.html?spm=a2g0o.productlist.0.0.48e15dd8AisfZd&algo_pvid=null&algo_expid=null&btsid=2100bdcf16100180514308589e6eca&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a>
<a href='https://fr.aliexpress.com/item/32896781515.html?spm=a2g0o.productlist.0.0.7c694ce4mS4BPk&algo_pvid=e0f06b71-fe57-450c-a420-fcb50ef3a8af&algo_expid=e0f06b71-fe57-450c-a420-fcb50ef3a8af-0&btsid=2100bde116116496357541685ee74a&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
High Frequency Low ESR Aluminum Capacitor 22µF 50V x1 --> <a href='https://www.aliexpress.com/item/33030332216.html?spm=a2g0o.productlist.0.0.12d330a9jR84Fg&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100182886983809e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Capacitor 0.15µF x1 --> <a href='https://fr.aliexpress.com/item/32719073307.html?spm=a2g0o.productlist.0.0.5a29ffee2lW9PU&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100185559405052e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Resistor 1/4W 10k&#x2126; x1<BR />
Resistor 1/4W 10k&#x2126; x2<BR />
Header male angle 2x15pin x1 --> <a href='https://fr.aliexpress.com/item/33043163402.html?spm=a2g0o.productlist.0.0.20038875rufBHE&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100186293925166e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Header female 2x15pin x1<BR />
Header female 1x6pin x4 (for 7 segment) --> <a href='https://fr.aliexpress.com/item/4000106121057.html?spm=a2g0s.9042311.0.0.584d6c374vkTRE'>aliexpress</a><BR />

<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/images/C172-XPNDR-3D.png' /><BR />
<table>
<tr>
	<th>PIN mega2560 R3</th><th>PIN Header H1</th><th>Device</th>
</tr>
<tr>
	<td>5V</td><td>1</td><td>--</td>
</tr><tr>
	<td>22</td><td>2</td><td>U1 - DIN (LCD)</td>
</tr><tr>
	<td>23</td><td>3</td><td>U1 - CLK (LCD)</td>
</tr><tr>
	<td>24</td><td>4</td><td>U1 - LOAD (LCD)</td>
</tr><tr>
	<td>25</td><td>5</td><td>SW1 - mode off</td>
</tr><tr>
	<td>26</td><td>6</td><td>SW1 - mode standby</td>
</tr><tr>
	<td>27</td><td>7</td><td>SW1 - mode test</td>
</tr><tr>
	<td>28</td><td>8</td><td>SW1 - mode on</td>
</tr><tr>
	<td>29</td><td>9</td><td>SW1 - mode alt</td>
</tr><tr>
	<td>30</td><td>10</td><td>SW2 - IDT</td>
</tr><tr>
	<td>31</td><td>11</td><td>SW3 - CLEAR</td>
</tr><tr>
	<td>32</td><td>12</td><td>SW4 - VFR</td>
</tr><tr>
	<td>33</td><td>13</td><td>SW5 - 0</td>
</tr><tr>
	<td>34</td><td>14</td><td>SW6 - 1</td>
</tr><tr>
	<td>35</td><td>15</td><td>SW6 - 2</td>
</tr><tr>
	<td>36</td><td>16</td><td>SW6 - 3</td>
</tr><tr>
	<td>37</td><td>17</td><td>SW6 - 4</td>
</tr><tr>
	<td>38</td><td>18</td><td>SW6 - 5</td>
</tr><tr>
	<td>39</td><td>19</td><td>SW6 - 6</td>
</tr><tr>
	<td>40</td><td>20</td><td>SW6 - 7</td>
</tr><tr>
	<td>41</td><td>21</td><td>LED D1 on/off</td>
</tr><tr>
	<td>42</td><td>22</td><td>LED D2 mode alt</td>
</tr><tr>
	<td>-</td><td>23</td><td>not use</td>
</tr><tr>
	<td>-</td><td>24</td><td>not use</td>
</tr><tr>
	<td>-</td><td>25</td><td>not use</td>
</tr><tr>
	<td>-</td><td>26</td><td>not use</td>
</tr><tr>
	<td>-</td><td>27</td><td>not use</td>
</tr><tr>
	<td>-</td><td>28</td><td>not use</td>
</tr><tr>
	<td>-</td><td>29</td><td>not use</td>
</tr><tr>
	<td>GND</td><td>30</td><td>GND</td>
</tr>
</table>
<H2>3D Printing</H2>
<H3>Materials</H3>
- HEAD : 0.2mm and 0.6mm<BR />
- PLA BLACK and PLA WHITE<BR />
<H3>CURA  configuration</H3>
With CURA you need plugin PauseAtZ, i modified the plugin to add 2 pauses (printing buttons by example) download and install it--> <a href='https://github.com/kkr0kk/c172-autopilot/blob/main/Gcode/pauseAtZ.py'>Here</a><BR />
TEXT is printing with this technics --> https://www.youtube.com/watch?v=jnYfF_O7INk
STL files with text is ready for print directly, the text layer are 0.3mm layer, add a pause a 0.31mm that you can change the color and drop down the head by one click directly on the motor and resume the print

<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/chassis.png" />

<H2>SUPPORT for controller</H2>
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/support%20mega2560R3.png" />
<H3>Support for mega 2560 R3</H3>
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/support%20mega%202560%20R3%20-%20sh%C3%A9matic.png" />
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/support%20mega%202560%20R3%20-%20PCB.png" />
<H3>Support for mega 2560 pro mini</H3>
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/support_mega2560-pro-mini_PCB.png?raw=true" />
<H3>Adaptateur for 195x55 mm mount with front screws</H3>
<img src="https://github.com/kkr0kk/c172-xpndr/blob/main/images/adaptateur.png" /><BR />
<H2>Other Projects</H2>
Build AutoPilot KAP140 for Cessna172 -> <a href='https://github.com/kkr0kk/c172-autopilot'>AutoPilot</a><BR />

