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

## Geplanter Ablauf

Externe JSON -> externe QMD -> externe DOCX zur Durchsicht -> akzeptierte
Kommentare/Änderungen zurück in die maßgebliche QMD -> geprüfter Neurender.

Der geplante Skill draft-conversation-notes soll Ergebnisse, Beschlüsse, Aufgaben
und offene Fragen unterscheiden, Nachweise erhalten und Unsicherheiten markieren.
Vorschläge dürfen nicht zu Beschlüssen und fehlende Angaben nicht erfunden werden.
Skill und Protokollschema werden gemeinsam konzipiert; sie sind nicht implementiert.

## Dauerhafte Speichergrenze

Alle Gesprächsdateien bleiben außerhalb von Git und dauerhaft unversioniert:
JSON, Derivate, QMD, DOCX/PDF/HTML, kommentierte Kopien, Nachweise, Zwischenstände
und fiktive Testdateien. Externe QMD bleibt maßgeblich. Git enthält nur Skills,
Skripte, generische Vorlagen, Konfiguration und gesprächsfreie Projektdokumentation.

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) definiert diese bewusste
Docs-Template-Abweichung. Die ignorierte CONVERSATION_PATHS.local.md ordnet
externe Speicherorte zu und steht auf Unset. Konkreter Zugriff, externe
Schreibaktionen, Sync-Übermittlung, Weitergabe und Veröffentlichung bleiben
getrennte Entscheidungen. Sync-Einrichtung erfolgt später.

## Stand und nächster Schritt

Projektregeln und externe Render-/Revisionsanweisungen sind eingerichtet.
Quarto 1.9.38/Pandoc 3.8.3 sind vorhanden. Die separat freigegebene lokale
Validator-Umgebung enthält Python 3.12.14/PyYAML 6.0.3; beide Skills sind validiert.
Keine Verarbeitung realer Dateien, Gesprächsrenders, Git-Schreibaktion oder
Veröffentlichung erfolgte. Keine Projektversion/Etappe ist abgeschlossen.

Als Nächstes Skill/Schema gemeinsam konzipieren, dann einen kleinen fiktiven
Ausschnitt mit externer Speicherung, DOCX-Review und Korrekturrückführung prüfen.
Der generische Testvertrag steht in [DOCUMENTS.md](DOCUMENTS.md), Voraussetzungen
in [DOCS_SETUP.md](DOCS_SETUP.md). Repository-docs/ enthält nur Workflowleitlinien.

## Lizenz

[MIT](LICENSE). Bestehende Copyright-/Herkunftshinweise bleiben erhalten.
Die Repository-Lizenz erlaubt keinen Zugriff oder Austausch von Gesprächsdateien.
