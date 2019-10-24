# Vaja7-PWM-Nucleo
Kontroliranje PWM z Nucleo L476RG

<h3>Kateri pin ste omogočili, kaj se izpiše poleg pina?</h3>
<p>Omogočila sva pin PA8. Poleg omogočenega pina se izpiše TIM1_CH1.</p>

<h3>Koliko je vreden prescaler?</h3>
<p>Prescaler sva nastavila na 16, da sva dobila 1MHz frekvenco.</p>

<h3>Koliko znaša takt časovnika?</h3>
<p>Takt časovnika sedaj znaša 10kHz</p>

<h3>Kaj pomeni parameter Generation Channel pulse?</h3>
<p>Vrednost širine pulza. Nastavimo ga na 50%.</p>

<h3>V kodi spremenite vrednost širine pulza ba 25%, zapišite popravljen ukaz</h3>
<p>sConfigOC.Pulse = 25; </p>

<h3>Zapišite kaj počnejo ukazi v 1., 2. in 3. vrstici</h3>
<p>1)Na začetku zanke program nastavi htim1.Instance->CCR1 na vrednost spremenljivke dutyCycle.</p>
<p>2) Vsakič ko program loopa skozi to vrstico doda spremenljivki dutyCycle + 10. </p>
<p>3) Preveri, če je vrednost dutyCycle-a večja od 90, če je potem nastavi dutyCycle nazaj na 10, kar pomeni
da je to neskončna zanka.</p>

<p>Ustvarila Nik Vogrinec in Luka Voje</p>
