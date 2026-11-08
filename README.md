# Where Have I Been

Dit project is een website gebouwd met Next.js. Volg de stappen hieronder om het project op een Windows-computer lokaal te starten, naar GitHub te pushen en online te zetten via Vercel.

## 1. Installeer Node.js

Node.js bevat ook npm, waarmee de benodigde projectpakketten worden geïnstalleerd.

1. Ga naar [nodejs.org/en/download](https://nodejs.org/en/download) en download de **LTS**-versie voor Windows.
2. Open het gedownloade installatiebestand en volg de installatiestappen. De standaardinstellingen zijn geschikt.
3. Sluit een eventueel geopende PowerShell of terminal en open die opnieuw.
4. Controleer de installatie met:

	```powershell
	node -v
	npm -v
	```

Beide commando's tonen een versienummer.

## 2. Open PowerShell in de projectmap

1. Open de projectmap in Windows Verkenner.
2. Klik in de balk van het adres en type: `Powershell` 
3. Check dat de Powershell opent in `C:\Users\Olivia\where-have-i-been>` 

Je kunt de map ook openen in [Visual Studio Code](https://code.visualstudio.com/) en daar **Terminal > Nieuwe terminal** kiezen.

## 3. Start de website lokaal

Voer in PowerShell of de terminal van Visual Studio Code deze opdrachten uit:

```powershell
npm install
npm run dev
```

`npm install` installeert de projectpakketten. Open daarna [http://localhost:3000](http://localhost:3000) in je browser. De website wordt bijgewerkt wanneer je bestanden aanpast.

Stop de lokale server met **Ctrl+C** in de terminal.

Als je al eerder een install gedaan hebt dan kan je starten met:
```powershell
npm run dev
``` 

## 4. Push het project naar GitHub via Visual Studio Code

Je hebt een GitHub-account en Git nodig. Installeer Git voor Windows via [git-scm.com/download/win](https://git-scm.com/download/win) en open Visual Studio Code daarna opnieuw.

### Eerste keer publiceren

1. Open de projectmap in Visual Studio Code.
2. Klik links op **Broncodebeheer** (het vertakkingspictogram).
3. Kies **Repository initialiseren** als Visual Studio Code daarom vraagt.
4. Stage de bestanden die je wilt opslaan met het **+**-pictogram naast een bestand, of stage alle bestanden.
5. Typ bovenaan een commitbericht, bijvoorbeeld `Eerste versie`, en klik op **Commit**.
6. Klik op **Publish Branch** of **Publish to GitHub**.
7. Meld je aan bij GitHub als daarom wordt gevraagd. Kies of de repository openbaar of privé moet zijn en bevestig het publiceren.

Visual Studio Code maakt de GitHub-repository aan en pusht de commit. De repository is daarna te vinden op `https://github.com/<gebruikersnaam>/<repositorynaam>`.

### Volgende wijzigingen pushen

1. Sla je wijzigingen op en open **Broncodebeheer**.
2. Stage de bestanden die je wilt meesturen met **+**.
3. Typ een commitbericht en klik op **Commit**.
4. Klik op **Synchronisatie wijzigen** of **Push** om de commit naar GitHub te sturen. Bevestig zo nodig dat Visual Studio Code de wijzigingen mag synchroniseren.

De commit staat nu op GitHub. Als de repository nog niet aan een GitHub-account is gekoppeld, gebruik dan **Publish Branch** om dat alsnog te doen.

## 5. Deploy de website via Vercel

1. Push eerst de laatste wijzigingen naar GitHub.
2. Ga naar [vercel.com/new](https://vercel.com/new) en meld je aan met GitHub.
3. Geef Vercel toestemming om de GitHub-repository te gebruiken.
4. Kies bij **Import Git Repository** de repository van dit project en klik op **Import**.
5. Vercel herkent Next.js automatisch. Laat de standaardinstellingen staan en klik op **Deploy**.
6. Na de build toont Vercel de URL van je website. Die eindigt meestal op `.vercel.app`.

Je projecten en deployments staan op [vercel.com/dashboard](https://vercel.com/dashboard). Na de eerste koppeling maakt iedere push naar GitHub automatisch een nieuwe deployment. De productie-URL blijft hetzelfde; tijdelijke deployments kunnen ook een eigen preview-URL krijgen.
