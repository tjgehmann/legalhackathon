# Rechtlicher Rahmen: Behördliche Auskunfts- und Beschlagnahmepflichten für deutsche Hosting- und Domain-Unternehmen

> Dieses Dokument ist ein praxisorientierter Überblick für das Compliance-Team von NetHost GmbH. Es ersetzt keine Rechtsberatung im Einzelfall.

---

## 1. Das Fundament: Verfassungsrechtlicher Schutz (Art. 10 GG)

### Fernmeldegeheimnis

Art. 10 GG schützt das **Fernmeldegeheimnis**: die Vertraulichkeit der Telekommunikation und ihrer Inhalte. Dieser Schutz wirkt auch gegenüber dem Staat — staatliche Eingriffe sind nur auf gesetzlicher Grundlage und unter strikten Verhältnismäßigkeitsanforderungen zulässig.

**Was das für NetHost bedeutet:**
- E-Mail-Inhalte, Kommunikationsmetadaten und Verbindungsdaten genießen verfassungsrechtlichen Schutz
- Jede Herausgabe an Behörden erfordert eine spezifische gesetzliche Grundlage
- Herausgabe ohne Rechtsgrundlage = Verletzung des Fernmeldegeheimnisses + DSGVO-Verstoß

### Das Prinzip des Richtervorbehalts (Richtervorbehalt)

Bei grundrechtsintensiven Eingriffen — insbesondere in das Fernmeldegeheimnis — ist ein **vorheriger richterlicher Beschluss** erforderlich. Der Richtervorbehalt dient als Kontrollmechanismus: Ein unabhängiger Richter prüft, ob die Maßnahme gerechtfertigt ist, bevor sie vollzogen wird.

**Ausnahme — Gefahr im Verzug (Eilkompetenz):**
Bei unmittelbarer Gefahr für den Ermittlungszweck (z.B. drohende Datenvernichtung) kann in bestimmten Fällen die Staatsanwaltschaft oder Polizei ohne vorherigen Richterbeschluss handeln. Sie müssen dann **unverzüglich** (in der Regel innerhalb von 3 Werktagen) eine richterliche Bestätigung einholen. Ohne diese Bestätigung wird die Maßnahme rückwirkend rechtswidrig.

> **Kritisch:** Die Eilkompetenz gilt NICHT für alle Maßnahmen. Für Verkehrsdaten nach § 100g StPO gibt es **keine Eilkompetenz** der Staatsanwaltschaft.

---

## 2. Strafprozessordnung (StPO) — Die zentralen Vorschriften

### § 94–98 StPO — Sicherstellung und Beschlagnahme

**§ 94 StPO — Sicherstellung von Beweisgegenständen**
Gegenstände (einschließlich Daten auf Speichermedien), die als Beweismittel für die Untersuchung von Bedeutung sein können, sind in Verwahrung zu nehmen oder anderweitig sicherzustellen.

**§ 98 StPO — Beschlagnahme durch richterliche Anordnung**
Beschlagnahmen ordnet der Richter an. Bei Gefahr im Verzug: Staatsanwaltschaft oder Polizei können sicherstellen, müssen jedoch unverzüglich richterliche Bestätigung erwirken.

**Für NetHost relevant:**
- Wenn ein gültiger Beschlagnahmebeschluss nach § 98 StPO vorliegt, besteht eine Herausgabepflicht
- Ohne Beschluss: keine Pflicht, keine Befugnis zur Herausgabe (außer Gefahr im Verzug mit StA-Anordnung)
- Polizeiliche Anfragen allein ohne StA- oder Richterbeschluss: ablehnen

---

### § 99–101 StPO — Postbeschlagnahme (analoge Anwendung auf E-Mail)

**§ 99 StPO — Postbeschlagnahme**
Ursprünglich für Briefpost und Pakete konzipiert. Bundesverfassungsgericht und BGH haben die analoge Anwendung auf **beim Provider gespeicherte E-Mails** bejaht (BVerfG NJW 2006, 976; BGH Beschl. v. 31.03.2009 — 1 StR 76/09).

**§ 100 StPO — Richterliche Anordnung der Postbeschlagnahme**
Ausschließlich der Richter darf die Postbeschlagnahme anordnen. Staatsanwaltschaft hat begrenzte Eilkompetenz, muss aber unverzüglich richterliche Bestätigung erwirken.

**Konsequenz für E-Mail-Provider:**
- E-Mail-Inhalte beim Hosting-Anbieter genießen Fernmeldegeheimnisschutz (Art. 10 GG) — bestätigt durch BVerfG
- Herausgabe nur aufgrund richterlichem Beschluss
- Beschluss muss das konkrete Postfach, den Zeitraum und die Maßnahme spezifizieren

**Die "Transitfrage":** Ob E-Mails im Posteingang ("ruhend") denselben Schutz genießen wie E-Mails "in transit", war lange umstritten. Nach herrschender Meinung gilt der Schutz des Art. 10 GG auch für beim Provider gespeicherte E-Mails, solange sie noch im Herrschaftsbereich des Providers liegen und noch nicht vollständig vom Empfänger abgerufen wurden (BVerfGE 124, 43).

---

### § 100a StPO — Telekommunikationsüberwachung (TKÜ)

**Was es ist:** Echtzeit-Überwachung und Aufzeichnung laufender Telekommunikation.

**Voraussetzungen:**
- Richterlicher Beschluss (immer, keine Ausnahmen)
- Katalogtat nach § 100a Abs. 2 StPO (schwere Straftaten: Mord, Bandendiebstahl, Drogenhandel, Terrorismus, schwerer Betrug, u.a.)
- Verdächtiger muss Beschuldigter sein oder die Anschlusskennung muss diesem zuzuordnen sein
- Subsidiarität: andere Ermittlungsmaßnahmen müssen erfolglos oder aussichtslos sein

**Für NetHost:**
- TKÜ trifft nur "öffentlich zugängliche Telekommunikationsdienste" (§ 170 TKG)
- Shared Hosting ohne eigenen E-Mail-Dienst: wahrscheinlich KEIN öffentlicher TK-Dienst
- E-Mail-Hosting mit eigenen Postfächern für Kunden: KANN öffentlicher TK-Dienst sein
- Technische Umsetzung: SINA-Box oder vergleichbare TKÜ-Schnittstelle erforderlich — NetHost muss prüfen, ob diese vorhanden ist
- Bei Eingang eines TKÜ-Beschlusses: sofort Legal und IT kontaktieren

---

### § 100g StPO — Erhebung von Verkehrsdaten

**Was es ist:** Herausgabe von gespeicherten Verbindungs- und Verkehrsdaten (wer hat wann mit wem telefoniert/kommuniziert, welche IP-Adressen wurden verwendet).

**Voraussetzungen:**
- **Richterlicher Beschluss zwingend** (§ 101a Abs. 1 StPO) — **keine Eilkompetenz der Staatsanwaltschaft**
- Bestimmte Straftaten (bei § 100g Abs. 1: erhebliche Straftaten; bei § 100g Abs. 2: schwere Straftaten aus Katalog)
- Nur Verkehrsdaten, die beim Anbieter tatsächlich gespeichert sind

**VDS-Problem (Vorratsdatenspeicherung):**

Die Vorratsdatenspeicherung in Deutschland ist nach mehreren EuGH-Urteilen (SpaceNet/Telekom Deutschland, C-793/19 und C-794/19, April 2022) mit Unionsrecht unvereinbar. Das TDDDG enthält keine anlasslose Speicherpflicht mehr.

**Praktische Konsequenz für NetHost:**
- NetHost ist NICHT verpflichtet, Verbindungsdaten anlasslos zu speichern
- NetHost darf Verbindungsdaten nur so lange speichern, wie es für den eigenen Betrieb erforderlich ist (Datensparsamkeit, Art. 5 Abs. 1 lit. e DSGVO)
- Wenn bei einer § 100g StPO-Anfrage die gespeicherten Daten nicht mehr existieren: ausdrücklich mitteilen ("Die angeforderten Verbindungsdaten für den Zeitraum X–Y sind nicht mehr gespeichert, da NetHost keine anlasslose Vorratsdatenspeicherung betreibt.")

---

### § 161 / 163 StPO — Allgemeine Ermittlungskompetenz

**§ 161 StPO — Staatsanwaltschaft:** Zur Erforschung des Sachverhalts kann die Staatsanwaltschaft von Behörden und Beamten Auskunft verlangen und Ermittlungen jeder Art vornehmen oder vornehmen lassen.

**§ 163 StPO — Polizei:** Die Polizei ist befugt, alle Maßnahmen zu treffen, die zur Erforschung des Sachverhalts und zur Ermittlung des Täters erforderlich sind.

**Für Bestandsdatenauskunften:** Diese Vorschriften bilden zusammen mit § 174 TKG / § 22 TTDSG die Rechtsgrundlage für Bestandsdatenanfragen ohne Richterbeschluss.

> **Wichtig:** §§ 161/163 StPO decken **Bestandsdaten** ab, aber NICHT Inhalte oder Verkehrsdaten. Wer § 161 StPO als Grundlage für eine Inhalts- oder Verkehrsdatenanfrage angibt, hat die falsche Rechtsgrundlage.

---

## 3. Telekommunikationsgesetz (TKG) und TTDSG

### § 174 TKG — Auskunftserteilung

Anbieter von öffentlichen Telekommunikationsnetzen und öffentlich zugänglichen Telekommunikationsdiensten sind verpflichtet, auf Anordnung der Behörden Bestandsdaten zu übermitteln.

**Bestandsdaten umfassen (§ 174 Abs. 1 TKG):**
- Name, Anschrift, Geburtsdatum
- Rufnummern und sonstige Anschlusskennungen
- Bankverbindung (soweit für Vertrag erhoben)
- Datum des Vertragsbeginns

**§ 174 Abs. 4 TKG — Zugangsdaten:** Passwörter und PINs dürfen NICHT herausgegeben werden, außer für bestimmte Delikte im Zusammenhang mit dem Schutz des Kindeswohls oder bei richterlichem Beschluss.

**Anspruchsberechtigte nach § 174 TKG:**
- Staatsanwaltschaft (immer)
- Polizei, wenn sie im staatsanwaltschaftlichen Auftrag handelt oder bei Gefahrenabwehr nach Landesrecht
- Verfassungsschutzbehörden (Bundesamt für Verfassungsschutz, LfV) — eigene gesetzliche Grundlagen

### § 22/23 TTDSG — Telemediendienste

Für Anbieter von Telemediendiensten (Webhosting ohne eigenen TK-Dienst) gilt § 22 TTDSG als Auskunftsgrundlage für Bestandsdaten. Inhaltlich ähnlich wie § 174 TKG.

---

## 4. DSGVO-Schnittstelle

### Wann ist eine Datenherausgabe unter der DSGVO rechtmäßig?

**Art. 6 Abs. 1 lit. c DSGVO:** Verarbeitung (einschließlich Weitergabe) ist rechtmäßig, soweit sie zur Erfüllung einer rechtlichen Verpflichtung erforderlich ist, der der Verantwortliche unterliegt.

**Was das bedeutet:** Wenn NetHost aufgrund von § 174 TKG, § 99 StPO oder einem Richterbeschluss verpflichtet ist, Daten herauszugeben, ist diese Weitergabe unter Art. 6 Abs. 1 lit. c DSGVO rechtmäßig — kein separater DSGVO-Rechtsfertigungsgrund erforderlich.

**Wenn keine Rechtspflicht besteht:** Zum Beispiel bei informellen Polizeianfragen — gibt es keine rechtliche Verpflichtung, ist Art. 6 Abs. 1 lit. c DSGVO nicht anwendbar. NetHost muss dann Art. 6 Abs. 1 lit. f DSGVO (berechtigtes Interesse) prüfen — was in der Praxis für behördliche Anfragen ohne Rechtsgrundlage nicht ausreicht.

### Art. 23 DSGVO — Beschränkungen

Mitgliedstaaten können durch Rechtsvorschriften die Rechte und Pflichten aus der DSGVO beschränken, wenn dies für Ermittlungs- und Strafverfolgungszwecke erforderlich ist. Die StPO-Regelungen und das TTDSG stellen solche nationalen Einschränkungsregeln dar.

### Rechenschaftspflicht (Art. 5 Abs. 2 DSGVO)

NetHost muss **jede Datenherausgabe dokumentieren**: welche Daten, an wen, auf welcher Rechtsgrundlage, wann. Dies ist im Falle einer DSGVO-Prüfung der Nachweispflichtige.

### Benachrichtigung des Betroffenen

**Grundsatz:** Der von einer Behördenmaßnahme betroffene Kunde wird von der Ermittlungsbehörde benachrichtigt (§ 101 StPO), nicht von NetHost.

**Was NetHost tun darf/muss:**
- Während laufender Ermittlungen: KEINE Benachrichtigung des Kunden (Gefährdung des Ermittlungszwecks)
- Nach Abschluss der Ermittlungen: Ermittlungsbehörde informiert den Betroffenen
- Bei Datenpanne i.S.d. Art. 4 Nr. 12 DSGVO (z.B. unbefugte Herausgabe): Meldepflicht nach Art. 33/34 DSGVO

---

## 5. Die Behördenhierarchie — Wer darf was anordnen?

### Übersicht der Anordnungsbefugnisse

| Maßnahme | Richter | Staatsanwaltschaft | Polizei |
|----------|---------|-------------------|---------|
| Bestandsdatenauskunft (§ 174 TKG) | Ja | Ja | Ja (im Ermittlungsauftrag) |
| Postfachbeschlagnahme (§ 99/100 StPO) | Ja (Regelfall) | Ja (nur bei GiV, + sofort Richterbestätigung) | Nein |
| Datenbeschlagnahme (§ 94/98 StPO) | Ja (Regelfall) | Ja (nur bei GiV, + sofort Richterbestätigung) | Ja (nur bei GiV, + sofort StA/Richterbestätigung) |
| Verkehrsdaten (§ 100g StPO) | Ja (zwingend) | Nein | Nein |
| TKÜ (§ 100a StPO) | Ja (zwingend) | Nein | Nein |
| Onlinedurchsuchung (§ 100b StPO) | Ja (zwingend) | Nein | Nein |

> **GiV = Gefahr im Verzug**

### Gefahr im Verzug (GiV) — Was gilt?

**Voraussetzungen für GiV:**
- Konkrete Gefahr, dass Beweismittel vernichtet werden, bevor ein Richter erreicht werden kann
- Der Richter war nicht erreichbar (Dokumentation erforderlich)
- Die Maßnahme ist dringend und kann nicht aufgeschoben werden

**Nachfolgepflicht:** Nach einer GiV-Maßnahme muss die Staatsanwaltschaft (oder Polizei) unverzüglich — in der Praxis innerhalb von 3 Werktagen — einen richterlichen Beschluss erwirken. Ohne diesen wird die Maßnahme rückwirkend rechtswidrig. NetHost sollte in solchen Fällen verlangen, den Richterlicherbeschluss nachgereicht zu bekommen.

---

## 6. Besonderheiten für Domain-Registrare (ICANN)

### RDSAP — Registration Data System Access Protocol

ICANN verpflichtet akkreditierte Registrare durch den Registrar Accreditation Agreement (RAA) zu einem Prozess für den Zugang von Strafverfolgungsbehörden zu ansonsten nichtöffentlichen WHOIS-Daten (durch DSGVO nicht mehr öffentlich zugänglich).

**Der RDSAP-Prozess:**
1. Behörde stellt Anfrage über RDSAP-Kanal
2. NetHost prüft, ob Anfrage einem anerkannten Strafverfolgungszweck entspricht
3. NetHost entscheidet über Freigabe

> **Wichtig:** RDSAP läuft parallel zu deutschen Rechtspflichten. Auch wenn RDSAP eine Freigabe theoretisch ermöglicht, muss NetHost stets die deutschen DSGVO-Anforderungen und das TTDSG beachten. Im Zweifel: deutsche Rechtsgrundlage (§ 174 TKG oder § 22 TTDSG) verlangen.

### ccTLDs (.de) — DENIC-Schnittstelle

Für .de-Domains ist DENIC eG die Registry. Behördenanfragen für .de-WHOIS-Daten können auch direkt an DENIC gehen. NetHost als Registrar muss separat für die in seinem System gespeicherten Kundendaten entscheiden.

---

## 7. Auslandsbehörden und Internationales

### Europäische Ermittlungsanordnung (EEA / EIO)

Für Strafverfolgungsanfragen aus EU-Mitgliedstaaten gilt die Richtlinie 2014/41/EU (Europäische Ermittlungsanordnung). Der Prozess:

1. Ausländische Staatsanwaltschaft beantragt EIO in ihrem Mitgliedstaat
2. EIO geht an die deutsche Zentralbehörde (Bundesamt für Justiz / Bundesjustizministerium)
3. Deutsche Staatsanwaltschaft vollstreckt die EIO nach deutschem Recht
4. Deutsche Staatsanwaltschaft stellt förmliches Auskunftsersuchen an NetHost

**Konsequenz:** NetHost bekommt die Anfrage von einer deutschen Staatsanwaltschaft — nicht direkt aus dem Ausland. NetHost muss nicht selbst prüfen, ob die EIO korrekt ist.

### MLAT — Mutual Legal Assistance Treaty (Drittstaaten)

Für Drittstaaten (USA, UK, Australien etc.) gilt das Rechtshilfeverfahren (MLAT). Der Prozess ist analog: Auslandsbehörde → DOJ/gleichwertiges → Bundesjustizministerium → Staatsanwaltschaft → NetHost.

**US-Besonderheit — CLOUD Act:**
Der CLOUD Act (Clarifying Lawful Overseas Use of Data Act, 2018) verpflichtet US-Unternehmen, Daten auf Anfrage des US-DOJ herauszugeben — auch wenn die Daten in der EU gespeichert sind. NetHost ist ein deutsches Unternehmen ohne US-Nexus und daher direkt nicht betroffen. Wenn NetHost jedoch Teil einer US-Konzernstruktur wäre, müsste Legal eine CLOUD Act / DSGVO-Konfliktanalyse durchführen.

---

## 8. Checkliste für jede eingehende Behördenanfrage

### Schritt 1 — Erste Klassifikation (< 5 Minuten)
- [ ] Von wem kommt die Anfrage? (Richter / Staatsanwaltschaft / Polizei / Ausland / informell)
- [ ] Was wird angefragt? (Bestandsdaten / Inhaltsdaten / Verkehrsdaten / Echtzeit-TKÜ)
- [ ] Welche Rechtsgrundlage wird zitiert?
- [ ] Gibt es ein Aktenzeichen?
- [ ] Gibt es einen richterlichen Beschluss (bei beschlussbedürftigen Maßnahmen)?

### Schritt 2 — Formale Prüfung (< 10 Minuten)
- [ ] Hat die anfragende Behörde die Anordnungsbefugnis für diese Maßnahme?
- [ ] Ist die zitierte Rechtsgrundlage korrekt und auf die angeforderten Daten anwendbar?
- [ ] Ist der richterliche Beschluss vorhanden (wo erforderlich)?
- [ ] Ist der Beschluss noch gültig (nicht abgelaufen)?
- [ ] Stimmt der Umfang der Anfrage mit dem Beschluss überein?
- [ ] Ist die Anfrage von einer deutschen oder EU-MLAT/EIO-anerkannten Behörde?

### Schritt 3 — Entscheidung
- **COMPLY:** Alle formalen Voraussetzungen erfüllt → Daten herausgeben, dokumentieren
- **PARTIAL COMPLY:** Beschluss deckt nur Teil der Anfrage → nur beschlusskonformen Teil herausgeben
- **REFUSE:** Keine Rechtsgrundlage, falsche Behörde, fehlender Beschluss → ablehnen, Vorlage für Antwortschreiben
- **ESCALATE:** TKÜ-Beschluss, komplexer Auslandsfall, unklare Lage → Legal sofort

### Schritt 4 — Datensicherung (Legal Hold)
- [ ] Bei allen Beschlagnahme- und TKÜ-Beschlüssen: sofortiger Legal Hold auf betroffene Daten
- [ ] Internes Ticket öffnen: Legal Hold aktiv, Datum, Aktenzeichen
- [ ] Legal Hold erst aufheben, wenn Ermittlungsbehörde schriftlich bestätigt

### Schritt 5 — Dokumentation (DSGVO-Rechenschaft)
- [ ] Eingang der Anfrage loggen (Datum, Uhrzeit, Kanal)
- [ ] Entscheidung dokumentieren (Comply / Refuse / Partial)
- [ ] Herausgegebene Daten mit Hash dokumentieren
- [ ] Antwortschreiben archivieren
- [ ] Bearbeitende Person dokumentieren

---

## 9. Typische Fehler und wie man sie vermeidet

| Fehler | Konsequenz | Vermeidung |
|--------|-----------|------------|
| Comply auf informelle Polizeianfrage | DSGVO-Verstoß, Haftung gegenüber Kunden | Immer förmliches Ersuchen verlangen |
| Comply bei § 100g StPO-Anfrage ohne Richterbeschluss | Rechtswidrige Datenweitergabe | Richterlichen Beschluss immer verlangen |
| Herausgabe über Beschlussumfang hinaus | Unrechtmäßige Offenbarung | Beschluss Satz für Satz gegen Anfrage prüfen |
| Herausgabe an Auslandsbehörde direkt | Art. 44 ff. DSGVO-Verstoß | Immer MLAT/EIO-Verfahren verlangen |
| Abgelaufenen Beschluss vollziehen | Rechtswidrige Maßnahme, ggf. Haftung | Ablaufdatum jedes Beschlusses prüfen |
| Kunden während Ermittlungen benachrichtigen | Gefährdung des Ermittlungszwecks, strafbar | Keine Benachrichtigung ohne Freigabe der StA |
| Keine Dokumentation der Herausgabe | Keine DSGVO-Rechenschaft | Immer vollständiges Log führen |
