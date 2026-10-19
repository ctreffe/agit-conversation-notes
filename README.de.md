# AGIT Conversation Notes

> [!NOTE]
> **KI-Zusammenarbeit**
>
> KI unterstützt Workflowkonzeption und Projektdokumentation. Transkriptbasierte
> Entwürfe und Review bilden den vorgesehenen Ablauf.
> [COLLABORATION.md](COLLABORATION.md) dokumentiert Maintainer-Autorität,
> Quellennachweise, Revisionspraxis und die externe Speichergrenze.

[English](README.md)

## Workflows und Skills

Der [Workflowleitfaden](TEMPLATE_README.de.md) beschreibt verfügbare Skills und
Regeln. [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md) enthält den aktuellen Stand.
Die Initialisierung ist abgeschlossen; weitere abgegrenzte Arbeit nutzt start-task.

## Zweck

KI-gestützter Workflow zur Aufbereitung sprecherzugeordneter Transkripte in
strukturierte Gesprächsnotizen mit Quarto-Ausgaben und nachvollziehbarer Revision.
Whisper-v3 der Uni liefert JSON aus einvernehmlich aufgezeichneten Gesprächen.
Transkription und Sprecherzuordnung können fehlerhaft sein.

Ziel ist eine ausführliche deutsche thematische Aufbereitung der besprochenen
Inhalte, zunächst als persönliche Gedächtnisstütze. Wer welchen Satz gesagt hat,
bestimmt nicht die Struktur. Transkriptstellen ermöglichen Überprüfung; Namen
sind nur relevant, wo sie nötig sind, etwa für bestätigte Aufgaben.

## Ablauf

Externe JSON -> externe QMD -> externe DOCX zur Durchsicht -> akzeptierte
Kommentare/Änderungen zurück in die maßgebliche QMD -> geprüfter Neurender.

[draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md) klärt
zuerst Transkriptunklarheiten mit nummerierten Kontextfragen in Blöcken von
höchstens zehn Punkten und erstellt dann die deutsche thematische QMD.
Wichtige Argumente, Begründungen und Alternativen bleiben erhalten;
Wiederholungen und Gesprächsfüllwörter werden verdichtet. Gesprächsdatum und
Beteiligte stehen in einem kurzen Kopf. Die Gliederung folgt den Inhalten;
sinnvolle Befunde/Hervorhebungen, Kategorien und Übersichten sind optional.
Kompakte Fußnoten liefern Quellennachweise.
Klärungsantworten liefern zusätzlich knappe Erläuterungsfußnoten zu Fachbegriffen
und internen Zusammenhängen, wo sie das Verständnis erleichtern.
Die vorläufige QMD wird nach dem ersten
Testprojekt geprüft und spätestens nach dem zweiten überarbeitet.
Vorschläge werden nicht zu Beschlüssen, fehlende Angaben nicht erfunden. Die
[generische QMD-Vorlage](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd)
wird vor dem Befüllen an einen freigegebenen unversionierten Arbeitsort kopiert.
Der erste Gesprächstest hat einen QMD-Entwurf und DOCX erzeugt, die jetzt im
freigegebenen externen Sync-Projekt liegen; Durchsicht und Korrekturrückführung
stehen noch aus.

## Dauerhafte Versionierungsgrenze

Alle Gesprächsdateien bleiben dauerhaft unversioniert und außerhalb von GitHub:
JSON, Derivate, QMD, DOCX/PDF/HTML, kommentierte Kopien, Nachweise, Zwischenstände
und fiktive Testdateien. Sie dürfen innerhalb des Projektordners in bewusst
gewählten ignorierten Ablagen liegen. Die ausgewählte unversionierte QMD bleibt
maßgeblich. Der versionierte Git-Bestand enthält nur Skills,
Skripte, generische Vorlagen, Konfiguration und gesprächsfreie Projektdokumentation.

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) definiert diese bewusste
Docs-Template-Abweichung und die Klarstellung in PDR-0002. Die ignorierte
CONVERSATION_PATHS.local.md ordnet den dauerhaften externen Sync-Projektordner
und das lokale Repository-temp/conversation-work/ zu. Beide sind auf diesem Gerät
eingerichtet; der entfernte Synchronisationsstand ist ungeprüft. Weitere bewusst
zugeordnete ignorierte lokale Ablagen sind nach Prüfung des Git-Ausschlusses
zulässig. Konkreter Zugriff, externe Schreibaktionen, Sync-Übermittlung, Weitergabe
und Veröffentlichung bleiben getrennte Entscheidungen. Temporäre Dateien werden
nie synchronisiert; Gesprächsinhalte werden nie für einen Commit vorgemerkt,
committet oder durch erzwungenes Hinzufügen versioniert.

## Stand und nächster Schritt

Projektregeln und externe Render-/Revisionsanweisungen sind eingerichtet.
Quarto 1.9.38/Pandoc 3.8.3 sind vorhanden. Die separat freigegebene lokale
Validator-Umgebung enthält Python 3.12.14/PyYAML 6.0.3; beide angepassten Skills
und der neue Entwurfsskill sind validiert. Pandoc hat QMD-Struktur und Fußnoten
geparst. Ein ausgewähltes Transkript wurde geklärt und ein QMD-/DOCX-Entwurf
technisch geprüft. Maßgebliche QMD, DOCX und aufbewahrte Revisionsnachweise liegen
im freigegebenen externen Sync-Projekt; die Kopien sind per SHA-256 geprüft.
Seine Inhalte bleiben unversioniert; eine Veröffentlichung erfolgte nicht.
Der entfernte Synchronisationsstand ist ungeprüft.
Keine versionierte Projektetappe ist abgeschlossen.

Als Nächstes die DOCX durchsehen und akzeptierte Korrekturen in die maßgebliche
QMD zurückführen.
Der generische Testvertrag steht in [DOCUMENTS.md](DOCUMENTS.md), Voraussetzungen
in [DOCS_SETUP.md](DOCS_SETUP.md). Repository-docs/ enthält nur Workflowleitlinien.

## Lizenz

[MIT](LICENSE). Bestehende Copyright-/Herkunftshinweise bleiben erhalten.
Die Repository-Lizenz erlaubt keinen Zugriff oder Austausch von Gesprächsdateien.
