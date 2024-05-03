# Ultrageluidsgolf
![[Pasted image 20240104053058.png|300]]

- $d$ = deflectie ($dB$)
- $A$ = amplitude ($dB/Pa$) ~ "E"
- $\lambda = c/f$
- $Power = A^2$
	- akoustische druk per tijdseenheid ($mJ/s$)
	- ↓ power -> ↑ diepte
	- ↑ power -> ↑ kwaliteit, ↑ risico biologische effecten
- $I = P/opp$ ("intensiteit = power/beam area")($mJ/s/cm^2$)
	- $I = p^2$
		- lage $I$ aan randen en einde van bundel
		- ruimtelijk gemiddelde intensiteit/piekintensiteit
	- attenuatie coëfficiënt = $\frac{1}{2}F_t \, (dB/cm)$
		- ↑attenuatie bij ↑$F_t$ of ↑diepte
		- lucht > bot >> weke delen > bloed
	- intensiteit halfwaarde diepte = $6 \, cm/F_t$
- Duty factor
	- DF = PD/PRP
	- DF = PD, PRF
		- ~ 0.0005 - 0.0002
	- in geval van PW gepulseerd
	- in geval van CW continue
# Toepassingen in de echografie
- TTE circa 1 - 7 MHz, volwassenen 2.5 - 5 MHz (intracoronair ~ 20 MHz)
- 2D echo beeld: pulsgewijs activatie kristallen en in specifieke volgorde (phased array)
	- object groter dan $\lambda$? -> reflectie
	- object kleiner dan $\lambda$? -> scattering
## sterkte echo's
- attenuatie: reductie signaalsterkte door:
	- diepte
	- power
	- frequentie
	- medium (b.v. lucht ++)
	- niet haaks treffen:
		- onregelmatigheid in ogenschijnlijk gladde structuren -> toch zichtbaar
## weergave echo's
- tijd tussen uitzenden en ontvangen blokje (~ 1540 m/s; apparaat op afgesteld) -> afstand
	- A-mode
	- B-mode (brightness)
	- M-Mode (tijd)
	- 3D
- reguleren "intensiteit" echo's:
	- overall gain factor control
	- time-gain-compensation (TGC; schuifjes)
	- reject control: filtert kleine echo's uit (ruis)
	- gray scale: hoe beter, hoe breder 'dynamic range' (dB): capaciteit van systeem om range van waardevolle echo's te registreren
		- m.n. relevant voor myocard & massa's
# Beeldkwaliteit
*1. transducerfrequentie*
- ↑frequentie -> ↑ resolutie, ↓ penetrantie
	- US > 20.000 Hz
	- TTE volwassenen 2-4 MHz
- transducers: bandbreedte
	- bandbreedte (MHz) = 1/PD ($\mu s$)
	  
*2. focus (lens/activatie kristallen)*
- diepte focus = $(ø_{kristal})^2/4\lambda$
  
*3. resolutie*
- axiale resolutie
	- ↑ bij ↑ F
	- ↓ bij ↑ PD (~ c)
	- ~ bandbreedte
- laterale resolutie
	- ↑ bij ↑ focus
	- ↓ bij ↑ diepte (bredere bundel)
	- ~ F en bandbreedte
- elevationele resolutie
	- ↑ bij ↑ kristaldikte
	- ↓ bij ↑ diepte
	- ↑ bij ↑ focus

*4. frame rate (≈ temporele resolutie)*
- n pulsen beschikbaar per seconde
	- ↑ F -> ↓ PRP -> ↑ PRF -> ↑ FR
	- ↑ diepte -> ↑ PRP -> ↓ PRF -> ↓ FR
- FR = PRF x aantal scan lines per frame
	- PRF = 1 / PRP
		- PRP = PD + luistertijd
			- PD = periode x aantal cycli in puls
- spatial pulse length = $\lambda$ x aantal cycli in puls

*5. pulse repitition frequency (aantal pulsen per seconde)*
- PRF = 1 / PRP
	- PRF = c / 2x diepte (klopt?)
- aantal pulsen per seconde:
	- 4 MHz transducer: 61
	- 5 MHz transducer: 72
## Beeldartefacten
- side lobes: ++ echogene structuren in side lobes (↓ laterale resolutie)
	- dicht bij transducer
	- voorbij focuspunt
	- vb'en: pacemakerdraad in LA, closure device ASD in LA
- revertebraties (=spiegel artefact)
	- ++ echogeen oppervlak 2x weerkaatst echo's van andere structuren
		- vb: mitralisklep áchter pericard b.v.
	- óók twee echogene lagen dicht bij elkaar: revertebrations (engelse definitie)
- shielding/shadowing
	- ++ echogene structeren
		- soms ook mee in zijwaartse sectorrichting
- refractie
	- structuur 2x zichtbaar naast elkaar
		- bundel afgebogen (b.v. dubbele RA/RV wand)
- near field clutter
	- oscillaties met ++ amplitude, DD trombus
		- to do: 
			- ↑ frequentie transducer
			- goede focus
			- second harmonic imaging
## Second harmonic imaging
- second harmonic doorgelaten -> vanaf 6 cm pas zinvol
	- voordeel: 
		- ↑ resolutie EN ↑ penetrantie
		- ↑ laterale resolutie
	- nadeel:
		- ↓ axiale resolutie (relatief lage frequentie ontvang je ook)
- +/- contrast
# Doppler
## PW/CW Doppler
- aliasing = omkering signaal als Nyquist grens wordt bereikt
	- Nyquist frequentie ($F_N$)= PRF/2
		- Nyquist limiet = $F_N$ omgerekend naar snelheid
	- oplossing:
		- HPRF:
			- 2e sample-V op halve afstand tot transducer -> 2x zo vaak gesampeld 
				- nadeel: ↓ spatiële resolutie
- Doppler shift
	- $f_d = 2f_0 \frac{v \cdot cos \alpha}{c}$
		- $v = c \cdot f_d / 2f_{t} \cdot cos \alpha$
- Uit snelheid drukverschil!
	- $p_{1} - p_{2} = \frac{1}{2}\rho (v_{2}^{2} - v_{1}^{2}) + \rho \int^{2} dv/dt \cdot ds + R(v)$
		- $p_1$ = druk proximaal van stenose
		- $p_2$ = druk t.h.v. stenotisch ostium
		- $\frac{1}{2}\rho (v_{2}^{2} - v_{1}^{2})$ = convectieve acceleratie
		- $\rho \int^{2} dv/dt \cdot ds$ = flow accelaratie
		- $R(v)$ = viscositeit
	- in sterk vereenvoudigde vorm:
		- $p = 4v_{2}^2$
			- aannames:
				- viscositeit onbelangrijk
				- geen tubulaire stenose
				- geen seriële stenosen
				- $v_1$ is ongeveer 0
### Kleuren Doppler
- cave revertebraties en effecten side lobes
	- vb: +++ PI geprojecteerd op septumwand (lijkt op VSD)
- intensiteit, vorm en diepte afhankelijk van:
	- richting flow
	- flow - snelheid
	- diepte
	- tussenliggend weefsel
	- vorm van de jet
	- vlak van doorsnede
	- moment hartcyclus
	- onderzoeker
	- apparaat
		- gain
			- check buiten hartholtes: spikkeltjes? iets terugdraaien
		- Nyquist grens
			- to do:
				- reduceer sectorbreedte (↑ PRF)
				- reduceer diepte (↑ PRF)
				- reduceer F$_{t}$(?)
		- PRF
		- F$_t$
		- FR (↓ FR -> ↑ jet oppervlakte)
		- kleurenpersistence (↓ persistence -> ↓ jet oppervlakte)
## Tissue Doppler
- filter hoge snelheden: TDI
- TVI = tissue velocity imaging, kleur = mean peak velocities
	- belangrijke parameters: S' en E' 
	- + PW-Doppler (= spectrale Doppler) -> peak velociteies
- strain = relatieve verandering in dikte/lengte (lokaal, geen dimensie)
	- i.e. maat voor deformatie
- strain rate = $v$ relatieve verandering dikte/lengte
# Speckle tracking
- backscattering myocard: kwantificatie bewegingen
	- onafhankelijk van hoek!
# Color kinesis
- wandbewegingen deel myocard (b.v. endocard) volgen doorheen de tijd