# Funktionierendes Portal Radio (remix von [@AIBot | MyMiniFactory](https://www.myminifactory.com/object/3d-print-portal-radio-50006) (GERMAN)

## Vorwort
Zunächst ein Dank an:
: @Aibot für die Druckdateien
: @Astro_Flora für das Drucken von “Shell” und “Bottom” mit seinem Bambu Lab X1C 
: @monion für das Helfen mit dem Code (er ist nicht verantwortlich für den endgültigen Code ;D )
: @Chair Gaming für allgemeine Hilfe

Hinweis: 
Hier kannst du nur meine modifizierten Teile herunterladen. Bitte lade das komplette Projekt vom Original-Autor herunter! 
[**https://www.myminifactory.com/object/3d-print-portal-radio-50006**](https://www.myminifactory.com/object/3d-print-portal-radio-50006)
  
## Allgemeine Informationen
  
**HIER KANNST DU NUR MEINE MODIFIZIERTEN PARTS HERUNERLADEN, BITTE LADE DAS KOMPLETTE PROJEKT VOM ORIGIALEN AUTOR HERUNTER!**  
  
Für die Elektronik habe ich mich an einer Anleitung für ein DIY-Radio von AZ-Delivery orientiert und es so angepasst, wie es für mich passt: [https://www.az-delivery.de/products/internet-radio-mit-dem-esp32](https://www.az-delivery.de/products/internet-radio-mit-dem-esp32).

Verwendete Drucker:

-   **Bambu Lab X1C und Bambu Lab A1 Mini**
-   „Shell“ und „Base“ wurden mit dem Bambu Lab X1C gedruckt, können aber auch mit dem Bambu Lab A1 gedruckt werden. Beide haben eine Druckfläche von 256x256x256 mm.
-   Kleinere Teile wurden mit dem Bambu Lab A1 Mini (Druckfläche 180x180x180 mm) gedruckt.

### Bekannte Probleme
Da dies mein erstes Projekt ist, kenne ich mich mit der verwendeten Mikroelektronik noch wenig aus. Ein nerviges Problem ist der DFPlayer. Beim Einschalten gibt er ein Störgeräusch von sich, bevor er den Song abspielt. Auch während des Songs ist ein leises, aber hörbares Störgeräusch vorhanden, insbesondere bei geringer Lautstärke. Bis jetzt habe ich dafür noch keine Lösung gefunden.
Wenn man den Verstärker PAM8403 bis ganz an Ende zu dem Rastpunkt dreht und ihn dann wieder aufdreht Startet der Arduino aus unbekannten gründen neu. Ich habe das Problem bissher noch nicht behoben und habe bissher auch noch keinen Lösungsansatz.
  
## Das Portal Radio
![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Portal%20Radio%20Front.jpg?raw=true)![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Portal%20Radio%20Back.jpg?raw=true)


### Funktion
  
Das Radio soll folgende Funktionen erfüllen:

-   Beim Einschalten leuchten die LEDs am Ring blau auf, die 7-Segment-Anzeige zeigt „85.2“ an, und die Radiomusik aus dem Spiel beginnt zu spielen.
-   Die blaue LED an der Front leuchtet, sobald der Code „hochgefahren“ ist, als Indikator.
-   Über einen Drehregler kann die Lautstärke eingestellt werden. Weitere Funktionen wie Songauswahl und Frequenzeinstellung sind geplant.
  
### Teileliste
  
Hier sind die Teile die ich für das Radio gekauft habe, eine Mischung vom Amazon und AliExpress:  
  
-[7 Segment Anzeige TM1637 Blau](https://www.amazon.de/dp/B09X1Z8CC8?ref=ppx_yo2ov_dt_b_fed_asin_title)  
-[USB Typ C Batterielademodul TP4056](https://amzn.eu/d/bJx8FN1) [¹]
-[Step Up Module MT3608](https://amzn.eu/d/h4YCcV0)  
-[AZ Delivery Mikrocontroller AZ-ATmega 328](https://amzn.eu/d/12fmeU2)  
-[2x AZ Delivery DFPlayer Mini 3 Watt Lautsprecher](https://amzn.eu/d/aCnC54G)  
-[5mm LED Blau](https://amzn.eu/d/fTzluys)  
-[DFPlayer Mini](https://de.aliexpress.com/item/1005006181511315.html?)  
-[PAM8403 Audio Verstärker](https://de.aliexpress.com/item/1005006135778016.html)  
-[JST XH 2 Polig Kabelstecker](https://de.aliexpress.com/item/1005006577211209.html) [²] 
-[Wippschalter Rund](https://amzn.eu/d/0qvCGKB)  
-[verwendeter Akku](https://www.conrad.de/de/p/reely-modellbau-akkupack-lipo-3-7-v-1000-mah-zellen-zahl-1-30-c-bec-2582341.html) [³]

-[~350g PLA Schwarzes Filament](https://amzn.eu/d/ibRLTVA)
-[~265g PLA Weißes Filament](https://amzn.eu/d/6HExSpr)
-[~30g PLA Durchsichtiges Filament](https://amzn.eu/d/5HmzEyD)
-[~2g PETG Schwarzes Filament](https://amzn.eu/d/5IXwTd8)[⁴]
-Sekundenkleber (zum Ankleben der Elektronik so wie der LED's)
-Blechschrauben (zum Anschrauben der Elektronik)

[¹]: Vorsicht!, mit diesem Lademodul kann man nur mit einem USB A auf USB C Kabel laden, nicht mit einem USB C - USB C Kabel
[²]: um den Akku und die Lautsprecher abtrennbar zu machen, ich habe die Originalen Stecker der jeweiligen Komponenten abgeschnitten und diesen angelötet, schlauer wäre gewesen gleich den Richtigen Stecker zu bestellen aber egal ^^
[³]: alle Akkus die ich auf Amazon bestellt habe haben mit diesem Projekt nicht funktioniert. Der Akku war immer zu schwach und das Radio wurde bei hoher Lautstärke abgeschaltet. Deswegen der Reely Modellbauakku von Conrad.. eine Powerbank hätte es glaube ich auch getan
[⁴]: Das PETG Filament ist für das Aperture Logo vorne am Radio damit man es sieht. Man sieht es mit dem PETG Filament zwar, es kommt aber tatsächlich drauf an wie man drauf schaut. Aufällig ist es nicht also kann man dafür auch anderes Filament z.b. in einer anderen Farbe verwenden.

## 3D Druck 

### Info und änderungen
Abgeändert habe ich das *"front-panel"* damit das Display vorne rein passt so wie den *"top-button"* damit man den Knopf oben für die Lautstärke drehen kann und das der Audio Verstärker PAM8403 da Perfekt reinpasst. Diese änderungen kannst du hier auf GitHub herunterladen. 
Dadurch das ich das Display in das Radio Montiert habe müssen folgende Teile die du von Aibot auf MMF herunterlädtst nicht gedruck werden:
- "ledholder-screen"
- "screen-main"
- "screen-8-top"
- "screen-8-bot"

Außerdem habe ich "electronics-mount" und "front-logo-stencil-1" nicht gedruckt. Das Front Logo habe ich so angepasst das der Drucker das Logo mit vorne rein druckt. Aibot hat denke ich vorgesehen das man das Logo vorne Dransprüht mit dem "front-logo-stencil-1".

### Druckereinstellungen
Die Druckeinstellungen basieren alle auf **Bambu Studio**.

-   **0,20 mm Standardprofil**, 15 % Fülldichte, Gitternetz-Füllmuster, Wandlinien: 2, Schichthöhe: 0,2 mm, keine Supports (außer für „Shell“).
![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Default%20Print%20Settings.png?raw=true)

### Base

Für die Base habe ich "base" genommen und nicht "base-with-holes-for-electronics-mount" da ich meine eigene Elektronik eingebaut habe.
Folgende Druckeinstellungen habe ich bei der Base geändert:

- Fülldichte: 35 %, Füllmuster: Geradlinig, Wandlinien: 4 (für besseren Halt der Schrauben). 

![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Print%20Settings%20Base.png?raw=true)

### Shell
Die Shell muss mit Supports gedruckt werden. Verwendet wurden die Supports "Baum". 
Bei der Druckbetthaftung habe ich die Schürzenschlaufen auf 5 und die Nahtposition auf zufällig. 

![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Print%20Settings%20Shell.png?raw=true)

### Zusammenbau
Nachdem alles gedruckt wurde sollte man 10 einzelne Teile vor sich liegen haben
- "base"
- "shell"
- "antenne-holder"
- "grill-left"
- "grill-right"
- "led-ark"
- "led-ark-diffuser"
- "led-ring"
- "[front-panel](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Modified%203D%20Print%20Parts/front-panel-modified-for-displayl.stl)" (meine geänderte Version)
- "[top-button](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Modified%203D%20Print%20Parts/top-button-modified-for-PAM8403.stl)" (meine geänderte Version)

An sich sollte es sich fast von selber erklären wie das Radio zusammengebaut wird. 
"base" und "shell" werden miteinander verschraubt, ich habe eine M3 Mutter in die "shell" geklebt und mit einer M3x8 Schraube verbinde ich dann "base" und "shell" auch so das es einfach wieder geöffnet werden kann.

"antenne-holder" habe ich an die "shell" angeklebt
"top-button" habe ich auch an die "shell" angeklebt
"grill-left" und "grill-right" habe ich an "front-panel" angeklebt 
"led-ring" habe ich auch an "front-panel" angeklebt
"led-ark" habe ich in die dafür vorgesehenen löcher in der "base" mit blechschrauben eingeschraubt nachdem ich die LED's in die "led-ark" eingeklebt hatte. Ich habe nicht alle löcher vom "led-ark" mit LED's gefüllt, ich habe nur jedes zweite Loch verwendet und es ist trozdem hell genug. Auch habe ich erst alle LED's Parallel zusammengelötet bevor ich die ark in die Base eingeschraubt habe.

Die Löcher für den ein/aus Schalter so wie das Loch für den Poti hinten und den Ladeport habe ich je nach Position reingebohrt. 


## Die Elektronik

### Schaltplan
Wie bereits am anfang erwähnt, habe ich die Elektronik von einer DIY Anleitung für ein Internetradio von AZ Delivery abgeschaut. Aber bevor ich die Elektronik verdrahtet und einegabut habe, habe ich mit der Software **Fritzing** einen Schaltplan erstellt den ich euch hier zur verfügung stelle. 

![Alt](https://github.com/MrTiiv/Portal-Radio-Doku-German/blob/main/Bilder%20f%C3%BCr%20Doku/Portal%20Radio%20Sketch%20V0.1%20Schematic.png?raw=true)
> VORSICHT! Bei der Programmierung des DFPlayers ist RX und TX wieso auch immer gedreht.
z.b. **`SoftwareSerial mySoftwareSerial(11, 10); // RX, TX`** funktioniert nicht du musst
 **`SoftwareSerial mySoftwareSerial(10, 11); // RX, TX`** verwenden
Also **RX = TX** und **TX = RX** (wieso auch immer?)

Der Schaltplan ist 1:1 zu meinem jetzigen Portal Radio.
Das Step Up Module muss VOR dem einbauen eingestellt werden. Ich habe die ganze Elektronik gelötet, das Step Up Module hätte ich genau so wie den Akku und die Lautsprecher Steckbar machen sollen falls das Modul nochmal nachgestellt werden muss. Die Spannung habe ich mit Wago 221 Klemmen verteilt die ich auf der Base aufgeklebt habe (please don't judge me)

### Das einbauen der Elektronik

An sich gibt es keine feste Position für die Elektronik, das muss man am ende selbst entscheiden.
Ich habe den Charger und das Step-Up Module mit kleinen abstandshaltern wegen den Lötpunkten an der Base mit Sekundenkleber festgeklebt.
Die LED's habe ich mit jeweils einem kleinen tropfen Sekundenkleber in den led ring geklebt.
Den Arduino habe ich auch mit einem kleinen abstandshaltern mit Blechschrauben festgeschraubt.
Für den DFPlayer habe ich eine kleine Platte gedruckt die etwas länger ist als der DFPlayer um den DFPlayer mit zwei Blechschrauben zu befestigen. Die Platte hält den DFPlayer sogesehen fest.
Die 7 Segment anzeige habe ich in das von mir geänderte Front Panel eingeschraubt.
Die Lautsprecher habe ich schräg in das Front Panel eingeschraubt damit die Membranen sogesehen durch den "grill-left" und "grill-right" hindurchschauen.

### Der Code
Den Code stelle ich hier zur vefügung, sobald er soweit ist. Der Code der gerade auf dem Arduino läuft ist eigentlich nur ein Test Code und ich glaube jeder der sich mit dem Arduino auskennt würde mich umbringen dafür :D (aber es funktioniert)

Beim Code schreibe ist nur das zu beachten, was ich oben unter den Schaltplan geschrieben habe, sonst funktioniert es nicht.

> VORSICHT! Bei der Programmierung des DFPlayers ist RX und TX wieso auch immer gedreht.
z.b. **`SoftwareSerial mySoftwareSerial(11, 10); // RX, TX`** funktioniert nicht du musst
 **`SoftwareSerial mySoftwareSerial(10, 11); // RX, TX`** verwenden
Also **RX = TX** und **TX = RX** (wieso auch immer?)

## Schlusswort
Ich hoffe diese Dokumentation hilft beim nachbau des Portal Radios. Das Radio ist ein wirklicher Hingucker und das es den Radiosong abspielt macht es noch um einiges cooler.

Fragen oder Anregungen gerne auf GitHub, Discord (MrTiiv), [Instagram](https://www.instagram.com/mrtiiv/), [Steam](https://steamcommunity.com/id/MrTiiv).

 >This was a triumph  
I'm making a note here; "Huge success"

