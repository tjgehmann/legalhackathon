# NetHost GmbH — Antwortvorlagen für Behördenanfragen

> Alle Vorlagen sind auf Deutsch, da sie an deutsche Behörden gerichtet sind. Interne Dokumentationsfelder sind in [GROSSBUCHSTABEN] markiert und vor dem Versand zu befüllen.

---

## TEMPLATE-COMPLY-BESTANDSDATEN
### Verwendung: Herausgabe von Bestandsdaten auf rechtmäßiges Ersuchen

```
NetHost GmbH
Rechtsabteilung / Compliance
[ADRESSE]

Per Fax / per Post / per verschlüsselter E-Mail
An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Ihr Auskunftsersuchen vom [DATUM EINGANG] — Aktenzeichen [AZ]

Sehr geehrte Damen und Herren,

vielen Dank für Ihr Auskunftsersuchen nach § 174 TKG / § 22 TTDSG vom
[DATUM], das uns am [EINGANG] zugegangen ist.

Auf der Grundlage Ihres Ersuchens übermitteln wir folgende Bestandsdaten:

Domain / E-Mail-Adresse / Account-ID: [BEZEICHNUNG]

–––––––––––––––––––––––––––––––––––––––––––
BESTANDSDATEN (Stand: [DATUM])
–––––––––––––––––––––––––––––––––––––––––––
Name des Kontoinhabers:       [NAME]
Anschrift:                    [STRASSE, PLZ, ORT]
E-Mail-Adresse (Kontakt):     [E-MAIL]
Telefonnummer:                [TELEFON oder "nicht erfasst"]
Kundennummer:                 [KUNDENNUMMER]
Vertragsschluss:              [DATUM]
Vertragsart:                  [PRODUKT]
Zahlungsmittel:               [IBAN-ENDUNG / KREDITKARTE-ENDUNG oder "nicht erfasst"]
Letzte Anmelde-IP (statisch): [IP ODER "nicht erfasst"]
Domain-Registrierungsdatum:   [DATUM ODER "nicht zutreffend"]
–––––––––––––––––––––––––––––––––––––––––––

[FALLS DATEN NICHT VORHANDEN:]
Hinweis: [FEHLENDE ANGABE] ist in unseren Systemen nicht erfasst.

Diese Auskunft ergeht ausschließlich auf Grundlage Ihres förmlichen
Ersuchens und dient ausschließlich dem angegebenen Ermittlungszweck.
Wir weisen darauf hin, dass wir gem. § 174 Abs. 5 TKG den betroffenen
Kunden derzeit nicht über dieses Ersuchen informieren.

Für Rückfragen steht Ihnen unser Compliance-Team unter
compliance@nethost.de zur Verfügung.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance / Rechtsabteilung
NetHost GmbH

–––––––––––––––––––––––––––––––––––––––––––
Interner Vermerk (nicht für Behörde):
Anfrage-ID: [LEA-XXX]
Entscheidung: COMPLY
Rechtsgrundlage geprüft: JA
Daten übergeben: [DATUM/UHRZEIT]
Bearbeitende Person: [NAME]
Legal Hold aktiviert: [JA/NEIN]
–––––––––––––––––––––––––––––––––––––––––––
```

---

## TEMPLATE-COMPLY-BESTANDSDATEN-DRINGEND
### Verwendung: Dringende Herausgabe bei Gefahr im Verzug

```
NetHost GmbH — DRINGENDE ANTWORT
Compliance-Hotline: [NUMMER]

An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]
Übermittlung: [DATUM, UHRZEIT]

Betr.: Dringendes Auskunftsersuchen — Sofortantwort

Sehr geehrte/r Frau/Herr [NACHNAME],

auf Ihr als dringend gekennzeichnetes Ersuchen vom heutigen Tag
übermitteln wir unverzüglich folgende Bestandsdaten:

IP-Adresse: [ANGEFRAGTE IP]
Zeitpunkt:  [DATUM, UHRZEIT UTC]

Zugeordneter Kunde:
  Name:     [NAME]
  Anschrift: [ADRESSE]
  Kontakt:   [E-MAIL / TELEFON]
  Account:   [KUNDENNUMMER]

[FALLS IP NICHT NETHOST ZUGEHÖRIG:]
Die angefragte IP-Adresse [IP] gehört nicht zum IP-Adressbestand von
NetHost GmbH. Bitte wenden Sie sich an den zuständigen Anbieter
(RIR-Auskunft über RIPE NCC: https://apps.db.ripe.net/db-web-ui/query).

Für weitere dringende Anfragen: compliance-emergency@nethost.de
oder Compliance-Hotline: [NUMMER] (24/7 besetzt)

Mit freundlichen Grüßen

[NAME], NetHost GmbH Compliance

Interner Vermerk: Anfrage-ID [LEA-XXX] | GiV-Verfahren | [DATUM/UHRZEIT]
```

---

## TEMPLATE-COMPLY-BESCHLAGNAHME
### Verwendung: Herausgabe von Inhalts- oder Accountdaten auf richterlichen Beschluss

```
NetHost GmbH
Rechtsabteilung / Compliance
[ADRESSE]

[EINSCHREIBEN MIT RÜCKSCHEIN]
An: Staatsanwaltschaft [ORT]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Vollziehung des Beschlusses des [GERICHT] vom [BESCHLUSSDATUM]
       Aktenzeichen: [AZ GERICHT] / StA-AZ: [AZ STA]

Sehr geehrte Damen und Herren,

wir beziehen uns auf den uns am [EINGANG] zugegangenen Beschluss des
[GERICHT] vom [BESCHLUSSDATUM] und zeigen dessen vollständige Vollziehung an.

Vollzogene Maßnahme:
☐  Sicherstellung und Übermittlung von E-Mail-Inhalten
☐  Sicherstellung und Übermittlung von Account-/Hostingdaten
☐  Sicherstellung von [SONSTIGES]

Betroffene Kennung: [POSTFACH / DOMAIN / ACCOUNT-ID]
Zeitraum:           [VON – BIS] (wie im Beschluss angegeben)

Übermittlung der Daten:
Wir übermitteln die angeordneten Daten in der Form [VERSCHLÜSSELTES
DATENTRÄGER-PAKET / GESICHERTER DATEIDOWNLOAD / PHYSISCHER DATENTRÄGER].

Technische Details:
– Dateigröße: [GRÖSSE]
– Format: [FORMAT, z.B. MBOX, PST, ZIP]
– Prüfsumme (SHA-256): [HASH]
– Übergabe an: [ZUSTELLADRESSE / BEHÖRDE]
– Übergabedatum/-uhrzeit: [DATUM, UHRZEIT]

Hinweis zur Vollständigkeit:
[FALLS DATEN FEHLEN, z.B.:]
Für den Zeitraum [X–Y] sind keine E-Mails mehr vorhanden (gelöscht durch den
Nutzer vor Eingang der Anordnung).
[ODER:]
Die Daten wurden vollständig gemäß dem Beschlussumfang übergeben.

Nicht im Umfang des Beschlusses enthaltene Daten wurden nicht übermittelt.

Der Legal Hold auf [POSTFACH / ACCOUNT] bleibt bis zur schriftlichen
Aufhebung durch Ihre Behörde bestehen.

Wir bitten um schriftliche Bestätigung des Datenempfangs.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance / Rechtsabteilung
NetHost GmbH

Anlage: Datenträger / Download-Link / Dateiliste mit Hashwerten

Interner Vermerk: Anfrage-ID [LEA-XXX] | Legal Hold: AKTIV | [DATUM]
```

---

## TEMPLATE-TEILWEISE-COMPLY
### Verwendung: Teilergebnis bei Umfang-Überschreitung der Anfrage gegenüber dem Beschluss

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Teilweise Vollziehung des Beschlusses [AZ] vom [DATUM]
       Hinweis: Anfrage überschreitet Beschlussumfang

Sehr geehrte Damen und Herren,

wir beziehen uns auf den Beschluss des [GERICHT] vom [DATUM] sowie auf das
begleitende Schreiben [IHRER BEHÖRDE] vom [DATUM].

Wir vollziehen den Beschluss wie folgt:

Vollzogen (entspricht Beschlussumfang):
[BESCHREIBUNG DER HERAUSGEGEBENEN DATEN — NUR WAS IM BESCHLUSS STEHT]

Nicht vollzogen (geht über Beschlussumfang hinaus):
Die in Ihrem Begleitschreiben zusätzlich erbetene Herausgabe von
[BESCHREIBUNG DER NICHT-HERAUSGEGEBENEN DATEN] geht über den Umfang
des richterlichen Beschlusses hinaus. Der Beschluss erstreckt sich
ausschließlich auf [BESCHLUSSGEGENSTAND].

Für die Herausgabe der darüber hinausgehenden Daten bedarf es eines
gesonderten richterlichen Beschlusses, der diese Daten und/oder
diesen erweiterten Umfang ausdrücklich erfasst.

Wir bitten zu beachten, dass NetHost GmbH als datenschutzrechtlich
Verantwortliche nicht berechtigt ist, Kundendaten ohne ausreichende
Rechtsgrundlage zu übermitteln. Eine Ausweitung über den Beschlussumfang
hinaus würde einen Verstoß gegen Art. 6 DSGVO darstellen.

Die vollzogenen Daten werden wie folgt übermittelt:
[ÜBERMITTLUNGSDETAILS, HASH, DATUM]

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH
```

---

## TEMPLATE-ABLEHNUNG-INFORMELL
### Verwendung: Ablehnung informeller Anfragen ohne förmliche Rechtsgrundlage

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [ANFRAGENDE PERSON / BEHÖRDE]
[KONTAKTDATEN]

[ORT, DATUM]

Betr.: Ihre Anfrage vom [DATUM] — [BETREFF DER ANFRAGE]

Sehr geehrte/r Frau/Herr [NACHNAME],

vielen Dank für Ihre Anfrage.

Wir müssen Sie darauf hinweisen, dass NetHost GmbH als
datenschutzrechtlich Verantwortliche Kundendaten nur auf der Grundlage
einer ausreichenden Rechtsgrundlage i.S.d. Art. 6 DSGVO übermitteln darf.

Eine informelle Anfrage per [Telefon / E-Mail] — auch von Behörden —
begründet keine rechtliche Verpflichtung zur Auskunft und stellt
keine ausreichende Rechtsgrundlage für die Übermittlung
personenbezogener Kundendaten dar.

Wir bitten Sie daher, für Ihr Auskunfts- oder Ermittlungsbegehren ein
förmliches schriftliches Auskunftsersuchen auf der Grundlage der
einschlägigen Rechtsvorschriften (z.B. § 174 TKG, § 161 StPO) zu stellen.
Dies erfordert in der Regel die Einschaltung der zuständigen
Staatsanwaltschaft.

Das Ersuchen ist per Fax an [FAX-NUMMER] oder per Post an die oben
genannte Adresse zu richten und muss enthalten:
- Aktenzeichen des Ermittlungsverfahrens
- Name und Dienstbezeichnung des zuständigen Staatsanwalts
- Konkrete Benennung der begehrten Daten und der Rechtsgrundlage

Wir stehen für förmliche Auskunftsersuchen jederzeit zur Verfügung.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH

Interner Vermerk: Anfrage-ID [LEA-XXX] | REFUSE — informell | [DATUM]
```

---

## TEMPLATE-ABLEHNUNG-KEIN-BESCHLUSS
### Verwendung: Ablehnung bei fehlenden richterlichen Beschluss (wo erforderlich)

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Ihr Ersuchen vom [DATUM], Az. [AZ] — Fehlender richterlicher Beschluss

Sehr geehrte Damen und Herren,

wir haben Ihr Ersuchen vom [DATUM] geprüft. Sie ersuchen um
[BESCHREIBUNG DER ANGEFORDERTEN DATEN] auf der Grundlage von
[ZITIERTE RECHTSGRUNDLAGE].

Leider können wir dem Ersuchen in dieser Form nicht entsprechen:

[WÄHLEN SIE ZUTREFFENDES:]

☐  Die beantragte Maßnahme nach [§ 100g / § 99 / § 94] StPO erfordert
   gemäß [§ 101a Abs. 1 / § 100 Abs. 1 / § 98 Abs. 1] StPO einen
   richterlichen Beschluss. Ein solcher ist Ihrem Ersuchen nicht beigefügt.

☐  Die angeführte Rechtsgrundlage (§ [NORM]) deckt die begehrten Daten
   ([DATENTYP]) nicht ab. [ERLÄUTERUNG, z.B.: § 161 StPO ermächtigt zur
   Bestandsdatenauskunft, nicht zur Erhebung von Verkehrsdaten.]

☐  Das Ersuchen stammt von einer Behörde, die für diese Anordnung keine
   Anordnungskompetenz besitzt. [ERLÄUTERUNG]

Wir bitten Sie, das Ersuchen nach Erwirkung des erforderlichen richterlichen
Beschlusses erneut zu stellen. NetHost GmbH wird einen gültigen Beschluss
unverzüglich vollziehen.

[OPTIONAL — bei Beschlagnahme-Eilfällen:]
Wir regen an, bis zur Vorlage eines gültigen Beschlusses einen freiwilligen
Datensicherungs-Hinweis entgegenzunehmen: Wir werden die betreffenden Daten
[ACCOUNT / POSTFACH] für einen Zeitraum von [X TAGEN] sichern, ohne sie
zu löschen. Diese Sicherung erfolgt ohne Anerkennung einer Rechtspflicht
und endet nach Fristablauf ohne gesonderte Mitteilung.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH

Interner Vermerk: Anfrage-ID [LEA-XXX] | REFUSE — fehlender Beschluss | [DATUM]
[FALLS FREIWILLIGER HOLD:] Temporärer Hold bis [DATUM] auf [ACCOUNT/POSTFACH]
```

---

## TEMPLATE-ABLEHNUNG-ABGELAUFEN
### Verwendung: Ablehnung bei abgelaufenem Beschluss

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Ihr Ersuchen vom [DATUM] — Beschluss [AZ GERICHT] — Ablauf der Gültigkeit

Sehr geehrte Damen und Herren,

wir beziehen uns auf den uns am [EINGANG] zugegangenen Beschluss des
[GERICHT] vom [BESCHLUSSDATUM], Az. [AZ].

Wir müssen Sie darauf hinweisen, dass der vorliegende Beschluss eine
Befristung bis zum [ABLAUFDATUM] enthält. Unser Eingang erfolgte erst am
[EINGANGSDATUM], d.h. [X TAGE] nach Ablauf der im Beschluss gesetzten
Vollzugsfrist.

Da der Beschluss zum Zeitpunkt seines Eingangs bei uns nicht mehr gültig ist,
können wir ihn nicht vollziehen. Die Vollziehung eines abgelaufenen
richterlichen Beschlusses wäre rechtlich nicht gedeckt.

Wir bitten Sie, einen aktuellen Beschluss mit gültiger Vollzugsfrist
zu erwirken und uns zuzuleiten.

[OPTIONAL — freiwilliger temporärer Hold:]
Um den Ermittlungszweck nicht zu gefährden, sichern wir die betreffenden
Daten [ACCOUNT / POSTFACH] bis zum [DATUM — z.B. 4 Wochen ab heute] ohne
Weitergabe und ohne Benachrichtigung des Kunden. Diese Sicherung erfolgt
ohne Anerkennung einer Rechtspflicht.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH

Interner Vermerk: Anfrage-ID [LEA-XXX] | REFUSE — abgelaufener Beschluss
Freiwilliger Hold [ACCOUNT]: aktiv bis [DATUM]
```

---

## TEMPLATE-ABLEHNUNG-AUSLAND
### Verwendung: Ablehnung direkter Anfragen ausländischer Behörden (Nicht-EU)

```
NetHost GmbH
Legal & Compliance Department
[ADRESSE]

To: [FOREIGN AUTHORITY]
Attn.: [CONTACT PERSON]
Re.: Your request dated [DATE] — Reference: [REFERENCE]

[CITY, DATE]

Dear Sir or Madam,

Thank you for your inquiry dated [DATE].

NetHost GmbH is a German company operating exclusively under German and
European Union law. We are not in a position to comply with direct requests
from foreign law enforcement authorities.

Data disclosure to authorities outside the European Union requires a valid
legal basis under GDPR Article 44 et seq. and must follow established
international legal assistance procedures. Direct requests from foreign
authorities do not constitute such a legal basis.

For requests from United States authorities:
Please route your request through the established Mutual Legal Assistance
Treaty (MLAT) process via the U.S. Department of Justice and the German
Federal Ministry of Justice (Bundesministerium der Justiz).

For requests from other non-EU countries:
Please use the applicable bilateral or multilateral legal assistance
agreement and route your request through the German Federal Ministry of Justice.

Once a formal request reaches the competent German public prosecutor's
office and we receive a lawful order under German law, we will cooperate
promptly and fully.

We are unable to provide any information about the subject of your inquiry
outside this process.

Yours sincerely,

[NAME]
Head of Compliance
NetHost GmbH

Internal note: Request-ID [LEA-XXX] | REFUSE — foreign authority, no MLAT | [DATE]
```

---

## TEMPLATE-ABLEHNUNG-AUSLAND-EU
### Verwendung: Ablehnung direkter Anfragen aus EU-Mitgliedstaaten (ohne EIO)

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [AUSLÄNDISCHE BEHÖRDE]
z.H. [SACHBEARBEITER]

[ORT, DATUM]

Betr.: Ihre Anfrage vom [DATUM]

Sehr geehrte Damen und Herren,

vielen Dank für Ihre Anfrage.

NetHost GmbH unterliegt deutschem Recht und ist nicht berechtigt,
personenbezogene Kundendaten auf direkte Ersuchen ausländischer Behörden
herauszugeben — auch nicht für EU-Mitgliedstaaten.

Die Übermittlung personenbezogener Daten an Behörden eines anderen
EU-Mitgliedstaates im Bereich der Strafverfolgung erfolgt ausschließlich
im Rahmen der Europäischen Ermittlungsanordnung (EEA/EIO) nach der
Richtlinie 2014/41/EU. Dieser Weg verläuft über:

1. Antrag auf Europäische Ermittlungsanordnung durch Ihre Behörde
2. Übermittlung an die Zentralbehörde Ihres Mitgliedstaates
3. Weiterleitung an die deutsche Zentralbehörde
   (Bundesamt für Justiz, Adenauerallee 99–103, 53113 Bonn)
4. Vollstreckung durch die zuständige deutsche Staatsanwaltschaft
5. Förmliches Auskunftsersuchen der deutschen Staatsanwaltschaft
   an NetHost GmbH nach deutschem Recht

Eine direkte Anfrage an NetHost GmbH ohne diesen Verfahrensweg
begründet keine Auskunftspflicht und darf aus datenschutzrechtlichen
Gründen (Art. 44 ff. DSGVO) nicht entsprochen werden.

Wir stehen im Rahmen des EIO-Verfahrens für eine schnelle Kooperation
zur Verfügung.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH
```

---

## TEMPLATE-ESKALATION-TKU
### Verwendung: Interne Eskalation bei TKÜ-Beschluss — für Legal-Team

```
INTERNE ESKALATION — VERTRAULICH — SOFORTMASSNAHME

An:  Legal-Team (legal@nethost.de)
     IT-Sicherheit (itsec@nethost.de)
     Geschäftsleitung
Von: Compliance
Betr.: TKÜ-Beschluss eingegangen — sofortige Bearbeitung erforderlich

EINGANG: [DATUM, UHRZEIT]
ANFRAGE-ID: [LEA-XXX]

Ein richterlicher Beschluss zur Telekommunikationsüberwachung nach
§ 100a StPO ist eingegangen. Folgender Handlungsbedarf besteht:

BESCHLUSS-DETAILS:
– Ausstellendes Gericht:   [GERICHT]
– Aktenzeichen:            [AZ GERICHT] / [AZ STA]
– Betroffene Kennung:      [E-MAIL-ADRESSE / ANSCHLUSS]
– Gültigkeitsdauer:        [VON – BIS]
– Katalogsdelikt:          [DELIKT UND § 100a Abs. 2 NUMMER]

OFFENE FRAGEN — BITTE SOFORT KLÄREN:

☐  1. Ist der NetHost-Dienst [E-MAIL-HOSTING / SONSTIGES] als öffentlich
       zugänglicher Telekommunikationsdienst i.S.d. § 170 TKG eingestuft?

☐  2. Besteht für diesen Dienst eine technische TKÜ-Pflicht nach § 170 TKG?

☐  3. Verfügt NetHost über eine technische TKÜ-Schnittstelle (SINA-Box
       oder Äquivalent) für diesen Dienst?

☐  4. Falls nicht: Was ist der frühestmögliche Zeitpunkt der Umsetzung?
       Die Behörde muss unverzüglich informiert werden.

☐  5. Ist der Beschluss vollständig formal korrekt? (Landgericht,
       Richterunterschrift, Katalogsdelikt, Zeitbefristung, Verhältnismäßigkeit?)

FRIST: Der Beschluss läuft ab am [ABLAUFDATUM].
       Reaktionszeit: unverzüglich, spätestens [48h nach Eingang].

KEINE AKTIONEN GEGENÜBER DEM BETROFFENEN KUNDEN BIS ZUR FREIGABE DURCH LEGAL.

[NAME], Compliance
```

---

## TEMPLATE-KEINE-DATEN-VORHANDEN
### Verwendung: Anfrage rechtmäßig, aber Daten nicht mehr vorhanden (VDS-Problem)

```
NetHost GmbH
Rechtsabteilung / Compliance

An: [BEHÖRDE]
z.H. [SACHBEARBEITER]
Aktenzeichen: [AKTENZEICHEN]

[ORT, DATUM]

Betr.: Ihr Ersuchen vom [DATUM] — Daten nicht vorhanden

Sehr geehrte Damen und Herren,

wir haben Ihr Ersuchen vom [DATUM], Az. [AZ], geprüft. Das Ersuchen ist
formal korrekt und wird von uns als rechtmäßig anerkannt.

Wir müssen Sie jedoch darauf hinweisen, dass die angefragten Daten bei
NetHost GmbH nicht mehr vorhanden sind:

Angefragter Zeitraum:      [VON – BIS]
Angefragte Daten:          [VERBINDUNGSLOGS / SONSTIGE VERKEHRSDATEN]
Status bei NetHost:        Nicht gespeichert / Nicht mehr vorhanden

Hintergrund: NetHost GmbH betreibt keine anlasslose Vorratsdatenspeicherung.
Nach den Urteilen des Europäischen Gerichtshofs (EuGH, Urteil vom 20.09.2022,
C-793/19 und C-794/19) ist eine anlasslose Speicherung von Verbindungsdaten
mit dem Unionsrecht unvereinbar. NetHost speichert Verbindungsdaten nur,
soweit dies für den technischen Betrieb des jeweiligen Dienstes erforderlich
ist, und löscht diese nach Ablauf dieser Frist.

Für den von Ihnen angeforderten Zeitraum sind die betreffenden Daten nicht
mehr vorhanden.

[FALLS TEILWEISE VORHANDEN:]
Für den Zeitraum [NEUERER ZEITRAUM] liegen uns folgende Daten vor, die wir
aufgrund des vorliegenden Beschlusses herausgeben: [DATEN]

Wir bedauern, dass wir in diesem Fall nicht vollständig kooperieren können.

Mit freundlichen Grüßen

[NAME]
Leitung Compliance
NetHost GmbH
```
