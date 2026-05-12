---
date: Juli 2025
title: "![arc42](images/arc42-logo.png) Template"
---

# 

**Über arc42**

arc42, das Template zur Dokumentation von Software- und
Systemarchitekturen.

Template Version 9.0-DE. (basiert auf der AsciiDoc Version), Juli 2025

Created, maintained and © by Dr. Peter Hruschka, Dr. Gernot Starke and
contributors. Siehe <https://arc42.org>.

:::: note
::: title
:::

Diese Version des Templates enthält Hilfen und Erläuterungen. Sie dient
der Einarbeitung in arc42 sowie dem Verständnis der Konzepte. Für die
Dokumentation eigener System verwenden Sie besser die *plain* Version.
::::

# Einführung und Ziele {#section-introduction-and-goals}

Beschreibt die wesentlichen Anforderungen und treibenden Kräfte, die bei
der Umsetzung der Softwarearchitektur und Entwicklung des Systems
berücksichtigt werden müssen.

Dazu gehören:

-   zugrunde liegende Geschäftsziele,

-   wesentliche Aufgabenstellungen,

-   wesentliche funktionale Anforderungen,

-   Qualitätsziele für die Architektur und

-   relevante Stakeholder und deren Erwartungshaltung.

## Aufgabenstellung {#_aufgabenstellung}

::: formalpara-title
**Inhalt**
:::

Kurzbeschreibung der fachlichen Aufgabenstellung, treibenden Kräfte,
Extrakt (oder Abstract) der Anforderungen. Verweis auf (hoffentlich
vorliegende) Anforderungsdokumente (mit Versionsbezeichnungen und
Ablageorten).

::: formalpara-title
**Motivation**
:::

Aus Sicht der späteren Nutzung ist die Unterstützung einer fachlichen
Aufgabe oder Verbesserung der Qualität der eigentliche Beweggrund, ein
neues System zu schaffen oder ein bestehendes zu modifizieren.

::: formalpara-title
**Form**
:::

Kurze textuelle Beschreibung, eventuell in tabellarischer Use-Case Form.
Sofern vorhanden, sollte die Aufgabenstellung Verweise auf die
entsprechenden Anforderungsdokumente enthalten.

Halten Sie diese Auszüge so knapp wie möglich und wägen Sie Lesbarkeit
und Redundanzfreiheit gegeneinander ab.

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Anforderungen und Ziele](https://docs.arc42.org/section-1/) in
der online-Dokumentation (auf Englisch!).

## Qualitätsziele {#_qualitätsziele}

::: formalpara-title
**Inhalt**
:::

Die Top-3 bis Top-5 der Qualitätsanforderungen für die Architektur,
deren Erfüllung oder Einhaltung den maßgeblichen Stakeholdern besonders
wichtig sind. Gemeint sind hier wirklich Qualitätsziele, die nicht
unbedingt mit den Zielen des Projekts übereinstimmen. Beachten Sie den
Unterschied.

Hier ein Überblick möglicher Themen (basierend auf dem ISO 25010
Standard):

![Kategorien von
Qualitätsanforderungen](images/01_2_iso-25010-topics-DE.drawio.png)

::: formalpara-title
**Motivation**
:::

Weil Qualitätsziele grundlegende Architekturentscheidungen oft
maßgeblich beeinflussen, sollten Sie die für Ihre Stakeholder relevanten
Qualitätsziele kennen, möglichst konkret und operationalisierbar.

::: formalpara-title
**Form**
:::

Tabellarische Darstellung der Qualitätsziele mit möglichst konkreten
Szenarien, geordnet nach Prioritäten.

## Stakeholder {#_stakeholder}

::: formalpara-title
**Inhalt**
:::

Expliziter Überblick über die Stakeholder des Systems -- über alle
Personen, Rollen oder Organisationen --, die

-   die Architektur kennen sollten oder

-   von der Architektur überzeugt werden müssen,

-   mit der Architektur oder dem Code arbeiten (z.B. Schnittstellen
    nutzen),

-   die Dokumentation der Architektur für ihre eigene Arbeit benötigen,

-   Entscheidungen über das System und dessen Entwicklung treffen.

::: formalpara-title
**Motivation**
:::

Sie sollten die Projektbeteiligten und -betroffenen kennen, sonst
erleben Sie später im Entwicklungsprozess Überraschungen. Diese
Stakeholder bestimmen unter anderem Umfang und Detaillierungsgrad der
von Ihnen zu leistenden Arbeit und Ergebnisse.

::: formalpara-title
**Form**
:::

Tabelle mit Rollen- oder Personennamen, sowie deren Erwartungshaltung
bezüglich der Architektur und deren Dokumentation.

+-----------------+-----------------+-----------------------------------+
| Rolle           | Kontakt         | Erwartungshaltung                 |
+=================+=================+===================================+
| *\<Rolle-1\>*   | *\<Kontakt-1\>* | *\<Erwartung-1\>*                 |
+-----------------+-----------------+-----------------------------------+
| *\<Rolle-2\>*   | *\<Kontakt-2\>* | *\<Erwartung-2\>*                 |
+-----------------+-----------------+-----------------------------------+

# Randbedingungen {#section-architecture-constraints}

::: formalpara-title
**Inhalt**
:::

Randbedingungen und Vorgaben, die ihre Freiheiten bezüglich Entwurf,
Implementierung oder Ihres Entwicklungsprozesses einschränken. Diese
Randbedingungen gelten manchmal organisations- oder firmenweit über die
Grenzen einzelner Systeme hinweg.

::: formalpara-title
**Motivation**
:::

Für eine tragfähige Architektur sollten Sie genau wissen, wo Ihre
Freiheitsgrade bezüglich der Entwurfsentscheidungen liegen und wo Sie
Randbedingungen beachten müssen. Sie können Randbedingungen vielleicht
noch verhandeln, zunächst sind sie aber da.

::: formalpara-title
**Form**
:::

Einfache Tabellen der Randbedingungen mit Erläuterungen. Bei Bedarf
unterscheiden Sie technische, organisatorische und politische
Randbedingungen oder übergreifende Konventionen (beispielsweise
Programmier- oder Versionierungsrichtlinien, Dokumentations- oder
Namenskonvention).

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Randbedingungen](https://docs.arc42.org/section-2/) in der
online-Dokumentation (auf Englisch!).

# Kontextabgrenzung {#section-context-and-scope}

::: formalpara-title
**Inhalt**
:::

Die Kontextabgrenzung grenzt das System gegen alle Kommunikationspartner
(Nachbarsysteme und Benutzerrollen) ab. Sie legt damit die externen
Schnittstellen fest und zeigt damit auch die Verantwortlichkeit (scope)
Ihres Systems: Welche Verantwortung trägt das System und welche
Verantwortung übernehmen die Nachbarsysteme?

Differenzieren Sie fachlichen (Ein- und Ausgaben) und technischen
Kontext (Kanäle, Protokolle, Hardware), falls nötig.

::: formalpara-title
**Motivation**
:::

Die fachlichen und technischen Schnittstellen zur Kommunikation gehören
zu den kritischsten Aspekten eines Systems. Stellen Sie sicher, dass Sie
diese komplett verstanden haben.

::: formalpara-title
**Form**
:::

Verschiedene Optionen:

-   Diverse Kontextdiagramme

-   Listen von Kommunikationsbeziehungen mit deren Schnittstellen

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Kontextabgrenzung](https://docs.arc42.org/section-3/) in der
online-Dokumentation (auf Englisch!).

## Fachlicher Kontext {#_fachlicher_kontext}

::: formalpara-title
**Inhalt**
:::

Festlegung **aller** Kommunikationsbeziehungen (Nutzer, IT-Systeme, ...​)
mit Erklärung der fachlichen Ein- und Ausgabedaten oder Schnittstellen.
Zusätzlich (bei Bedarf) fachliche Datenformate oder Protokolle der
Kommunikation mit den Nachbarsystemen.

::: formalpara-title
**Motivation**
:::

Alle Beteiligten müssen verstehen, welche fachlichen Informationen mit
der Umwelt ausgetauscht werden.

::: formalpara-title
**Form**
:::

Alle Diagrammarten, die das System als Blackbox darstellen und die
fachlichen Schnittstellen zu den Nachbarsystemen beschreiben.

Alternativ oder ergänzend können Sie eine Tabelle verwenden. Der Titel
gibt den Namen Ihres Systems wieder; die drei Spalten sind:
Kommunikationsbeziehung, Eingabe, Ausgabe.

**\<Diagramm und/oder Tabelle\>**

**\<optional: Erläuterung der externen fachlichen Schnittstellen\>**

## Technischer Kontext {#_technischer_kontext}

::: formalpara-title
**Inhalt**
:::

Technische Schnittstellen (Kanäle, Übertragungsmedien) zwischen dem
System und seiner Umwelt. Zusätzlich eine Erklärung (*mapping*), welche
fachlichen Ein- und Ausgaben über welche technischen Kanäle fließen.

::: formalpara-title
**Motivation**
:::

Viele Stakeholder treffen Architekturentscheidungen auf Basis der
technischen Schnittstellen des Systems zu seinem Kontext.

Insbesondere bei der Entwicklung von Infrastruktur oder Hardware sind
diese technischen Schnittstellen durchaus entscheidend.

::: formalpara-title
**Form**
:::

Beispielsweise UML Deployment-Diagramme mit den Kanälen zu
Nachbarsystemen, begleitet von einer Tabelle, die Kanäle auf
Ein-/Ausgaben abbildet.

**\<Diagramm oder Tabelle\>**

**\<optional: Erläuterung der externen technischen Schnittstellen\>**

**\<Mapping fachliche auf technische Schnittstellen\>**

# Lösungsstrategie {#section-solution-strategy}

::: formalpara-title
**Inhalt**
:::

Kurzer Überblick über die grundlegenden Entscheidungen und
Lösungsansätze, die Entwurf und Implementierung des Systems prägen.
Hierzu gehören:

-   Technologieentscheidungen

-   Entscheidungen über die Top-Level-Zerlegung des Systems,
    beispielsweise die Verwendung gesamthaft prägender Entwurfs- oder
    Architekturmuster,

-   Entscheidungen zur Erreichung der wichtigsten Qualitätsanforderungen
    sowie

-   relevante organisatorische Entscheidungen, beispielsweise für
    bestimmte Entwicklungsprozesse oder Delegation bestimmter Aufgaben
    an andere Stakeholder.

::: formalpara-title
**Motivation**
:::

Diese wichtigen Entscheidungen bilden wesentliche „Eckpfeiler" der
Architektur. Von ihnen hängen viele weitere Entscheidungen oder
Implementierungsregeln ab.

::: formalpara-title
**Form**
:::

Fassen Sie die zentralen Entwurfsentscheidungen **kurz** zusammen.
Motivieren Sie, ausgehend von Aufgabenstellung, Qualitätszielen und
Randbedingungen, was Sie entschieden haben und warum Sie so entschieden
haben. Vermeiden Sie redundante Beschreibungen und verweisen Sie eher
auf weitere Ausführungen in Folgeabschnitten.

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Lösungsstrategie](https://docs.arc42.org/section-4/) in der
online-Dokumentation (auf Englisch!).

# Bausteinsicht {#section-building-block-view}

::: formalpara-title
**Inhalt**
:::

Die Bausteinsicht beschreibt die statische Struktur des Food-Truck-PoS-Systems.  
Das System ist in mehrere logisch getrennte Services und Komponenten aufgeteilt, um Skalierbarkeit, Wartbarkeit und Offline-Fähigkeit zu ermöglichen.

Das System besteht aus:

- lokalen Komponenten im Food Truck
- zentralen Backend-Services
- externen Drittanbieter-Systemen

Die wichtigsten Bausteine sind:

- PoS App
- Offline Sync Service
- Local Inventory Cache
- Order Service
- Payment Service
- Promotion Service
- Inventory Service
- Accounting Export Service
- Procurement Service
- Marketing Service
- Reporting Service

---

::: formalpara-title
**Motivation**
:::

Das Food-Truck-System muss auch bei schlechter oder fehlender Internetverbindung funktionieren.  
Gleichzeitig sollen zentrale Geschäftsprozesse wie:

- Zahlungsabwicklung
- Lagerverwaltung
- Buchhaltung
- Marketing
- Reporting

zentral verwaltet werden.

Die Architektur trennt daher:

- lokale Echtzeitfunktionen im Truck
- zentrale Geschäftslogik im Backend
- externe Integrationen

Dadurch wird:

- Offline-Betrieb ermöglicht
- Skalierbarkeit verbessert
- Wartung vereinfacht
- Erweiterbarkeit unterstützt

---

::: formalpara-title
**Form**
:::

Die Architektur wird als hierarchische Whitebox-/Blackbox-Struktur beschrieben.

- Ebene 1 zeigt die Hauptkomponenten des Gesamtsystems
- Ebene 2 beschreibt zentrale Services detaillierter
- Ebene 3 beschreibt interne Strukturen einzelner Services

---

## Whitebox Gesamtsystem {#_whitebox_gesamtsystem}

### Übersichtsdiagramm

*<Hier Bild der Bausteinsicht einfügen>*
[Diagramm](images/bausteinsicht.drawio.png)

---

### Begründung

Die Architektur folgt einer serviceorientierten Struktur.

Die wichtigsten Entscheidungen:

| Entscheidung | Begründung |
|---|---|
| Trennung zwischen Truck-System und Cloud-Backend | Offline-Fähigkeit und bessere Skalierbarkeit |
| Offline Sync Service | Synchronisierung bei instabiler Verbindung |
| Separater Inventory Service | Zentrale Lagerverwaltung |
| Separater Payment Service | Entkopplung von Zahlungslogik |
| Reporting Service liest Daten aus mehreren Services | Zentrale Analyse aller Geschäftsprozesse |
| Procurement Service getrennt | Nachbestellung von Waren |

---

### Enthaltene Bausteine

| Name | Verantwortung |
|---|---|
| PoS App | Benutzeroberfläche für Kassierer |
| Offline Sync Service | Synchronisierung lokaler Daten mit Backend |
| Local Inventory Cache | Lokaler Lagerbestand für Offline-Betrieb |
| Order Service | Verwaltung von Bestellungen |
| Payment Service | Zahlungsabwicklung |
| Promotion Service | Rabatt- und Angebotslogik |
| Inventory Service | Verwaltung des globalen Lagerbestands |
| Accounting Export Service | Export von Rechnungsdaten |
| Procurement Service | Automatische Warenbeschaffung |
| Marketing Service | Marketingkampagnen und Social-Media-Kommunikation |
| Reporting Service | Analyse und Reporting |
| External Payment Provider | Externer Zahlungsanbieter |
| Cloud TSE Service | Fiskalisierung und TSE-Signierung |
| Accounting System | Externes Buchhaltungssystem |
| External Supplier System | Lieferantenplattform |
| Social Media APIs | Social-Media-Integration |

---

## PoS App

### Zweck / Verantwortung

Die PoS App dient als Hauptoberfläche für den Kassierer im Food Truck.

Funktionen:

- Produktauswahl
- Preisberechnung
- Zahlungsstart
- Anzeige von Fehlermeldungen
- Bon-Anzeige
- Kommunikation mit Backend-Services

---

### Schnittstellen

| Schnittstelle | Beschreibung |
|---|---|
| Order API | Bestellung anlegen |
| Payment API | Zahlung starten |
| Promotion API | Rabatte berechnen |
| Sync API | Offline-Synchronisierung |
| Local Cache Access | Zugriff auf lokalen Lagerbestand |

---

### Qualitätsmerkmale

- Schnelle Reaktionszeit
- Offline-Fähigkeit
- Einfache Bedienbarkeit
- Touchscreen-Optimierung

---

## Offline Sync Service

### Zweck / Verantwortung

Der Offline Sync Service synchronisiert lokale Daten mit dem zentralen Backend.

Funktionen:

- Zwischenspeicherung von Bestellungen
- Wiederholung fehlgeschlagener Synchronisationen
- Synchronisierung des Lagerbestands

---

### Schnittstellen

| Schnittstelle | Beschreibung |
|---|---|
| Order Service API | Synchronisiert Bestellungen |
| Inventory Service API | Aktualisiert Lagerdaten |

---

### Qualitätsmerkmale

- Fehlertoleranz
- Wiederanlauf nach Verbindungsabbruch
- Asynchrone Verarbeitung

---

## Order Service

### Zweck / Verantwortung

Der Order Service verwaltet den gesamten Bestellprozess.

Funktionen:

- Bestellungen speichern
- Kommunikation mit TSE
- Lagerbestand reduzieren
- Buchhaltungsdaten exportieren

---

### Schnittstellen

| Schnittstelle | Beschreibung |
|---|---|
| Inventory API | Lagerbestand aktualisieren |
| TSE API | Fiskalische Signierung |
| Accounting Export API | Rechnungsdaten exportieren |

---

### Qualitätsmerkmale

- Hohe Zuverlässigkeit
- Konsistenz der Bestellungen
- Transaktionssicherheit

---

## Inventory Service

### Zweck / Verantwortung

Der Inventory Service verwaltet den zentralen Lagerbestand aller Trucks.

Funktionen:

- Lagerbestand aktualisieren
- Nachbestellungen auslösen
- Bestandsanalysen

---

### Schnittstellen

| Schnittstelle | Beschreibung |
|---|---|
| Procurement API | Waren nachbestellen |
| Reporting API | Lagerdaten bereitstellen |

---

## Reporting Service

### Zweck / Verantwortung

Der Reporting Service sammelt Daten aus mehreren Services.

Funktionen:

- Umsatzanalyse
- Verkaufsstatistiken
- Rabattanalysen
- Lageranalysen

---

### Schnittstellen

| Schnittstelle | Beschreibung |
|---|---|
| Order Service | Verkaufsdaten |
| Promotion Service | Rabattdaten |
| Inventory Service | Lagerdaten |

---

# Laufzeitsicht {#section-runtime-view}

::: formalpara-title
**Inhalt**
:::

Die Laufzeitsicht beschreibt den Ablauf eines Verkaufs im Food Truck.

Dabei wird gezeigt:

- wie Services miteinander kommunizieren
- wie Zahlungen verarbeitet werden
- wie Bestellungen gespeichert werden
- wie Lager und Buchhaltung aktualisiert werden

---

::: formalpara-title
**Motivation**
:::

Die Laufzeitsicht hilft beim Verständnis der dynamischen Zusammenarbeit der Komponenten.

Besonders wichtig sind:

- Reihenfolge der Aufrufe
- Fehlerbehandlung
- Synchronisation
- externe Integrationen

---

## Verkaufsvorgang am Food Truck {#_verkaufsvorgang_foodtruck}

### Sequenzdiagramm

*<Hier Bild des Sequenzdiagramms einfügen>*
[Diagramm](images/laufzeitsicht.png)

---

### Beschreibung des Szenarios

1. Der Kassierer wählt Produkte aus.
2. Die PoS App fragt Rabatte beim Promotion Service an.
3. Der Kassierer startet die Zahlung.
4. Der Payment Service kommuniziert mit dem externen Zahlungsanbieter.
5. Bei erfolgreicher Zahlung:
   - wird die Bestellung gespeichert
   - die TSE-Signatur erstellt
   - der Lagerbestand reduziert
   - die Buchhaltung aktualisiert
6. Danach wird die Bestellung synchronisiert.
7. Abschließend wird der Bon angezeigt oder gedruckt.

Bei fehlgeschlagener Zahlung wird eine Fehlermeldung angezeigt.

---

# Verteilungssicht {#section-deployment-view}

::: formalpara-title
**Inhalt**
:::

Die Verteilungssicht beschreibt die technische Infrastruktur des Systems.

Das System besteht aus:

- mobilen Geräten im Food Truck
- zentralem Cloud-Backend
- externen Cloud-Systemen

---

::: formalpara-title
**Motivation**
:::

Die Verteilung ist entscheidend für:

- Offline-Fähigkeit
- Skalierbarkeit
- Cloud-Integration
- mobile Nutzung
- externe Schnittstellen

---

## Infrastruktur Ebene 1 {#_infrastruktur_ebene_1}

### Übersichtsdiagramm

*<Hier Bild der Verteilungssicht einfügen>*
[Diagramm](images/verteilungssicht.png)


---

### Begründung

Die Infrastruktur wurde so gestaltet, dass:

- der Food Truck mobil arbeiten kann
- Offline-Betrieb möglich ist
- zentrale Daten konsistent bleiben
- externe Dienste integriert werden können

---

### Qualitäts- und Leistungsmerkmale

| Merkmal | Beschreibung |
|---|---|
| Offline-Fähigkeit | Lokale Speicherung im Truck |
| Skalierbarkeit | Cloud-Backend kann horizontal erweitert werden |
| Wartbarkeit | Serviceorientierte Struktur |
| Fehlertoleranz | Synchronisierung bei Netzwerkausfällen |
| Erweiterbarkeit | Neue Services können ergänzt werden |

---

### Zuordnung von Bausteinen zu Infrastruktur

| Infrastruktur | Zugeordnete Bausteine |
|---|---|
| Tablet / PoS Device | PoS App, Offline Sync Service, Local Inventory Cache |
| Backend Server | Alle zentralen Services |
| PostgreSQL Database | Persistenz der Geschäftsdaten |
| External Systems | Zahlungsanbieter, TSE, Buchhaltung, Lieferanten |

---

## Infrastruktur Ebene 2 {#_infrastruktur_ebene_2}

### Tablet / PoS Device

Der Tablet-/PoS-Bereich enthält:

- Benutzeroberfläche
- lokale Synchronisierung
- lokalen Lagercache

Diese Komponenten müssen performant und offlinefähig sein.

---

### Cloud Backend

Das Cloud Backend enthält:

- zentrale Geschäftslogik
- Datenpersistenz
- externe Integrationen

Die Services laufen innerhalb eines NestJS-Servers.

---

### External Systems

Externe Systeme werden über APIs angebunden:

- Payment APIs
- TSE APIs
- Export APIs
- Social APIs

Diese Systeme liegen außerhalb der direkten Kontrolle des Unternehmens.

# Querschnittliche Konzepte {#section-concepts}

::: formalpara-title
**Inhalt**
:::

Dieser Abschnitt beschreibt übergreifende, prinzipielle Regelungen und
Lösungsansätze, die an mehreren Stellen (=*querschnittlich*) relevant
sind.

Solche Konzepte betreffen oft mehrere Bausteine. Dazu können vielerlei
Themen gehören, wie beispielsweise die Themen aus dem nachfolgenden
Diagramm:

![Mögliche Themen für querschnittliche
Konzepte](images/08-concepts-DE.drawio.png)

::: formalpara-title
**Motivation**
:::

Konzepte bilden die Grundlage für *konzeptionelle Integrität*
(Konsistenz, Homogenität) der Architektur und damit eine wesentliche
Grundlage für die innere Qualität Ihrer Systeme.

Dieser Abschnitt im Template ist der richtige Ort für die konsistente
Behandlung solcher Themen.

Viele solche Konzepte beeinflussen oder beziehen sich auf mehrerer Ihrer
Bausteine.

::: formalpara-title
**Form**
:::

Kann vielfältig sein:

-   Konzeptpapiere mit beliebiger Gliederung,

-   beispielhafte Implementierung speziell für technische Konzepte,

-   übergreifende Modelle/Szenarien mit Notationen, die Sie auch in den
    Architektursichten nutzen,

::: formalpara-title
**Struktur**
:::

Wählen Sie **nur** die wichtigsten Themen für Ihr System und erklären
das jeweilige Konzept dann unter einer Level-2 Überschrift dieser
Sektion (z.B. 8.1, 8.2 etc).

Beschränken Sie sich auf die wichtigen, und versuchen **auf keinen
Fall** alle oben dargestellten Themen zu bearbeiten.

::: formalpara-title
**Weiterführende Informationen**
:::

Einige Themen innerhalb von Systemen betreffen oft mehrere Bausteine,
Hardwareelemente oder Prozesse. Es könnte einfacher sein, solche
*Querschnittsthemen* an einer zentralen Stelle zu kommunizieren oder zu
dokumentieren, anstatt sie in der Beschreibung der betreffenden
Bausteine, Hardwareelemente oder Entwicklungsprozesse zu wiederholen.

Bestimmte Konzepte können **alle** Elemente eines Systems betreffen,
andere sind vielleicht nur für einige wenige relevant.

Siehe [Querschnittliche Konzepte](https://docs.arc42.org/section-8/) in
der online-Dokumentation (auf Englisch).

## *\<Konzept 1\>* {#_konzept_1}

*\<Erklärung\>*

## *\<Konzept 2\>* {#_konzept_2}

*\<Erklärung\>*

...​

## *\<Konzept n\>* {#_konzept_n}

*\<Erklärung\>*

# Architekturentscheidungen {#section-design-decisions}

::: formalpara-title
**Inhalt**
:::

Wichtige, teure, große oder riskante Architektur- oder
Entwurfsentscheidungen inklusive der jeweiligen Begründungen. Mit
\"Entscheidungen\" meinen wir hier die Auswahl einer von mehreren
Alternativen unter vorgegebenen Kriterien.

Wägen Sie ab, inwiefern Sie Entscheidungen hier zentral beschreiben,
oder wo eine lokale Beschreibung (z.B. in der Whitebox-Sicht von
Bausteinen) sinnvoller ist. Vermeiden Sie Redundanz. Verweisen Sie evtl.
auf Abschnitt 4, wo schon grundlegende strategische Entscheidungen
beschrieben wurden.

::: formalpara-title
**Motivation**
:::

Stakeholder des Systems sollten wichtige Entscheidungen verstehen und
nachvollziehen können.

::: formalpara-title
**Form**
:::

Verschiedene Möglichkeiten:

-   ADR ([Documenting Architecture
    Decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions))
    für jede wichtige Entscheidung

-   Liste oder Tabelle, nach Wichtigkeit und Tragweite der
    Entscheidungen geordnet

-   ausführlicher in Form einzelner Unterkapitel je Entscheidung

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Architekturentscheidungen](https://docs.arc42.org/section-9/) in
der arc42 Dokumentation (auf Englisch!). Dort finden Sie Links und
Beispiele zum Thema ADR.

# Qualitätsanforderungen {#section-quality-scenarios}

::: formalpara-title
**Inhalt**
:::

Dieser Abschnitt enthält alle relevanten Qualitätsanforderungen.

Die wichtigsten davon haben Sie bereits in Abschnitt 1.2
(Qualitätsziele) hervorgehoben, daher soll hier nur auf sie verwiesen
werden. In diesem Abschnitt 10 sollten Sie auch Qualitätsanforderungen
mit geringerer Bedeutung erfassen, deren Nichterfüllung keine großen
Risiken birgt (die aber *nice-to-have* sein könnten).

::: formalpara-title
**Motivation**
:::

Weil Qualitätsanforderungen die Architekturentscheidungen oft maßgeblich
beeinflussen, sollten Sie die für Ihre Stakeholder relevanten
Qualitätsanforderungen kennen, möglichst konkret und operationalisiert.

-   Siehe [Qualitätsanforderungen](https://docs.arc42.org/section-10/)
    in der online-Dokumentation (auf Englisch!).

-   Siehe auch das ausführliche [Q42 Qualitätsmodell auf
    https://quality.arc42.org](https://quality.arc42.org).

## Übersicht der Qualitätsanforderungen {#_übersicht_der_qualitätsanforderungen}

::: formalpara-title
**Inhalt**
:::

Eine Übersicht oder Zusammenfassung der Qualitätsanforderungen.

::: formalpara-title
**Motivation**
:::

Oft stößt man auf Dutzende (oder sogar Hunderte) von detaillierten
Qualitätsanforderungen für ein System. In diesem Abschnitt sollten Sie
versuchen, sie zusammenzufassen, z. B. durch die Beschreibung von
Kategorien oder Themen (wie z.B. von [ISO
25010:2023](https://www.iso.org/obp/ui/#iso:std:iso-iec:25010:ed-2:v1:en)
oder [Q42](https://quality.arc42.org) vorgeschlagen).

Wenn diese Kurzbeschreibungen oder Zusammenfassungen bereits präzise,
spezifisch und messbar sind, können Sie Abschnitt 10.2 auslassen.

::: formalpara-title
**Form**
:::

Verwenden Sie eine einfache Tabelle, in der jede Zeile eine Kategorie
oder ein Thema und eine kurze Beschreibung der Qualitätsanforderung
enthält. Alternativ können Sie auch eine Mindmap verwenden, um diese
Qualitätsanforderungen zu strukturieren. In der Literatur (insb.
\[Bass+21\]) ist die Idee eines *Quality Attribute Utility Tree* (auf
Deutsch manchmal kurz als *Qualitätsbaum* bezeichnet) beschrieben
worden, der den Oberbegriff „Qualität" als Wurzel hat und eine
baumartige Verfeinerung des Begriffs „Qualität" verwendet.

## Qualitätsszenarien {#_qualitätsszenarien}

::: formalpara-title
**Inhalt**
:::

Qualitätsszenarien konkretisieren Qualitätsanforderungen und ermöglichen
es zu entscheiden, ob sie erfüllt sind (im Sinne von
Akzeptanzkriterien). Stellen Sie sicher, dass Ihre Szenarien spezifisch
und messbar sind.

Zwei Arten von Szenarien finden wir besonders nützlich:

-   Nutzungsszenarien (auch bekannt als Anwendungs- oder
    Anwendungsfallszenarien) beschreiben, wie das System zur Laufzeit
    auf einen bestimmten Auslöser reagieren soll. Hierunter fallen auch
    Szenarien zur Beschreibung von Effizienz oder Performance. Beispiel:
    Das System beantwortet eine Benutzeranfrage innerhalb einer Sekunde.

-   Änderungsszenarien\_ beschreiben die gewünschte Wirkung einer
    Änderung oder Erweiterung des Systems oder seiner unmittelbaren
    Umgebung. Beispiel: Zusätzliche Funktionalität wird implementiert
    oder Anforderungen an ein Qualitätsmerkmal ändern sich, und der
    Aufwand oder die Dauer der Änderung wird gemessen.

::: formalpara-title
**Form**
:::

Typische Informationen für detaillierte Szenarien sind die folgenden:

In Kurzform (bevorzugt im Q42-Modell):

-   K**ontext/Hintergrund**: Um welche Art von System oder Komponente
    handelt es sich, wie sieht die Umgebung oder Situation aus?

-   **Quelle/Stimulus**: Wer oder was initiiert oder löst ein Verhalten,
    eine Reaktion oder eine Aktion aus.

-   **Metrik/Akzeptanzkriterien**: Eine Reaktion einschließlich einer
    *Maßnahme* oder *Metrik*

Die Langform von Szenarien (die von der SEI und \[Bass+21\] bevorzugt
wird) ist detaillierter und enthält die folgenden Informationen:

-   **Szenario-ID**: Ein eindeutiger Bezeichner für das Szenario.

-   **Szenario-Name**: Ein kurzer, beschreibender Name für das Szenario.

-   **Quelle**: Die Entität (Benutzer, System oder Ereignis), die das
    Szenario auslöst.

-   **Stimulus**: Das auslösende Ereignis oder die Bedingung, auf die
    das System reagieren muss.

-   **Umgebung**: Der betriebliche Kontext oder die Bedingungen, unter
    denen das System den Stimulus erlebt.

-   **Artefakt**: Die Bausteine oder anderen Elemente des Systems, die
    von dem Stimulus betroffen sind.

-   **Reaktion**: Das Ergebnis oder Verhalten, das das System als
    Reaktion auf den Stimulus zeigt.

-   **Antwortmaß**: Das Kriterium oder die Metrik, nach der die Antwort
    des Systems bewertet wird.

::: formalpara-title
**Beispiele**
:::

Ausführliche Beispiele für Qualitätsanforderungen finden Sie auf [der
Website zum Qualitätsmodell Q42](https://quality.arc42.org).

-   Len Bass, Paul Clements, Rick Kazman: „Software Architecture in
    Practice", 4. Auflage, Addison-Wesley, 2021.

# Risiken und technische Schulden {#section-technical-risks}

::: formalpara-title
**Inhalt**
:::

Eine nach Prioritäten geordnete Liste der erkannten Architekturrisiken
und/oder technischen Schulden.

> Risikomanagement ist Projektmanagement für Erwachsene.
>
> ---  Tim Lister Atlantic Systems Guild

Unter diesem Motto sollten Sie Architekturrisiken und/oder technische
Schulden gezielt ermitteln, bewerten und Ihren Management-Stakeholdern
(z.B. Projektleitung, Product-Owner) transparent machen.

::: formalpara-title
**Form**
:::

Liste oder Tabelle von Risiken und/oder technischen Schulden, eventuell
mit vorgeschlagenen Maßnahmen zur Risikovermeidung, Risikominimierung
oder dem Abbau der technischen Schulden.

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Risiken und technische
Schulden](https://docs.arc42.org/section-11/) in der
online-Dokumentation (auf Englisch!).

# Glossar {#section-glossary}

::: formalpara-title
**Inhalt**
:::

Die wesentlichen fachlichen und technischen Begriffe, die Stakeholder im
Zusammenhang mit dem System verwenden.

Nutzen Sie das Glossar ebenfalls als Übersetzungsreferenz, falls Sie in
mehrsprachigen Teams arbeiten.

::: formalpara-title
**Motivation**
:::

Sie sollten relevante Begriffe klar definieren, so dass alle Beteiligten

-   diese Begriffe identisch verstehen, und

-   vermeiden, mehrere Begriffe für die gleiche Sache zu haben.

::: formalpara-title
**Form**
:::

Zweispaltige Tabelle mit \<Begriff\> und \<Definition\>.

Eventuell weitere Spalten mit Übersetzungen, falls notwendig.

::: formalpara-title
**Weiterführende Informationen**
:::

Siehe [Glossar](https://docs.arc42.org/section-12/) in der
online-Dokumentation (auf Englisch!).

+----------------------+-----------------------------------------------+
| Begriff              | Definition                                    |
+======================+===============================================+
| *\<Begriff-1\>*      | *\<Definition-1\>*                            |
+----------------------+-----------------------------------------------+
| *\<Begriff-2*        | *\<Definition-2\>*                            |
+----------------------+-----------------------------------------------+
