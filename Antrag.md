# Digital Mate: KI-Methoden für prozesssichere Automatisierung im OpenBIM

## Untertitel
Entwicklung eines auf Natursprache (NLP) basierenden, IFC-konformen KI-Frameworks zur Analyse, Adaption und Orchestrierung bestehender sowie Generierung neuer Automatisierungsskripte für die BIM-Umgebung.

## Projektbeschreibung
Die deutsche Bauwirtschaft ist geprägt von zahlreichen kleinen und mittleren Planungsbüros (KMU), die bei der Digitalisierung ihrer Arbeitsprozesse vor großen Herausforderungen stehen. Ihnen fehlen oft die Ressourcen für Forschung und Entwicklung, um moderne Automatisierungstechnologien zu nutzen. Die Planungslandschaft ist durch eine **heterogene Software-Vielfalt** gekennzeichnet, bei der jedes Büro auf spezifische, oft kostspielige Programme setzt. Gängige KI-basierte Werkzeuge liegen zumeist als proprietäre Plug-ins einzelner Softwarehersteller vor. Dies führt zu **isolierten Insellösungen**: Ein für Revit entwickeltes Automatisierungsskript zur Erstellung eines Raumbuchs kann beispielsweise in Archicad nicht verwendet werden.

Dies führt zu zwei Kernproblemen: Erstens müssen viele Büros die gleichen Automatisierungsaufgaben immer wieder neu entwickeln, während andere KMU gar nicht erst die Möglichkeit haben, solche Skripte zu erstellen. Zweitens sind selbst vorhandene Skripte (z.B. für Dynamo oder Python) oft starr und **projekt-spezifisch implementiert**. Sie müssen für jedes neue Bauvorhaben aufwendig manuell angepasst werden, da sich beispielsweise Bauteil- oder Geschossbezeichnungen ändern. Ein Austausch oder eine flexible Wiederverwendung ist kaum möglich. Schließlich mangelt es an **Vertrauen in automatisierte Prozesse**, wenn deren Auswirkungen nicht vorab geprüft und nachvollzogen werden können.

Dieses Vorhaben zielt darauf ab, KI-basierte Verfahren zu erforschen, mit denen Planungsanforderungen in **kontrollierbare und anpassungsfähige BIM-Workflows** überführt werden. Als Demonstrator wird ein software-unabhängiger Digital Mate prototypisch erstellt. Dieser soll Planungsaufgaben in natürlicher Sprache entgegennehmen, passende Skripte aus einer Bibliothek finden, diese **intelligent an das jeweilige Projekt anpassen** oder gänzlich neue Skripte generieren. Die daraus entstehenden Workflows werden dem Nutzer zur Verifikation (z. B. durch „Trockenläufe“ und visuelle „Diff“-Vergleiche) präsentiert, bevor sie prozesssicher auf beliebige IFC-basierte BIM-Modelle angewendet werden.

## Einordnung in den Stand des Wissens und der Praxis und Beitrag Ihres Projekts
Der Stand der Technik bei KI im Bauwesen fokussiert auf generative Einzelaufgaben in proprietären Ökosystemen. Großen Sprachmodellen (LLMs) fehlt der BIM-Modellkontext, um komplexe, mehrstufige Planungsprozesse zu orchestrieren. Bestehende skriptbasierte Automatisierungslösungen erfordern hohes Expertenwissen, während KI-Werkzeuge fehlen, die nativ auf dem offenen IFC-Standard operieren und zugleich vorhandene Skript-Bibliotheken eines Unternehmens integrieren. Zudem mangelt es an Methoden, die KI-Handlungen für Planer **transparent, kontrollierbar und verifizierbar** machen.
Das Projekt liefert drei zentrale Beiträge zur Überwindung dieser Defizite:

1.  **IFC-native Methodik gegen Insellösungen:** Durch die native Operation auf dem offenen IFC-Standard wird eine herstellerunabhängige Schnittstelle geschaffen, die in den heterogenen Softwarelandschaften von Planungsbüros nahtlos einsetzbar ist und die Interoperabilität fördert.
2.  **Dynamische Workflow-Synthese und -Adaption:** Ein neuartiges System analysiert bestehende Skripte (Dynamo, Python, C#), extrahiert Metadaten und legt sie in einer internen Bibliothek ab. Bei Nutzeranfragen werden daraus nicht nur passgenaue, mehrstufige Workflows generiert, sondern die Skripte werden bei Bedarf auch **intelligent an die spezifischen Gegebenheiten des neuen Zielprojekts angepasst**.
3.  **Vertrauen durch kontrollierbare Automatisierung:** Wir entwickeln Methoden für eine prozesssichere Automatisierung. Mittels **visueller "Diff"-Vergleiche**, die Änderungen am Modell hervorheben, und **"Trockenlauf"-Simulationen**, die das Ergebnis vor der Ausführung zeigen, wird die Modellintegrität sichergestellt und das Vertrauen der Nutzer in die KI-Anwendung gefördert.

## Ziel(e) des Projekts und erwartete Effekte
**Spezifische Forschungsziele:**
* **Entwicklung einer Methodik zur KI-Orchestrierung:** Kernziel ist die Erarbeitung einer Methodik, die hoch-abstrakte Planungsanweisungen in ausführbare Workflows übersetzt und so die Lücke zwischen menschlicher Intention und bestehenden oder neu generierten Automatisierungsskripten schließt.
* **Schaffung eines erweiterbaren, offenen Frameworks:** Die Systemarchitektur wird modular konzipiert, um per "Plug-and-Play" die Integration neuer Sprachmodelle und Skripte zu ermöglichen und die Zukunftsfähigkeit zu sichern.
* **Erarbeitung und Test von Interaktions-Paradigmen für eine vertrauenswürdige BIM-Automatisierung:** Es werden spezifische Methoden für die **Nachvollziehbarkeit und Kontrolle** (z.B. visuelle Diffs, Dry-Runs) evaluiert, um durch geeignete Interaktionen Vertrauen und prozesssichere Steuerung zu gewährleisten.
* **Implementierung eines prototypischen Evaluierungsinstruments:** Zur Validierung der Methoden wird ein "Digital Mate"-Prototyp implementiert, der als Forschungswerkzeug dient, um die Hypothesen in realen Anwendungsfällen zu testen und Ergebnisse zu verifizieren.

**Erwartete übergeordnete Effekte:**
* **Stärkung des OpenBIM-Gedankens und der Interoperabilität:** Durch die konsequente IFC-Ausrichtung wird die herstellerunabhängige Digitalisierung gefördert und die Zusammenarbeit in der Wertschöpfungskette Bau verbessert.
* **Steigerung von Planungsqualität und -effizienz:** Die Automatisierung von Routinen entlastet Planende, die sich auf kreative und komplexe Entscheidungen konzentrieren können, was zu höherer Qualität und beschleunigten Prozessen führt.
* **Erhöhung der Transparenz und des Vertrauens in KI:** Die erforschten Methoden zur Prozesskontrolle holen KI-gestützte Automatisierung aus einer Vertrauenslücke und schaffen die Grundlage für nachvollziehbare Assistenzsysteme, was die Akzeptanz in der Praxis erhöht.
* **Impuls für die Digitalisierung von KMU:** Das frei verfügbare Framework senkt die Einstiegshürden für kleine und mittlere Büros, um an fortschrittlichen Automatisierungstechnologien teilzuhaben und ihre Wettbewerbsfähigkeit zu steigern.

## Arbeitshypothese / Forschungsfrage
**Zentrale Arbeitshypothese:**
Die primäre Barriere für die breite Anwendung von KI-gestützter Automatisierung in der heterogenen deutschen Planungslandschaft ist nicht nur die Dominanz geschlossener Softwaresysteme, sondern vor allem das Fehlen einer Methode zur **intelligenten Adaption und Wiederverwendung von Skripten** über Projekt- und Softwaregrenzen hinweg sowie ein **Vertrauensdefizit in nicht verifizierbare Prozesse**. Wir postulieren, dass ein softwareunabhängiger, transparenter KI-Co-Pilot (Digital Mate), der auf Basis natürlicher Sprache nutzereigene Skripte orchestriert und adaptiert, die Effizienz und Akzeptanz signifikant steigern kann, indem er den Anwender in die volle Kontrolle über einen nachvollziehbaren Prozess versetzt.

**Zentrale Forschungsfragen:**
1.  Welche formalen Modelle und Repräsentationen sind erforderlich, um ambivalente, hoch-abstrakte Planungsanweisungen (natürliche Sprache) in deterministische, atomare Operationen auf einem schematisch strengen Datenmodell wie IFC zu überführen?
2.  Mit welchen Methoden der statischen und dynamischen Code-Analyse lässt sich das in imperativen Skripten (Python, Dynamo) enthaltene prozedurale Wissen extrahieren, um eine **automatische Anpassung an neue Projektkontexte** (z. B. geänderte Benennungskonventionen) zur Lösung komplexer Probleme zu ermöglichen?
3.  Welche **Interaktions- und Visualisierungsparadigmen** (z. B. Dry-Runs, Diff-Ansichten) sind notwendig, um einen verifizierbaren und vertrauenswürdigen Human-in-the-Loop-Prozess zu etablieren, der die Effizienz der Automatisierung mit der Notwendigkeit menschlicher Kontrolle und Validierung in Einklang bringt? Wie beeinflussen diese Paradigmen die Akzeptanz und Fehleranfälligkeit des Gesamtsystems?

## Forschungsmethodik
Die Methodik basiert auf einem iterativen Entwicklungs- und Validierungsprozess für ein modulares, KI-gesteuertes Framework. Dieser Ansatz gewährleistet eine kontinuierliche Rückkopplung mit der Praxis und sichert die Anwendbarkeit der Ergebnisse. Das Framework besteht aus vier zentralen, interagierenden Komponenten:
1.  **Generische IFC-Abstraktions-API:** Als Fundament wird eine softwareunabhängige Python-API entwickelt, die auf Open-Source-Bibliotheken (z.B. IfcOpenShell) aufbaut. Sie kapselt komplexe IFC-Operationen in standardisierte, aufgabenorientierte Befehle und dient als robuste Brücke zwischen der KI-Logik und der BIM-Datenstruktur.
2.  **Multimodales LLM als semantischer Übersetzer:** Ein Open-Source Large Language Model wird durch Fine-Tuning darauf trainiert, natürlichsprachliche Planungsanweisungen zu interpretieren. Es übersetzt diese in eine logische, maschinenlesbare Sequenz von Aktionen, die auf den Befehlen der IFC-API basieren.
3.  **Code-Mining zur Erstellung der Skript-Bibliothek:** Bestehende Automatisierungsskripte (Dynamo, Python) werden mittels statischer Code-Analyse und semantischer Vektorisierung prozessiert. Dabei werden Metadaten wie Inputs, Outputs und Kernfunktionalität extrahiert und in einer durchsuchbaren Vektordatenbank als intelligenter „Werkzeugkasten“ abgelegt.
4.  **Verifikations- und Orchestrierungs-Engine:** Diese Kernkomponente erhält die Aufgaben-Sequenz vom LLM sowie die Werkzeuge aus der Skript-Bibliothek und stellt daraus einen ausführbaren Workflow zusammen. Dieser wird dem Planer zur **Verifikation (inkl. "Trockenlauf" und "Diff"-Funktion)** präsentiert. Mittels Reinforcement Learning from Human Feedback (RLHF) werden die Vorschläge kontinuierlich optimiert.
Die Validierung erfolgt zyklisch in Workshops mit dem Praxispartner, in denen der Prototyp auf reale Planungsaufgaben angewendet wird.

## Eigene Vorarbeiten und Aktivitäten auf dem Forschungsgebiet
Das Projektkonsortium vereint langjährige praktische Erfahrung in der BIM-basierten Planung mit wissenschaftlicher Expertise im Bereich KI und digitaler Methoden.
Der Praxispartner verfügt über eine umfangreiche, praxiserprobte Bibliothek von Automatisierungsskripten (Dynamo, pyRevit), die reale Probleme lösen. Diese Sammlung bildet die initiale, validierte Datengrundlage für die Skript-Ingestion-Engine des „Digital Mate“. Erfahrungen in der Entwicklung von Entwurfswerkzeugen untermauern zudem die Kompetenz, komplexe Back-End-Logik in nutzerfreundliche Oberflächen zu überführen und gewährleisten die Praxisrelevanz.
Der wissenschaftliche Partner (Bauhaus-Universität Weimar, InfAR/InfAU) baut auf zahlreichen relevanten Forschungsprojekten auf:
* **DigiWo:** Entwicklung generativer Methoden zur automatisierten Erstellung von Gebäudekubaturen, was eine tiefe Expertise in der algorithmischen Verarbeitung von Planungslogik belegt.
* **Neufert 4.0:** Nutzung von maschinellem Lernen zur Ableitung von Entwurfsheuristiken aus 35.000 Grundrissen. Die Expertise in der Wissensextraktion ist Grundlage für das geplante Code-Mining.
* **ILCO (Integrierte Lebenszyklusoptimierung):** Schaffung eines modularen Software-Frameworks zur Kopplung von Analysewerkzeugen. Die Erfahrungen sind essentiell für die Entwicklung der Orchestrierungs-Engine.
* **KREMLAS:** Langjährige Forschung begründet die Kompetenz in der Entwicklung nutzerzentrierter Schnittstellen und interaktiver Planungswerkzeuge.
Diese Kombination aus praxiserprobter BIM-Automatisierung und akademischer Spitzenforschung qualifiziert das Team ideal, um die Brücke zwischen bestehenden Automatisierungsinseln und einem integrierten, intelligenten Gesamtprozess zu schlagen.

## Beschreibung der Arbeitspakete
* **AP 1: Projektmanagement und Koordination** - Umfasst die übergeordnete Planung, Steuerung und Durchführung des Projekts. Beinhaltet Risikomanagement, Koordination der Projektpartner, Finanzcontrolling sowie die Organisation von regelmäßigen Abstimmungsterminen und Workshops zur Sicherstellung der Projektziele.
* **AP 2: Anforderungsanalyse und Use-Case-Definition** - Detaillierte Analyse der Planungsprozesse im Partnerbüro zur Identifikation von relevanten, wiederkehrenden Aufgaben für die Automatisierung. Definition konkreter, praxisnaher Anwendungsfälle (Use Cases) und Ableitung der technischen und funktionalen Anforderungen an den Digital Mate.
* **AP 3: Entwicklung der IFC-Abstraktions-API** - Konzeption und Implementierung der softwareunabhängigen Schnittstelle für den Lese- und Schreibzugriff auf IFC-Daten. Sicherstellung der Kompatibilität mit den gängigen IFC-Versionen und Definition einer einheitlichen Datenstruktur für die interne Verarbeitung.
* **AP 4: Implementierung der Skript-Ingestion-Pipeline** - Entwicklung der Engine zum automatisierten Parsen, Analysieren und Katalogisieren der bestehenden Automatisierungsskripte (Dynamo, Python, C#). Aufbau der durchsuchbaren Skript-Bibliothek mittels Code-Mining und Vektorisierung.
* **AP 5: Training des LLM und der Orchestrierungs-Engine** - Fine-Tuning eines Open-Source LLM zur Übersetzung von natürlichsprachlichen Anweisungen in logische Task-Sequenzen. Entwicklung der Kern-Engine, die diese Sequenzen mit den Skripten aus AP4 zu einem ausführbaren Workflow zusammensetzt und das Framework zur Verifikation und Kontrolle implementiert.
* **AP 6: Prototyp-Integration und Pilottest** - Zusammenführung aller Komponenten zu einem lauffähigen Prototyp. Durchführung von Pilottests mit den in AP2 definierten Use Cases an realen Projektdaten. Sammlung von Nutzerfeedback zur iterativen Verbesserung.
* **AP 7: Dokumentation, Veröffentlichung und Transfer** - Laufende Dokumentation der Forschungsergebnisse. Erstellung von wissenschaftlichen Publikationen und Beiträgen für Fachmedien. Aufbereitung der Ergebnisse für den Abschlussbericht und Veröffentlichung des Frameworks als Open-Source-Software.

## Projektbeteiligte / Organisationsstruktur
Das Projekt ist ein Verbundvorhaben zwischen einem Planungsbüro als Praxispartner und einer Forschungseinrichtung als wissenschaftlichem Partner.
* **Projektkoordination:** Die Gesamtkoordination des Projekts liegt bei der Forschungseinrichtung, die für das wissenschaftliche Controlling, das Management und die Berichterstattung verantwortlich ist.
* **Forschungseinrichtung (Wissenschaftlicher Partner):** Verantwortlich für die Grundlagenforschung und die technische Entwicklung des Kern-Frameworks. Dies umfasst die Konzeption der Systemarchitektur, die Entwicklung der IFC-API (AP3), der Skript-Ingestion-Pipeline (AP4) sowie das Training des LLM und der Orchestrierungs-Engine (AP5). Zudem leitet sie die wissenschaftliche Dokumentation und Veröffentlichung (AP7).
* **Planungsbüro (Anwendungspartner):** Verantwortlich für die praxisnahe Fundierung des Projekts. Liefert die realen Anwendungsfälle (AP2), stellt die bestehende Skript-Bibliothek als Datengrundlage zur Verfügung und führt die Pilottests mit dem Prototyp an echten Bauprojekten durch (AP6). Das direkte Feedback aus der Planungspraxis stellt die Relevanz und Nutzbarkeit der entwickelten Lösung sicher.
Die Zusammenarbeit wird durch regelmäßige Arbeitstreffen und quartalsweise Meilenstein-Workshops gewährleistet, um einen kontinuierlichen Austausch zwischen Forschung und Anwendung sicherzustellen.

## Prioritäre Zielgruppe(n)
1.  **Kleine und mittlere Architektur- und Planungsbüros (KMU):** Dies ist die primäre Zielgruppe. Das Projekt will diesen Büros, die oft nicht über große IT-Budgets oder spezialisiertes Personal verfügen, einen Handlungsimpuls zur Steigerung ihres Digitalisierungsgrades geben. Das offene Werkzeug soll ihre Effizienz und Wettbewerbsfähigkeit direkt stärken.
2.  **Softwareentwickler und BIM-Dienstleister im AEC-Sektor:** Durch die Veröffentlichung des Frameworks als Open-Source-Projekt wird die Forschung und Entwicklung angeregt. Entwickler können das Framework als Basis nutzen, um eigene spezialisierte Dienste und Werkzeuge zu schaffen, die auf offenen Standards aufbauen.
3.  **Bildungs- und Forschungseinrichtungen:** Die Projektergebnisse, insbesondere die Methodik zur intelligenten Orchestrierung und Adaption von Skripten sowie das Framework zur Prozesskontrolle, liefern wertvolle Erkenntnisse und Lehrmaterial für die Ausbildung und weitere Forschung im Bereich der angewandten KI im Bauwesen.

## Ergebnisform und geplanter Transfer
Die Projektergebnisse werden zielgruppenspezifisch aufbereitet, um einen maximalen Transfer in Wissenschaft und Praxis sicherzustellen.
**Für die Planungspraxis / Industrie:**
* Ein funktionsfähiger Prototyp des OpenBIM-Copiloten (Digital Mate), der die Kernfunktionen demonstriert.
* Ein praxisorientierter Leitfaden zur Implementierung und Nutzung des Frameworks in Planungsbüros.
* Publikationen in deutschsprachigen Fachmedien (z.B. DETAIL, Bauwelt, Deutsches Architektenblatt), um praktizierende Architekten und Ingenieure zu erreichen.
* Präsentation der Ergebnisse auf einer führenden Branchenveranstaltung wie der BIM World MUNICH, um Entscheidungsträger und Unternehmen der Bauindustrie zu adressieren.

**Für die wissenschaftliche Community:**
* Mindestens eine wissenschaftliche Publikation in einer hochrangigen, begutachteten Fachzeitschrift (z.B. Automation in Construction).
* Vortrag auf einer internationalen wissenschaftlichen Konferenz (z.B. eCAADe).

**Für die Öffentlichkeit und Entwickler-Community:**
* Das entwickelte Kern-Framework, inklusive der IFC-API, wird als Open-Source-Software auf einer Plattform wie GitHub veröffentlicht, um die Weiternutzung und Weiterentwicklung durch Dritte zu fördern.
* Ein öffentlich zugänglicher Abschlussbericht, der die Projektergebnisse und Erkenntnisse aus den Praxistests verständlich zusammenfasst.

## Gesamtdauer des Projekts in Monaten
24

## Arbeits- und Zeitplan
Wird als separates PDF-Dokument (Balkenplan) angehängt.