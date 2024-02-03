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
title = PTS - Information om användarne och deras kommunikation
link = "https://pts.se/globalassets/startpage/dokument/icke-legala-dokument/rapporter/2018/post/pts-er-2018_6-information-om-anvandarna-och-deras-kommunikation.pdf"
+++

Kort svar: Nej.

Långt svar: är lite komplicerat...

Du har säkert, precis som mig, fått mycket reklam senaste åren om diverse VPN
tjänster som påstår sig skydda dig mot diverse hot. Påståendena går från att ge
åtkomst till Netflix USA till att stoppa hackare från att få tag i dina
uppgifter och konton. Låt oss bryta ner de vanligaste påståenden och se vad som
håller upp och inte.

## Så när behöver jag en VPN?

Nedan går vi mer utförligt igenom de påståenden som VPN tjänster gör när det
kommer till deras tjänster. Men för att göra det enkelt kan man använda följande
kriterier:

Om du är en person som:

- Använder oskyddade öppna nätverk, exempelvis på fik eller flygplatser
- Tror att din internetleverantör spionerar på din trafik
- Vill ha åtkomst till streamingtjänsters utbud från andra delar av världen

## Påståenden

Det här är på inga sätt en helt utförlig lista eller på något sätt vetenskapligt
insamlad. Detta är bara de vanligaste påståenden jag har hört i reklam för olika
VPN tjänster.

### Geolocation

Det vanligaste och mest hållbara påståendet är att en VPN ger dig åtkomst till
streamingtjänsters utbud i andra länder. Detta kan vara korrekt för många
leverantörer men exempelvis Netflix blockerar VPN ansultingar till deras tjänst.
VPN leverantörer har många addresser de kan slussa din trafik genom så det är
mycket möjligt att det fortfarande kommer fungera för dig, men det är bra att
veta att det kan vara problem att ansluta till vissa tjänster från vissa
leverantörer.

### Malware skydd

Detta är rent strunt i de flesta fallen. Vissa leverantörer kör IPS eller någon
from av dns adblock på din anslutning men det är försvinnande ovanligt. **_Nedan
kollar vi närmare på en sådan leverantör._**

### Skyddar mot hackare

Mestadels strunt. Om man är någon som använder öppna nätverk mycket och dessutom
använder tjänster som inte använder den senaste skyddstekniken i forma av
kryptering kan man få mer skydd av att använda en VPN.

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

Däremot bör man vara medveten om att när man använder en VPN har den
leverantören möjlighet att spåra vad man gör över den VPN ansultningen. Precis
som med internetleverantören betyder det inte att de kan se allt du gör, då
många sidor själva använder kryptering som standard, men oskyddat innehåll samt
vilka sidor du surfar till går alltid att se. VPN leverantörer brukar däremot
hållas till en högre standard i dessa avseenden och många har haft audits
utförda av 3:e part för att bevisa att de inte loggar data.

## Välja leverantör

Om man bestämmer sig för att man vill ha en VPN vad ska man då tänka på? Här är
några saker jag skulle fundera på:

### Lokalisering

Vilket land VPN leverantören är registrerad i kan påverka hur de behöver agera i
många anseenden. Exempelvis måste ju en leverantör i USA följa deras
lagstiftning och en Svensk leverantör följa Svensk lagstiftning. Många
leverantörer skryter med att de är lokaliserade i Panama och liknande för att
komma undan five eyes och **_dylikt_**. Men det betyder också att man inte får
samma rättsliga skydd med sin data som man får i andra länder. I Sverige och USA
exempelvis behöver VPN leverantörer sammarbeta med rättsväsendet när det finns
skälig misstanke om brott. Vissa leverantörer kommer runt detta genom att helt
enkelt inte spara någon som hest användardata vilket betyder att när polisen
knackar på finns det ingenting att hämta.

### Loggning

De flesta leverantörer påstår att de inte loggar data om sina användare, men
vissa leverantörer går längre än andra genom att göra det svårare att få tag i
data om dig.

### Extern granskning

VPN leverantörer har inga krav på sig att rapportera hur deras miljö ser ut och
fungerar. Detta innebär att det inte finns något sätt för dig att kontrollera
vissa av de påståenden de gör om sin miljö. En granskning av en trejdepart kan h

## Leverantörer

### Mullvad

Jag går direkt ut och säger att det här är min personliga favorit, men jag ska
försöka att vara opartisk. Mullvad är en Svensk leverantör vilket betyder att
den faller under Svensk lagstiftning. De sparar ingen data om sina användare
utöver den data de behöver för att kunna ta betalt för tjänsten. Om man vill
vara helt anonym finns möjligten att antingen skicka in kontanter med brev eller
köpa förbetalda kort man kan använda för att aktivera sitt konto.

Mullvad har genomgått flera prövningar av externa parter och skryter om det på
sin [hemsida](https://mullvad.net/en/blog/tag/audits). Sedan September 2023 kör
hela deras infrastruktur endast på
[RAM utan permanent lagring](https://mullvad.net/sv/blog/we-have-successfully-completed-our-migration-to-ram-only-vpn-infrastructure).

Mullvad agerar också leverantörspartner för ett par andra VPN tjänster:

- [Mozilla VPN](https://www.mozilla.org/en-US/privacy/subscription-services/)
- Malwarebytes
- Tailscale

### Pango Group

- OVPN
-

### Kape Technologies

<https://en.wikipedia.org/wiki/Teddy_Sagi#Kape_Technologies_plc>

Kape Technologies är ägarna bakom flera av de VPN tjänster som går hårdast ut
med marknadsföringskampanjer

- PIA
- ExpressVPN
- CyberGhost VPN
- ZenMate VPN

### Nord Security

- NordVPN
- AtlasVPN
- Surfshark (Merger ongoing?)
