# AGIT Conversation Notes — Workflowleitfaden

> [!NOTE]
> **KI-Zusammenarbeit**
>
> Dieses Projekt nutzt KI-Unterstützung für Dokumentationspraktiken, abgegrenzte
> Workflows, Quellennachweise und Review. [COLLABORATION.md](COLLABORATION.md)
> dokumentiert die Maintainer-Autorität und die unversionierte Gesprächsquellenregel.

[English guide](TEMPLATE_README.md) · [Projekteinführung](README.de.md)

Dieser Leitfaden passt die geerbten Arbeitsregeln des AI Documentation Template an.
[PROJECT_CONTEXT.md](PROJECT_CONTEXT.md) hält verifizierte Herkunft,
Synchronisierungsbaseline und bewusste Abweichungen fest. Lokale AGENTS.md- und
Domänenregeln bleiben maßgeblich. Die Initialisierung ist abgeschlossen; geerbte
Einmalskills wurden entfernt. Der reguläre abgegrenzte Einstieg nutzt start-task.

## Inhalt

- [Gesprächsworkflow](#gesprächsworkflow)
- [Speicherung und Zugriff](#speicherung-und-zugriff)
- [Skills für die Zusammenarbeit](#skills-für-die-zusammenarbeit)
- [Render-Validierung und visuelle Inspektion](#render-validierung-und-visuelle-inspektion)
- [Git-Index und geschützte Git-Aktionen](#git-index-und-geschützte-git-aktionen)
- [Decision Records](#decision-records)
- [Repository und Tooling](#repository-und-tooling)
- [Lizenz](#lizenz)

## Gesprächsworkflow

Der [Skill draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md)
enthält Anweisungen für ausführliche deutsche thematische Zusammenfassungen als
persönliche Gedächtnisstütze. Er ordnet nicht
danach, wer was gesagt hat. Relevante Transkriptstellen dienen der Überprüfung;
Namen erscheinen nur, wo sie nötig sind. Ergebnisse, Beschlüsse, Aufgaben und
offene Fragen werden unterschieden, Unsicherheiten markiert, Vorschläge von
Beschlüssen getrennt und fehlende Angaben nicht erfunden.
Zuerst werden Unklarheiten durch nummerierte Kontextfragen in aufeinanderfolgenden
Blöcken von höchstens zehn Punkten geklärt. Danach bleiben wichtige Argumente,
Begründungen und Alternativen erhalten; Gesprächsdatum/Beteiligte werden festgehalten,
die Gliederung folgt den Inhalten. Sinnvolle Befunde/Hervorhebungen, Kategorien,
Tabellen und Übersichten sind optional; Nachweise stehen in kompakten Fußnoten.
Die vorläufige QMD wird nach dem ersten abgeschlossenen Testprojekt geprüft und
spätestens nach dem zweiten überarbeitet. Originalzitate
erscheinen nur bei wichtiger Formulierung oder verbleibender Unklarheit. Die
[generische QMD-Vorlage](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd)
wird an einem freigegebenen unversionierten Ort kopiert/befüllt. Beim
dokumentierten ersten Test sind Klärung, Entwurf und DOCX-Export abgeschlossen;
Durchsicht und Korrekturrückführung stehen noch aus.

Ein optionaler generischer Test kann einen kleinen fiktiven Ausschnitt extern nutzen:
geprüfte Struktur -> maßgebliche QMD -> DOCX -> Maintainer-Kommentare/Änderungen ->
akzeptierte Korrekturen in QMD -> geprüfter Neurender. Reale Dateien sind nicht nötig.

Für weitere generische Repository-Dokumente wird add-document ausdrücklich
aufgerufen. Vertrag und Navigation bleiben frei von Gesprächsinhalten; konkrete
Gespräche werden nicht im versionierten Katalog registriert.
[DOCUMENTATION_PROCESS.md](DOCUMENTATION_PROCESS.md) und
[FEEDBACK_WORKFLOW.md](FEEDBACK_WORKFLOW.md) definieren den laufenden Zyklus.

## Speicherung und Zugriff

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) ersetzt geerbte Speicher- und
Versionierungsdefaults. Alle Gesprächsdateien, JSON, Derivate, QMD, Ausgaben,
Review-Rückläufe, Snapshots, Nachweise, Logs und temporären Dateien bleiben
dauerhaft unversioniert und außerhalb von GitHub, auch fiktive Tests. Ignorierte
lokale Repository-Ablagen sind bei bewusster Zuordnung und geprüftem Git-Ausschluss
zulässig. Unversionierte QMD bleibt ohne Git-Historie maßgeblich. Gesprächsinhalte
gelangen niemals in versionierte Vorlagen, Dokumentation oder Projektaufzeichnungen;
sie werden niemals durch erzwungenes Hinzufügen versioniert.

Die ignorierte CONVERSATION_PATHS.local.md ordnet standardmäßig den dauerhaften
externen Sync-Speicher und das lokale ignorierte Repository-temp/conversation-work/
für Zwischenstände zu. Zugriff auf
konkrete Dateien und externe Schreibaktionen werden je Aufgabe freigegeben.
Nicht-sensitive Einstufung und Pfadzuordnung erlauben keinen Zugriff.
Sync-Speicher wird separat eingerichtet; Übermittlung, Weitergabe,
Veröffentlichung, Backup und Zugriff bleiben getrennte Entscheidungen.
Temporäre Inhalte werden nicht synchronisiert. Originale bleiben unverändert;
Arbeitsdateien/Nachweise bleiben extern. Revisionen gleichen den externen
Exportstand mit der aktuellen Quelle ab.

## Skills für die Zusammenarbeit

Skills sind abgegrenzte Arbeitsabläufe in [`.agents/skills/`](.agents/skills/).
Sie führen den Agenten durch eine bestimmte Aufgabe und laden dafür die
passenden Repository-Leitlinien. Rufe einen Skill im Chat mit `$skill-name`
auf, zum Beispiel `$review-project`. Die verlinkten Skill-Dateien beschreiben
den vollständigen Ablauf.

- **Agent oder explizit:** Der Agent darf den Skill bei einer passenden
  Aufgabe selbst auswählen; du kannst ihn auch direkt aufrufen.
- **Explizit:** Der Skill braucht einen bewussten Aufruf oder eine
  ausdrückliche Auswahl durch den Maintainer. Ein Vorschlag des Agenten
  aktiviert ihn noch nicht.
- **Aufgabenabhängig oder explizit:** Rendering darf aus einem Renderauftrag
  oder notwendiger Validierung folgen; freie implizite Skill-Auswahl ist
  ausgeschlossen. Ein direkter Aufruf bleibt möglich.

Die Auswahl eines Skills erteilt keine zusätzliche Freigabe für geschützte
Git-Aktionen, Installation, externe Übertragung oder Veröffentlichung. Die
lokalen Zugriffs- und Fachregeln gelten für jeden Ablauf.

In `commit-changes` umfasst eine explizite Commit-Freigabe den normalen Push zum
verifizierten bestehenden Upstream dieses Repositorys. In `commit-milestone`
umfasst eine explizite Meilenstein-Commit-Freigabe zusätzlich einen passenden
annotierten Versionstag und dessen gezielten Upstream-Push. „Nur Commit“ schließt
Tags und Pushes aus; „kein Push“ behält Commit/Tag lokal; „kein Tag“ schließt Tags
aus; „kein Tag-Push“ behält den Tag lokal. Andere Git-Aktionen, Tag-Verschiebung/
Ersetzung und Release-Publikation brauchen weiterhin eine eigene Freigabe.

`reuse-fixes` liest und ergänzt ausschließlich das Fehlerwissen dieses
Repositorys. Der Skill sammelt keine Erfahrungen über Repositories hinweg
und führt kein globales Fehlergedächtnis.
Aktive Lösungen stehen mit 4–8 Zeilen pro Fall in `TROUBLESHOOTING.md`.
[Ausführliche Belege](TROUBLESHOOTING_DETAILS.md) bleiben getrennt erhalten;
lies bei Bedarf nur den passenden Detailabschnitt.

| Skill | Aufruf | Zweck |
| --- | --- | --- |
| [`start-task`](.agents/skills/start-task/SKILL.md) | Agent oder explizit | Rekonstruiert nur den Kontext für eine neue abgegrenzte Aufgabe. |
| [`handoff-task`](.agents/skills/handoff-task/SKILL.md) | Agent oder explizit | Sichert Ergebnis, Evidenz und nächsten Schritt kompakt in `TASK_HANDOFF.md`. |
| [`commit-changes`](.agents/skills/commit-changes/SKILL.md) | Agent oder explizit | Erstellt einen regulären abgegrenzten Commit und führt den normalen Upstream-Push mit expliziter Commit-Freigabe aus, sofern der Push nicht ausgeschlossen wurde. |
| [`record-decision`](.agents/skills/record-decision/SKILL.md) | Agent oder explizit | Dokumentiert eine dauerhafte Entscheidung im passenden Record-Typ; Entscheidungen des Quelltemplates werden an Governance geroutet. |
| [`reuse-fixes`](.agents/skills/reuse-fixes/SKILL.md) | Agent oder explizit | Verwendet bestätigte Lösungen dieses Repositorys wieder, hält knappe Vorbeugung fest und fragt nur bei fehlender Freigabe oder blockierenden Entscheidungen nach. |
| [`review-project`](.agents/skills/review-project/SKILL.md) | Explizit | Erstellt eine umfassende neutrale Bestandsaufnahme des Projektzustands und der Evidenzlücken. |
| [`manage-external-storage`](.agents/skills/manage-external-storage/SKILL.md) | Explizit | Richtet optionalen externen Speicher ein, bindet einen Host an oder prüft ausgewählte lokale Dateien. |
| [`sync-template`](.agents/skills/sync-template/SKILL.md) | Explizit | Vergleicht ein abgeleitetes Projekt mit seinem verifizierten Quelltemplate und übernimmt ausgewählte Änderungen unter Erhalt der Projektanpassungen. |
| [`check-consistency`](.agents/skills/check-consistency/SKILL.md) | Explizit | Diagnostiziert interne Widersprüche zwischen Intention, Roadmap, Entscheidungen, Inhalten und Dokumentation und entwickelt abgegrenzte Optionen. |
| [`perform-retrospective`](.agents/skills/perform-retrospective/SKILL.md) | Explizit | Wertet Zusammenarbeitsevidenz aus und trennt Projektbefunde von wiederverwendbaren Template- oder Familienkandidaten. |
| [`add-document`](.agents/skills/add-document/SKILL.md) | Explizit | Ergänzt ein gepflegtes Dokument oder verknüpfte Sprachfassungen einschließlich Katalogmetadaten und Navigation. |
| [draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md) | Agent oder explizit | Klärt externe Transkripte in Blöcken von höchstens zehn Punkten und erstellt inhaltsgeleitete deutsche QMD mit Datum/Beteiligten, optionalen Hervorhebungen und Fußnoten. |
| [`render-document`](.agents/skills/render-document/SKILL.md) | Aufgabenabhängig oder explizit | Rendert gepflegte Quarto-Quellen in den benötigten Formaten und prüft technische Ergebnisse und Ablage. |
| [`revise-document`](.agents/skills/revise-document/SKILL.md) | Explizit | Wertet freigegebenes kommentiertes DOCX- oder PDF-Feedback aus und überträgt akzeptierte Revisionen in gepflegte Quellen. |
| [`review-document`](.agents/skills/review-document/SKILL.md) | Explizit | Prüft ein Dokument oder einen Abschnitt kritisch auf Korrektheit, erfolgreiche Bearbeitung der Leseraufgaben und Verständlichkeit; liefert belegte Befunde und Verbesserungsvorschläge. |
| [`visual-inspection`](.agents/skills/visual-inspection/SKILL.md) | Explizit | Prüft benannte aktuelle HTML-, PDF- oder DOCX-Renderings visuell und berichtet genauen Prüfumfang und Grenzen. |
| [`commit-milestone`](.agents/skills/commit-milestone/SKILL.md) | Explizit | Schließt einen geprüften Meilenstein mit Metadaten, umfassenden Prüfungen, Commit, annotiertem Versionstag und gezielten Upstream-Pushes ab, sofern nicht ausgeschlossen. |

### Optionale Planungsskills

`grill-me` und `grilling` sind übernommene MIT-lizenzierte Skills von Matt
Pocock. Sie ergänzen die eigenen Repository-Skills und werden ausschließlich
nach ausdrücklicher Auswahl verwendet. Der normale schlanke
Initialisierungsweg bleibt verfügbar.

| Skill | Aufruf | Zweck |
| --- | --- | --- |
| [`grill-me`](.agents/skills/grill-me/SKILL.md) | Explizit | Startet das optionale intensive Planungsinterview und leitet an `grilling` weiter. |
| [`grilling`](.agents/skills/grilling/SKILL.md) | Explizit | Prüft einen Plan, eine Entscheidung oder Idee in ausführlichen Interviewrunden; nur nach ausdrücklicher Auswahl. |

## Render-Validierung und visuelle Inspektion

Die routinemäßige Render- und Output-Validierung darf Quarto ausführen und das
erzeugte HTML technisch prüfen, ohne den Browser-Skill zu öffnen. Sie prüft je
nach Relevanz Build-Erfolg, Warnungen, erforderliche Dateien, HTML-Struktur,
Links, referenzierte Assets und offensichtlich nicht gerenderte Quellinhalte.
Das zählt nicht als visuelle Inspektion.

Rufe `$visual-inspection` ausdrücklich auf, wenn der Agent benannte aktuelle
Renders in durch den Maintainer gewählten Formaten inspizieren soll. Der Skill
öffnet gerendertes HTML mit dem Browser-Skill oder prüft ausgewählte PDF-/DOCX-
Seiten als Seitenbilder. Ein Milestone, Render oder eine visuelle Änderung löst
diesen Ablauf nicht aus. Fehlender Output wird weder gerendert noch ersetzt;
der Bericht benennt geprüfte Seiten, Routen, Viewports, Befunde und Grenzen.
Die visuelle Inspektion bestätigt weder Barrierefreiheit, technische
Korrektheit, Offenlegungsfreigabe noch Publikationsreife.

## Git-Index und geschützte Git-Aktionen

Der Maintainer kontrolliert die Git-Historie. Assistants dürfen Status, Diffs und Logs prüfen, Dokumentationsänderungen vorbereiten sowie Commit-Grenzen und -Metadaten vorschlagen.

Staging und Unstaging sind Indexoperationen. Sie benötigen kein Kontrollwort, dürfen aber nur nach einer konkreten Maintainer-Anweisung oder Autorisierung des zugehörigen Commits erfolgen. Bestehende Staging-Auswahlen und nicht zusammenhängende Änderungen müssen erhalten bleiben.

Geschützte Aktionen umfassen Commits, Amendments, Tags, Pushes, Pulls, Merges, Rebases, Resets, Branch-Wechsel, Stash-Manipulationen und andere Operationen an der Git-Historie. Ein Assistant darf eine bestimmte geschützte Aktion nur ausführen, wenn die Anweisung für genau diese Aktion `explicit` oder `explicitly` auf Englisch oder die deutsche Wortfamilie `explizit` enthält. Die Freigabe von Dateiänderungen autorisiert keine Änderung der Git-Historie; andere geschützte Aktionen brauchen weiterhin eine eigene Freigabe, mit den oben beschriebenen Commit-Abläufen als gezielten Ausnahmen.

Wenn diese Regel eine Autorisierung verlangt, schlägt der Assistant eine
minimal abgegrenzte, kopierfertige Anweisung vor, die genaue Aktion,
Repository und wesentliche Konsequenz benennt. Der Vorschlag selbst ist keine
Autorisierung.

Reguläre Dokumentations-Commits verwenden normalerweise `docs:` oder ein anderes passendes Conventional-Commit-Präfix. Milestone-Commits verzichten auf das Präfix, enthalten die abgeschlossene Version und schließen Dokumentation ab, die bereits in regulären Schritten entworfen, geprüft und korrigiert wurde.

## Decision Records

Wähle den Record-Typ nach dem Entscheidungsgegenstand:

- **DDR — Documentation Decision Record:** Informationsarchitektur, Zielgruppenannahmen, Terminologie, bilinguales Modell, Screenshot-Richtlinien, Linkmodell, visuelle Standards, Publikationsworkflow oder Milestone-Umfang.
- **PDR — Project Decision Record:** Projektumfang, Roadmap, Zusammenarbeit, Datenschutz, Quellen-Governance oder Repository-Struktur.
- **ADR — Architecture Decision Record:** Quarto-Struktur, Build-Pipeline, Tooling, Output-Modell, Automatisierung oder eine andere dauerhafte Entscheidung zum technischen Dokumentationssystem.

Vorlagen befinden sich in [decisions/](decisions/). Erstelle einen Record nur, wenn Begründung und Konsequenzen für künftige Maintainer relevant bleiben; gewöhnliche Formulierungsänderungen und Routinekorrekturen benötigen keinen.

## Repository und Tooling

[REPOSITORY.md](REPOSITORY.md) beschreibt die aktuelle Struktur. docs/ und
_quarto.yml enthalten nur generische Workflowdokumentation; optionale HTML-Ausgabe
bleibt ignoriert unter output/html/. Geerbte input-Leitlinien bleiben unverändert.
Repository-Ablagen dürfen Gesprächsdateien nur an bewusst zugeordneten,
ignorierten und unversionierten Orten aufnehmen. temp/conversation-work/ ist
die standardmäßige temporäre Ablage.

Quarto 1.9.38 und Pandoc 3.8.3 sind vorhanden. Einfache externe QMD -> DOCX braucht
kein TeX/R/Python. [QUARTO.md](QUARTO.md) beschreibt das externe Befehlsmuster,
das im fiktiven Test noch zu prüfen ist. Python/PyYAML wird separat für den
vorgeschriebenen Skill-Validator benötigt. Die separat freigegebene Clone-.venv
enthält nun Python 3.12.14/PyYAML 6.0.3; beide angepassten Skills bestanden.
Neue Clones nutzen [VALIDATION.md](VALIDATION.md) mit eigener Installationsfreigabe.
Optionale PDF- und visuelle Werkzeuge bleiben zurückgestellt.

CHANGELOG und TASK_HANDOFF enthalten nun projekteigenen Stand. Geerbter Backlog
und einmalige Setup-/Erzeugungsskills wurden entfernt; Setup-Provenienz bleibt.
Spätere Template-Synchronisierung verlangt den verifizierten ursprünglichen
Upstream-Commit; der importierte Snapshot wird nicht als dieser Commit ausgegeben.

## Lizenz

Das Repository behält seine [MIT-Lizenz](LICENSE), einschließlich des bestehenden
Copyrightvermerks von Christian Treffenstaedt. Template-Herkunft steht in
PROJECT_CONTEXT.md und ist keine eigene Projektversion oder Rechteerklärung.
Die erhaltenen grill-me/grilling-Skills von Matt Pocock behalten ihre MIT-Hinweise
in ihren Skillverzeichnissen. Die Repository-Lizenz erteilt keine Freigabe zur
Weitergabe oder Veröffentlichung von Gesprächsinhalten.
