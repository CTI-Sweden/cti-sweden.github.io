+++
title = 'Behöver jag en VPN?'
date = 2024-02-03T01:56:41+01:00
draft = true
toc = true
authors = [
    "Dennis Vesterlund"
]
groups = []
categories = []
sectors = []
tactics = []
techniques = []
tags = [
    "privacy",
    "vpn"
]
[[sources]]
title = "Netflix support - You seem to be using a VPN or proxy"
link = "https://help.netflix.com/en/node/277"
[[sources]]
title = "PTS - Information om användarne och deras kommunikation"
link = "https://pts.se/globalassets/startpage/dokument/icke-legala-dokument/rapporter/2018/post/pts-er-2018_6-information-om-anvandarna-och-deras-kommunikation.pdf"
+++

Kort svar: Nej.

Långt svar: är lite komplicerat...

Du har säkert, precis som mig, fått mycket reklam senaste åren från VPN
tjänster som påstår sig skydda dig mot diverse hot. Påståendena går från att ge
åtkomst till Netflix USA till att stoppa hackare från att få tag i dina
uppgifter och konton. I den här artikeln hoppas jag demystifiera valet av VPN leverantör så långt som rimligt.

## Så när behöver jag en VPN?

Nedan går vi mer utförligt igenom de påståenden som VPN tjänster gör när det
kommer till deras tjänster. Men för att göra det enkelt kan man använda följande
kriterier:

Om du är en person som:

- Använder oskyddade öppna nätverk, exempelvis på fik eller flygplatser
- Tror (eller vet) att din internetleverantör spionerar på din trafik
- Vill ha åtkomst till streamingtjänsters utbud från andra delar av världen

Det finns såklart vissa andra anledningar också (:skull_and_crossbones:) men de här skulle jag kalla de vanligaste.

## Påståenden

Det här är på inga sätt en helt utförlig lista eller på något sätt vetenskapligt
insamlad. Detta är de vanligaste påståenden jag har hört i reklam för olika
VPN tjänster.

### Geolocation

Det vanligaste och mest hållbara påståendet är att en VPN ger dig åtkomst till
streamingtjänsters utbud i andra länder. Detta kan vara korrekt för många
leverantörer men exempelvis Netflix blockerar VPN ansultingar till deras tjänst.
VPN leverantörer har många addresser de kan slussa din trafik genom och vissa påstår sig implementera tekniker för att komma runt blockeringsförsöken så det är
mycket möjligt att det fortfarande kommer fungera för dig, men det är bra att
veta att det kan vara problem att ansluta till vissa tjänster från vissa
leverantörer.

### Malware skydd

Detta är strunt i de flesta fallen. Vissa leverantörer kör IPS eller någon
from av dns adblock på din anslutning men det är inte vanligt. ProtonVPN exempelvis erbjuder [NetShield](https://protonvpn.com/support/netshield/) adblock.

### Skyddar mot hackare

Mestadels strunt. Om man är någon som använder öppna nätverk mycket och dessutom
använder tjänster som inte använder den senaste skyddstekniken i forma av
kryptering kan man få mer skydd av att använda en VPN. Sanningen i påståendet här kommer från att om man använder samma nätverk som en ilvillig aktör är det möjligt för dem att lura din dator att routa trafiken via dem. Det här gör inte automatisk så att de bara kan plocka dina inloggningar men det gör det mycket troligare att en sådan attack skulle lyckas om man inte använder VPN.

### Hindrar din ISP från att spionera på dig

Sant. En VPN kan helt hindra din leverantör att spionera på din data.
Internetleverantörer har möjlighet att kolla på och samla in din metadata, denna
kan sedan användas för att skapa en profil och sälja vidare eller sälja
annonsplatser. Enilgt PTS har telenor köpt upp ett bolag som verkar inom
anonssektorn.

> I början av 2016 köpte Telenor upp ett bolag, Tapad, som arbetar med
> annonsteknologi och vars syfte är att få bättre överblick över var människor
> finns och vad de gör online med hjälp av anonymiserade uppgifter
>
> Anna Montelius, PTS-ER-2018:6
> <https://pts.se/globalassets/startpage/dokument/icke-legala-dokument/rapporter/2018/post/pts-er-2018_6-information-om-anvandarna-och-deras-kommunikation.pdf>

Det finns just nu inga bevis på att telenor säljer eller delar uppgitter med
detta bolag men sedan 20 har det varit lag på att internetleverantörer måste
samla viss användardata.

<https://www.pts.se/sv/bransch/internet/sakerhet-och-skydd-av-uppgifter/Brottsbekampning/fragor-och-svar/>

Bahnhof publicerade 2019 en [artikel](https://bahnhof.se/2019/10/08/bahnhof-avslojar-operatorerna-som-lamnar-ut-dina-uppgifter-till-utpressare-2019/) där de avslöjar att Telia, ComHem och Telenor alla lämnat ut kunduppgifter kopplade till IP-addresser.

Däremot bör man vara medveten om att när man använder en VPN har den
leverantören möjlighet att spåra vad man gör över den VPN ansultningen. Precis
som med internetleverantören betyder det inte att de kan se allt du gör, då
många sidor själva använder kryptering som standard, men oskyddat innehåll,
vilka sidor du surfar till, samt en del annan metadata går alltid att se. VPN leverantörer brukar däremot
hållas till en högre standard i dessa avseenden och många har haft audits
utförda av 3:e part för att bevisa att de inte loggar eller sparar denna data.

## Välja leverantör

Om man bestämmer sig för att man vill ha en VPN vad ska man då tänka på? Här är
några saker jag skulle fundera på:

### Lokalisering

Vilket land VPN leverantören är registrerad i kan påverka hur de behöver agera i
många anseenden. Exempelvis måste ju en leverantör i USA följa deras
lagstiftning och en Svensk leverantör följa Svensk lagstiftning. Många
leverantörer skryter med att de är lokaliserade i Panama och liknande för att
komma undan 5 eyes, 9 eyes, och 12 eyes. Men det betyder också att man inte får
samma rättsliga skydd med sin data som man får i andra länder. I Sverige och USA
exempelvis behöver VPN leverantörer sammarbeta med rättsväsendet när det finns
skälig misstanke om brott. Vissa leverantörer kommer runt detta genom att helt
enkelt inte spara någon som hest användardata vilket betyder att när polisen
knackar på finns det ingenting att hämta.

### Loggning

De flesta leverantörer påstår att de inte loggar data om sina användare, men
vissa leverantörer går längre än andra genom att göra det svårare att få tag i
data om dig. Exempelvis genom att se till att deras miljö inte har möjlighet att spara data eller ta bort den direkt en session avslutas.

### Extern granskning

VPN leverantörer har inga krav på sig att rapportera hur deras miljö ser ut och
fungerar. Detta innebär att det inte finns något sätt för dig att kontrollera
vissa av de påståenden de gör om sin miljö. En granskning av en trejdepart kan h

### Historia

En viktig sak är att verifiera om aktören historiskt agerar på ett sätt som värnar om dig som kund. Har de haft säkerhetsincidenter och hur har dessa hanterats? Har de delat ut information eller haft rätsliga fall angåend sånt? Har de varit transperanta med deras verksamhet?

## Leverantörer

Det finns många leverantörer av den här typen av tjänster och nu mer ingår ofta VPN i andra tjänster man redan betalar för. Det här är såklart ingen utförlig lista men det är de viktigaste, och vanligaste, leverantörerna enligt mig.

### Mullvad

Jag går direkt ut och säger att det här är min personliga favorit, men jag ska
försöka att vara opartisk. Mullvad agerar också [leverantörspartner](https://mullvad.net/en/help/partnerships-and-resellers) för ett par andra VPN tjänster:

- [Mozilla VPN](https://www.mozilla.org/en-US/products/vpn)
- [Malwarebytes Privacy VPN](https://www.malwarebytes.com/vpn)
- [Tailscale](https://tailscale.com/) (Provides optional WireGuard exit nodes)

### Pango Group

Jag fann Pango Group då jag upptäckte att de hade förvärvat OVPN vilket är en leverantör jag håller i hög beaktning. Detta gjorde mig lite orolig då den här typen av konsolidering ofta leder till en sämre kvalitè i jakt på vinst. OVPN däremot skriver själva att de kommer agera precis som tidigare.

> OVPN kommer fortsätta att drivas som en fristående tjänst. Dina kunduppgifter som beskrivet i vår integritetspolicy lagras fortfarande på infrastruktur som drivs av OVPN, och vår VPN-infrastruktur kommer att fortsätta hålla samma höga säkerhetsstandard vi alltid har använt.
>
> David Wibergh, 2024-02-03, https://www.ovpn.com/sv/blog/nasta-kapitel-for-ovpn

Pango group äger följande VPN tjänster:

- [OVPN](https://www.ovpn.com/)
- [UltraVPN](https://ultravpn.com/)
- [VPN360](https://www.vpn360.com/)
- [Betternet](https://www.betternet.co/)

### Kape Technologies

<https://en.wikipedia.org/wiki/Teddy_Sagi#Kape_Technologies_plc>

Kape Technologies är ägarna bakom flera av de VPN tjänster som går hårdast ut
med marknadsföringskampanjer.

- [PIA](https://www.privateinternetaccess.com/)
- [ExpressVPN](https://www.expressvpn.com/)
- [CyberGhost VPN](https://www.cyberghostvpn.com/)
- [ZenMate VPN](https://zenmate.com/)

### Cyberspace

En till paraply-aktör som äger flera tjänster. Också den här väldigt flitig med marknadsföringskampanjer.

- [NordVPN](https://nordvpn.com/) (Nord Security)
- [AtlasVPN](https://atlasvpn.com/)
- [SurfShark](https://surfshark.com/vpn/) (Merger ongoing?)

### Integrity VPN

Drivs av [Femte Juli Stiftelsen](https://femtejuli.se/) och erbjuder VPN genom andra internetleverantörer. De har ett unikt tilvägagångssätt där man inte kan bli kund direkt hos dem utan man måste bli kund via en internetleverantör som sammarbetar med dem.

Denna aktör är ett bra alternativ om man har [Bahnhof](https://bahnhof.se/) som internetleverantör på grund av deras starka sammarbete.

### Proton VPN

En Schweizisk aktör som startade med att erbjuda integritetsfokuserad mail.
