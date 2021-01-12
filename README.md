# c172-xpndr
SIM Cessna 172 - Transpondeur

Build your own transponder for simulation cessna 172.<BR />
Electronics are design with EasyEDA.<BR />
3D parts are design with SolidWorks.<BR />

Only electronics, you can choose the microcontroller of your choice, the base design have addtionnal card for Mega2560R3.

For mine i use Mega2560R3 and Mobiflight --> <a href='https://www.mobiflight.com/en/index.html'>MOBIFLIGHT</a>
For others controllers you need to design the support for the card, or add wires to link them.

Parts list:

MAX7219 x1 --> <a href='https://fr.aliexpress.com/item/4001027015865.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
Selector 2P6T x1 --> <a href='https://fr.aliexpress.com/item/32949497961.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
Screen 7 Seg 4 digits x2 --> <a href='https://fr.aliexpress.com/item/32673704841.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
Switch x11 --> <a href='https://fr.aliexpress.com/item/32467872702.html?spm=a2g0s.9042311.0.0.338d6c379S0zX2'>Aliexpress</a><BR />
LED red 3mm x2 --> <a href='https://fr.aliexpress.com/item/4000968613440.html?spm=a2g0o.productlist.0.0.7b686c77RyIwIB&algo_pvid=null&algo_expid=null&btsid=2100bdcf16100179468078167e6eca&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Capacitor 10nF x16--> <a href='https://fr.aliexpress.com/item/32971478818.html?spm=a2g0o.productlist.0.0.48e15dd8AisfZd&algo_pvid=null&algo_expid=null&btsid=2100bdcf16100180514308589e6eca&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
High Frequency Low ESR Aluminum Capacitor 10µF 10V x1 --> <a href='https://www.aliexpress.com/item/33030332216.html?spm=a2g0o.productlist.0.0.12d330a9jR84Fg&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100182886983809e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Capacitor 0.1µF x1 --> <a href='https://fr.aliexpress.com/item/32719073307.html?spm=a2g0o.productlist.0.0.5a29ffee2lW9PU&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100185559405052e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />
Resistor 1/4W 1k&#x2126; x2<BR />
Resistor 1/4W 10k&#x2126; x1<BR />
Header male angle 30pin x1 --> <a href='https://fr.aliexpress.com/item/33043163402.html?spm=a2g0o.productlist.0.0.20038875rufBHE&algo_pvid=null&algo_expid=null&btsid=0b0a0ac216100186293925166e3a40&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_'>Aliexpress</a><BR />

<img src='https://github.com/kkr0kk/c172-xpndr/blob/main/C172-XPNDR-3D.png' /><BR />
<table>
<th>
	<td>PIN mega2560 R3</td><td>PIN Header H1</td><td>Device</td>
</th>
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
	<td>27</td><td>7</td><td>SW1 - mode</td>
</tr><tr>
	<td>28</td><td>8</td><td>SW1 - mode</td>
</tr><tr>
	<td>29</td><td>9</td><td>SW1 - mode</td>
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
</tr>
</table>
