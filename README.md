# oe-functies-herhaling-opl
Toepassing op programmeerstructuren en functies

**(!) In deze oefening heb je bijna uitsluitend anonieme functies nodig!**
## Doelstelling
In deze oefening worden een aantal oefeningen op lussen in een dynamische lay-out toegepast.
Naargelang de oefening worden er 1 of 2 textboxen getoond en wordt de code die uitgevoerd wordt bij een klik op de button met id `execute` gewijzigd.
Gebruik functions waar mogelijk om je code overzichtelijk en compact te houden.
## Functionaliteiten
### Opstarten
Voeg code toe aan: 
- `bindElements`: koppel alle DOM-elementen. Gebruik hiervoor de reeds gedeclareerde variabelen.
- `hideElements`: Alle controls onder de header met id `functionality` worden verborgen.
### eventListener die de info header aanpast bij een muisbeweging (+ resetten)
- Alle controls onder de header met id `functionality` worden verborgen. Dit kan je doen door gepaste CSS-klasse te schrijven.
- De input van de textboxen wordt gewist
- De tekst in de div met id `feedback` wordt gewist
- In de header met id `functionality` verschijnt de uitleg van de knop. Gebruik hiervoor de omschrijvingen uit de constanten die globaal gedeclareerd zijn.
### eventListener die de input-elementen en labels instelt bij een klik. (function `setInputElementsByFunctionality`)
- De tekst in de label(s) wordt aangepast:
    - Bij het klikken op de winstknop: er worden twee labels getoond met daarin de tekst 'aankoopprijs' en 'verkoopprijs'
    - Bij het klikken op de dierenknop: er wordt één label getoond met daarin de tekst 'Aantal huisdieren:'
    - Bij bij het klikken op de 'tafel van'-knop: er wordt één label getoond met daarin de tekst 'Tafel van:'
    - Bij klikken op de 'Tafels van ... tot ...'-knop: er worden twee labels getoond met daarin de tekst 'tafel van:' en 'tafel tot:'
- Er wordt een standaardwaarde ingevuld in de textboxen
### Winst: function `execute` en `getProfitMessage`
- De input van de twee textboxes wordt opgehaald
- Er wordt nagegaan of de input wel degelijk een getal is. Zoniet verschijnt er in de div met id `feedback`  "De input moet numeriek zijn"
- Op basis van de gekozen functionaliteit wordt de function `getProfitMessage` uitgevoerd.
- `getProfitMessage`: Afhankelijk van het verschil tussen de aan- en verkoopprijs wordt er een boodschap getoond:
    - Het resultaat is break even
    - De winst bedraagt: ...
    - Het verlies bedraagt: ...
### Dieren: function `execute` en `getAnimalLoveMessage`
- Het aantal dieren wordt opgehaald
- Er wordt nagegaan of het ingegeven getal positief is. Zoniet verschijnt de boodschap "Be positive".
- Bij een positief getal verschijnt de boodschap 'U meldde dat u x huisdier(en) bezat.' gevolgd door één van de volgende boodschappen
  - geen dieren: Geen dierenvriend?
  - één dier: Is het beestje niet eenzaam?
  - twee dieren: Komen ze een beetje overeen?
  - drie dieren: Leuke bende!
  - vier dieren: Gezellige beestenboel!
  - vijf of meer dieren: Amaai, wie geeft dat allemaal te eten?
### Tafel: function `execute` en `generateMultiplicationTable`
- De ingetikte tafel wordt opgehaald
- Check of er een positief geheel getal is ingetikt en geef eventueel passende feedback.
- Dit getal wordt vermenigvuldigd van 1 ... 10
- Gebruik een do while lus als het om een paar/even getal gaat (bvb. de tafel van 2)
- Gebruik een for lus bij onpare/oneven getallen
- De bewerkingen en het resultaat worden afgebeeld
### Tafels van ... tot: `execute` en function `generateMultiplicationTablesFromTo`
- De ingetikte getallen wordt opgehaald
- Check of er positieve gehele getal zijn ingetikt en geef eventueel passende feedback.
- Zorg ervoor dat in de variabele waarin de tafel van wordt bijgehouden het kleinste getal zit
- Geef de tafels naast elkaar weer
- De achtergrondkleur bij een tafel van een even getal is `gainsboro`
- De achtergrondkleur bij een tafel van een oneven getal is `aquamarine`

# Screenshots
![Screenshot winst](/img/Winst1.png)

![Screenshot verlies](/img/Winst2.png)

![Screenshot dieren](/img/Dieren.png)

![Screenshot 1 tafel](/img/Tafel1.png)

![Screenshot tafels](/img/Tafels.png)