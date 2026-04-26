# Presentationsmanus — Daniel

Slides 4–9 och 13 | Övningsversion | Svenska

---

## Slide 4: Traction

Innan vi byggde någonting körde vi varje event för hand. Med flit.

Carol och Anders hade redan kontakter med några av Sveriges bästa kockar. Så vi började där: kopplade ihop företag med kockar via deras befintliga nätverk. Noll marknadsföringskostnader, noll betald annonsering. Varje bokning kom via rykte och rekommendationer.

Och kunderna var inte precis vilka som helst. Hermès, Prada, Sail Racing, Chimi. Företag med höga krav. De valde oss för att vi levererade.

Men det vi hörde om och om igen var: "Kan ni hjälpa till med mer än bara kocken?" Varje kund ville ha en lokal också. Och transport. Och lite till. De ville inte ha en kockbokning, de ville ha hela eventet löst.

Det berättade för oss vad vi behövde bygga. Så vi byggde det. En plattform med de tre första leverantörskategorierna i ett och samma flöde: kock, lokal och hyrgods. Med autentisering, adminverktyg och betalning inkluderat.

Och nu är vi på nästa steg: att bygga verktyget kunderna faktiskt efterfrågar. Med ett heltidsteam kan vi driva produkt, partnerskap och sälj parallellt.

---

## Slide 5: Insikter

Varje event vi körde lärde oss samma sak om köparsidan.

Det är inte eventproffs. Det är kontorschefen, HR-ansvarige, eller assistenten som fick uppdraget. Inget leverantörsnätverk, ingen erfarenhet av vad saker borde kosta. De googlar, frågar runt och hoppas på det bästa. Varje gång.

Och när de kom till oss för en kock ville de alltid ha mer. Först kocken, sen lokalen, sen transporten. Varje gång expanderade behovet bortom en enda tjänst. Det är ingen slump. Det är så marknaden ser ut.

Det tredje mönstret är det som faktiskt gör det här till ett riktigt bolag: de kommer tillbaka. Och när de gör det börjar de från noll igen. Ingen institutionell minne. Ingen känsla för om priset är rimligt. Nästa event startar på ruta ett.

Det är därför en plattform spelar roll. Inte bara för att göra den första bokningen enklare. Utan för att fånga återköpscykeln, bygga leverantörsrelationerna, och ge köparna ett referensramverk de kan lita på.

En kund sa det rakt ut: inte "kan du hitta en kock?" utan "kan du ta hand om hela grejen?" Det är vad vi byggde Amici för att svara på.

---

## Slide 6: Produktvision — Flödet

Så här fungerar Amici.

Du beskriver ditt event. Antal gäster, format, datum. Plattformen matchar dig mot verifierade leverantörer och visar priser direkt. Inte inom 24 timmar. Inte efter en offertrunda. Direkt.

Du justerar inputs och totalsumman uppdateras live. Fler gäster, annat datum, annat format: priset uppdateras medan du gör det. När du är nöjd bokar du.

Efter bokningen har du ett val. Vill du att någon annan hanterar leverantörslogistiken åt dig, lägger du till en koordinator. Det är ett proffs som tar hand om allt. Vill du sköta det själv gör du det direkt via plattformen.

Och sedan finns det en funktion som investerare brukar fastna för: när du väl har kört ett event kan du återskapa det. Boka om från leverantörer du redan testat, behåll det som funkade, byt ut det du vill ändra. Plattformen kommer ihåg, även när du inte gör det.

Det som tidigare tog 7 till 14 dagar av aktivt arbete, utspritt över veckors väntan, tar nu minuter.

---

## Slide 7: Produktvision — Alla leverantörer. Ett ställe.

Det här är vad kunden ser.

Du beskriver eventet. Plattformen hämtar från vårt verifierade leverantörsnätverk och visar förhandlade priser direkt. Du väntar inte på att leverantörer ska svara. Det arbetet har vi gjort i förväg.

Till vänster ser du kundvyn på mobil. Till höger ser du vad leverantören ser i sin dashboard.

Ingen fram och tillbaka. Inga mejl till fem olika lokaler i hopp om att någon svarar. Priserna finns där. Du justerar, du bokar.

---

## Slide 8: Produktvision — Leverantörsmotorn

Här börjar det bli intressant för er som investerare.

I takt med att leverantörsnätverket växer blir det infrastruktur. Vilken plattform, byrå eller vilket företagsverktyg som helst som behöver koppla ihop användare med eventsuppliers kan plugga in sig i Amici via API eller embed.

Kocknätverket, lokalerna, transportleverantörerna, utrustningsuthyrningen, personalen: allt tillgängligt via en enda integration.

Vi bygger inte bara ett bokningsverktyg. Vi bygger lagret som sitter under eventspelarnas supply-sida. Det är ett annat sorts bolag.

---

## Slide 9: Konkurrenslandskapet

Marknaden har två ytterligheter. Till vänster gör du allt själv: googlar, ringer runt, koordinerar i ett kalkylblad. Det är gratis men jobbigt.

Till höger anlitar du en traditionell byrå. Fullservice, professionellt hanterat, och prissatt därefter. Byggt för företag med stora eventbudgetar och dedikerade inköpsteam.

Däremellan finns enskilda plattformar. Du kan boka en lokal på en, en cateringleverantör på en annan. Men du jonglerar fortfarande fyra olika leverantörer och ingen är ansvarig för helheten.

Amici sitter mellan enskilda plattformar och traditionella byråer. Alla dina leverantörer, en plattform. Lägg till en koordinator om du behöver det.

Anledningen till att byråer inte kan svara på det här: de säljer arbetstimmar. Varje event de kör kostar mer personaltid. Amici säljer mjukvara och nätverkseffekter. Varje event vi förmedlar körs på samma plattform till nästan noll marginalkostnad. Därför ser enhetsekonomin helt annorlunda ut.

---

## Slide 13: Plattformen

Jag vill ge er en konkret bild av vad Edin byggt, för det påverkar direkt hur kapitaleffektiva vi är.

Plattformen är ett monorepo. En kodbas. Fyra separata applikationer: kundplattformen, leverantörsportalen, admindashboarden och marknadsföringssajten. De delar kod, konfiguration och typer.

84 delade komponenter across de fyra apparna. Ändra en knapp på ett ställe och den uppdateras överallt. Nya leverantörskategorier kopplas in utan att vi behöver bygga om kärnan.

39 versionerade databasmigreringar. En automatiserad deployment-pipeline. Typsäkert från databasen hela vägen upp till UI:t.

De flesta startups samlar på sig teknisk skuld från dag ett. Edin byggde det här från grunden för att undvika det. Det innebär snabbare iteration, lägre burn och lägre risk för er som investerare. Fyra personer byggde det här. Tänk vad ett finansierat team kan göra med det.

---

## Anteckningar för övning

- **Slide 5 (Insikter):** kundcitatet är din landningsmomenten. Ta en paus innan du säger det.
- **Slide 6 (Flödet):** gå igenom stegen långsamt, investerare behöver visualisera UX:en.
- **Slide 9 (Konkurrensen):** "Byråer säljer arbetstimmar / Amici säljer mjukvara och nätverkseffekter" är din skarpaste poäng. Leverera den rent och låt den landa innan du går vidare.
- **Slide 13 (Plattformen):** om Edin är i rummet kan du lämna över den här sliden till honom. Annars, börja med affärsimplikationen ("kapitaleffektivt") snarare än den tekniska arkitekturen.
