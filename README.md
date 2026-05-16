# n8n-workflows

Öffentlich gehostete Demo-Workflows zu den n8n-Kursen von [Jan Kirenz](https://www.kirenz.com/).

Die JSON-Dateien lassen sich in einer beliebigen n8n-Instanz direkt per **Import from URL** importieren, ohne sie vorher herunterzuladen.

## Ordnerstruktur

- [`n8n-basics/`](./n8n-basics) — Workflows zum Kurs *n8n Grundlagen*

## Import in n8n

1. In n8n einen neuen, leeren Workflow anlegen.
2. Oben rechts auf das Drei-Punkte-Menü klicken.
3. **Import from URL** wählen.
4. Die Raw-URL der gewünschten JSON-Datei einfügen, etwa:

   ```
   https://raw.githubusercontent.com/kirenz/n8n-workflows/main/n8n-basics/modul-03-integrationen-switch.json
   ```

5. Bestätigen. Der Workflow erscheint im Editor mit allen Knoten und Verbindungen.

## Hinweis zu Credentials und Data Tables

Die Workflows enthalten keine Credentials. Für SMTP, IMAP, Google Gemini und ähnliche Knoten müssen die Credentials nach dem Import in der eigenen n8n-Instanz angelegt und im Knoten zugeordnet werden.

Data-Table-Knoten verweisen auf Tabellen-IDs, die in jeder n8n-Instanz lokal entstehen. Nach dem Import müssen die referenzierten Data Tables einmalig in der Zielinstanz angelegt und im Knoten neu ausgewählt werden.
