# skill-5-8-zusammenfassung

Paket von AIbex AIBOS mit dem Skill `5-8-zusammenfassung`, Version 1.3.0: gliedert ein Dokument zweistufig in je 5 bis 8 disjunkte, erschöpfende Themen und legt das Ergebnis als Memo im `@Memo/`-Ordner des Projekts ab.

## Holen

**Voraussetzung:** AIbex AIBOS v0.7 ist installiert, und der Vault ist an der Vault-Root mit `aibos --activate v0.7.<n>` gebunden (ein AIBOS-Workspace).

```bash
aibos --fetch skill-5-8-zusammenfassung
```

Das Paket braucht `skill-memo` (`~=6.1`); `aibos --fetch` holt es mit. Der Skill wirkt **ab dem nächsten Chat** im Projekt.

## Aufruf

Im Chat etwa „Mach eine 5-8-Zusammenfassung von `<dokument>`" oder `/5-8-zusammenfassung <dokument>`. Das Ergebnis ist ein Memo `NN <Titel> — 5-8-Zusammenfassung.md` in `@Memo/`.

Ab 1.2.0 kann ein Aufrufer, ein anderer Skill oder du im Chat, **Vorgaben** machen, jede einzeln: **Zielordner** (statt `@Memo/`, wird bei Bedarf angelegt), **Nummer** (statt eigener Vergabe), **Titel** und **nicht committen**. Beispiel: „Mach eine 5-8-Zusammenfassung von `<dokument>`, Zielordner `@Summary/`, Nummer `07`, Titel `Probe`, nicht committen". Eine bestehende Datei wird nie überschrieben.

## Lizenz

Apache License 2.0 (`LICENSE`), Rechteinhaber AIbex KG (`NOTICE`). Die Marken „AIbex" und „AIbex AIBOS" sind nicht mitlizenziert.
