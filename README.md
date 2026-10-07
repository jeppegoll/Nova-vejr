# Nova-vejr
en app der viser vejudsigten kun for kysten ud for NOVA
Hellerup Kyst – vind og bølger

En enkel webside, der viser prognosen for vind og bølger på Øresund ud for Hellerup Havn de næste 50 timer. Den er lavet til kajakroere og andre, der skal ud på vandet, men den giver ingen anbefalinger. Hver enkelt må selv vurdere, hvad de kan klare.

Se siden: https://BRUGERNAVN.github.io/hellerup-kyst/

Hvad siden viser
Lige nu: vindhastighed og retning, vindstød, Beaufort-styrke, bølgehøjde og bølgeretning, vand- og lufttemperatur samt vejret.
Graf for de næste 50 timer: middelvind og vindstød øverst, bølgehøjde nederst. Mørke timer mellem solnedgang og solopgang er skraveret, og små pile viser, hvor vinden blæser hen.
Time for time: en tabel med alle tallene. Den er foldet sammen og åbnes med et tryk på overskriften. Hver dag viser også tidspunkterne for solopgang og solnedgang.

Ved hver vindretning står, om det er pålandsvind (fra øst, ind mod stranden), fralandsvind (fra vest, ud fra land) eller vind langs kysten (fra nord eller syd).

Sådan bruger du den på telefonen

Åbn adressen i browseren og læg den på hjemmeskærmen:

iPhone: Åbn siden i Safari, tryk på del-knappen og vælg Føj til hjemmeskærm.
Android: Åbn siden i Chrome, tryk på ⋮ og vælg Føj til startskærm.

Så ligger den som et ikon og åbner som en app.

Hvor tallene kommer fra

Alle data kommer fra MET Norway (Meteorologisk institutt) og bruges under licensen CC BY 4.0:

Vind, lufttemperatur, nedbør og vejr: Locationforecast 2.0 for 55,73° N 12,58° Ø.
Bølger og vandtemperatur: Oceanforecast 2.0 for 55,73° N 12,62° Ø, lidt ude i Sundet.

Siden henter prognosen direkte fra MET Norway, hver gang den åbnes, og igen hver halve time, mens den står åben. Der er ingen server eller database bag. Kan tallene ikke hentes, står der en besked på siden i stedet for gamle tal.

Solopgang og solnedgang regnes ud på selve siden. "Føles som"-temperaturen er vindafkøling, som kun bruges, når luften er 10 °C eller koldere og det blæser.

Ansvar

Siden viser en vejrprognose. Den siger ikke, om det er sikkert at tage på vandet, og prognoser kan tage fejl. Se også DMI Hav og is, og vurder altid forholdene selv, før du tager ud.

Indhold og ændringer

Hele siden ligger i én fil, index.html, med HTML, CSS og JavaScript. Den bruger skrifttyperne Barlow Condensed og Source Sans 3 fra Google Fonts.

Du ændrer siden ved at uploade en ny index.html til repositoryet. Den nye version er online efter et minut eller to.

Hvis siden skal vise et andet sted, retter du koordinaterne i de to adresser øverst i scriptet, LOC_URL og SEA_URL, og i funktionen sun(), som bruges til at regne solopgang og solnedgang ud. Teksterne om påland og fraland forudsætter en kyst, der vender mod øst, og står i funktionen shore().
