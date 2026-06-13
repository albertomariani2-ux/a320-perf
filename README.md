# a320-perf
Takeoff performance & climb/descent planner for the FlyByWire A32NX on Microsoft Flight Simulator.
🛫 Live app — funziona da browser, mobile-friendly, usabile come EFB su tablet.
🇮🇹 Italiano
Cos'è
Un piccolo tool web in stile EFB/FCOM per pianificare i tuoi voli sul FlyByWire A32NX (Airbus A320neo, motori LEAP-1A). Calcola le V-Speeds di decollo, la FLEX temp, il THS trim e i punti TOC/TOD del piano di volo.
Pensato per simmer che vogliono procedure più realistiche e CRM accurato, senza dover scaricare app esterne o ricordare a memoria le formule.
Funzioni
Tab "V-Speeds" — Performance di decollo:
V1, VR, V2 (IAS in kt) calcolate da TOW, configurazione flap, PA, OAT, anti-ice, packs
FLEX TEMP auto-calcolata con la formula derata standard, override manuale ±1 °C dal display
THS trim automatico da CG % MAC con direzione UP/DN
Toggle Anti-Ice (ENG+WING) e Packs ON/OFF con compensazione automatica
ΔISA visualizzato in tempo reale
Tab "CLB · DES" — Pianificazione climb/descent:
TOC (Top of Climb): distanza e tempo basati su GS climb e ROC medio
TOD (Top of Descent): calcolo con regola 3:1 + angolo personalizzabile (default 3°) + buffer NM
ROD (rate of descent) automatica
Profilo configurabile: cruise FL, dep/dest elevation, GS, angolo
Interfaccia
Estetica cockpit/EFB in stile Airbus: sfondo scuro, glow ambra/verde/magenta/ciano, font monospace Share Tech Mono. Layout responsive ottimizzato per smartphone e tablet in modalità ritratto.
Single file HTML statico (~35 KB), nessuna dipendenza, funziona offline una volta caricato.
Note tecniche
Costanti calibrate per A320neo / LEAP-1A, OEW 42.6t / MTOW 79.0t
Formule semplificate in stile FCOM, non basate su tabelle ufficiali Airbus
Configurazioni supportate: 1+F, 2, 3
Range CG: 17–40 % MAC
FLEX range: 55–75 °C (warning sopra 70 °C TMAX NORMAL)
⚠️ Disclaimer
Solo per uso in simulazione. Non utilizzare per operazioni reali. Le formule sono approssimazioni didattiche calibrate empiricamente per il FlyByWire A32NX, non riflettono la performance reale dell'A320neo né rispettano i requisiti AFM/FCOM Airbus.
🇬🇧 English
What is it
A web-based EFB-style performance tool for the FlyByWire A32NX (Airbus A320neo, LEAP-1A engines) on Microsoft Flight Simulator. Computes takeoff V-Speeds, FLEX temperature, THS trim, and climb/descent planning points.
Built for simmers who want more realistic procedures and accurate CRM without external apps.
Features
V-Speeds tab — takeoff performance:
V1, VR, V2 (IAS, kt) from TOW, flap config, pressure altitude, OAT, anti-ice, packs
FLEX TEMP auto-calculated with derated standard formula; manual override ±1 °C
THS trim auto from CG % MAC with UP/DN direction
Anti-Ice (ENG+WING) and Packs toggles with automatic compensation
Real-time ΔISA display
CLB · DES tab — climb/descent planning:
TOC (Top of Climb): distance & time from GS climb and average ROC
TOD (Top of Descent): 3:1 rule with custom angle (default 3°) + NM buffer
Automatic ROD (rate of descent)
Configurable profile: cruise FL, dep/dest elevation, GS, descent angle
Interface
Cockpit/EFB aesthetic in Airbus style: dark background, amber/green/magenta/cyan glow, Share Tech Mono font. Responsive layout optimized for phone and tablet in portrait mode.
Single static HTML file (~35 KB), no dependencies, works offline after first load.
Tech notes
Constants calibrated for A320neo / LEAP-1A, OEW 42.6t / MTOW 79.0t
Simplified FCOM-style formulas, not based on official Airbus tables
Supported configurations: 1+F, 2, 3
CG range: 17–40% MAC
FLEX range: 55–75 °C (warning above 70 °C TMAX NORMAL)
⚠️ Disclaimer
For simulation use only. Do not use for real-world operations. Formulas are empirically calibrated educational approximations for the FlyByWire A32NX, and do not reflect real A320neo performance or comply with Airbus AFM/FCOM requirements.
🚀 How to use
Open albertoa320-perf.netlify.app in any browser
Add to home screen on mobile for an EFB-like experience (icon included)
Enter your TOW, CG, PA, OAT before takeoff
Read V-Speeds, FLEX, THS directly
Switch to CLB · DES tab for the climb/descent profile
💡 Feedback & contributions
This is a personal project shared with the simmer community. Suggestions, bug reports, and pull requests are welcome via GitHub Issues.
If you find it useful, please share with other A32NX pilots! ✈️
Made with ☕ by Alberto Mariani for the FlyByWire community.
