# Leitfaden für Ratgeber-Artikel auf habitswap.de

Jeden Tag erscheint ein Artikel, auf Deutsch und auf Englisch. Beide Fassungen behandeln dasselbe Thema und sind über `ref` verknüpft. Die englische Fassung ist keine wörtliche Übersetzung, sondern für englischsprachige Leser geschrieben, mit eigenem Suchbegriff, eigenen Beispielen und Hilfsangeboten aus den USA und Großbritannien.

Qualität geht vor Menge. Google bewertet nicht die Häufigkeit, sondern ob ein Artikel die Frage des Lesers besser beantwortet als andere Seiten. Lieber einen Tag auslassen als einen schwachen Artikel veröffentlichen.

## Leser

Menschen zwischen 16 und 45, die eine Gewohnheit loswerden oder aufbauen wollen: Pornografie, Alkohol, Handy, Rauchen, Glücksspiel, Gaming, Zucker, Aufschieben. Viele sind Christen oder offen für den Glauben, manche nicht. Sie suchen bei Google eine ehrliche, konkrete Antwort und schämen sich oft für ihr Problem.

## Haltung

- Ehrlich, warm, ohne Moralkeule. Der Leser wird nicht beschämt.
- Hoffnung statt Druck: Veränderung ist möglich, Ausrutscher gehören dazu.
- Glaube als Einladung: Wo es passt, ein Abschnitt zum Glauben (Gnade, Gebet, Gemeinschaft, Metanoia). Echte Veränderung kommt aus einem neuen Herzen, das Gott schenkt, nicht aus eigener Kraft. Nie so, dass Nichtchristen sich ausgeschlossen fühlen.
- Deutsch duzt („du“), Englisch spricht den Leser mit „you“ an.

## Aufbau

1. Front Matter (siehe unten).
2. Ein bis zwei Absätze Einstieg, die das Problem des Lesers in seinen Worten aufgreifen und sagen, was der Artikel bringt. Keine Floskeln wie „In diesem Artikel erfährst du …“.
3. Gleich zu Beginn eine kurze, direkte Antwort auf die Suchfrage (zwei bis vier Sätze), damit Google sie als Ausschnitt nehmen kann.
4. Hauptteil mit `##`-Zwischenüberschriften, gern als Fragen, die Menschen wirklich suchen. Konkrete Schritte, Beispiele, kleine Szenen aus dem Alltag. Listen und eine Tabelle nur, wo sie wirklich helfen.
5. Ein Abschnitt zum Glauben, wo das Thema es hergibt (nicht erzwingen).
6. Habit Swap höchstens ein- bis zweimal natürlich erwähnen, wo die App wirklich zum Schritt passt (Ersatz-Plan, Notfall-Coach, Check-in, 90-Tage-Weg, Rechenschaftspartner, Gebetsgruppe). Keine Werbesprache. Der Kasten mit dem App-Store-Knopf kommt automatisch unter jeden Artikel.
7. Kurzer Schluss mit einem nächsten Schritt, den der Leser heute tun kann.

Länge: 1.300 bis 2.000 Wörter. Kürzer, wenn das Thema es nicht hergibt. Nichts strecken.

## Fakten und Quellen

- Keine erfundenen Zahlen, Studien oder Zitate. Wenn du dir bei einer Zahl nicht sicher bist, lass sie weg oder formuliere vorsichtig.
- Bekannte Belege, die verwendet werden dürfen, wenn sie passen: Lally u. a. 2010 (European Journal of Social Psychology, im Mittel 66 Tage bis zur Automatisierung, Spanne 18 bis 254), Wenn-dann-Pläne nach Gollwitzer (implementation intentions), Wendy Wood zu Gewohnheiten und Umgebung, HALT (hungry, angry, lonely, tired) aus der Suchthilfe, „Urge Surfing“ nach Alan Marlatt. Quellen im Text kurz nennen (Autor, Jahr, Zeitschrift), Links nur auf Seiten, deren Adresse du sicher kennst (z. B. Behörden wie bzga.de, nih.gov, nhs.uk, cdc.gov).
- Keine Heilversprechen, keine Diagnosen, keine Medikamentenempfehlungen. Bei Sucht auf Arzt und Suchtberatung verweisen.
- Bibelverse: Deutsch nur aus der Lutherbibel 1912 (gemeinfrei), Englisch aus der World English Bible (WEB) oder der King James Version. Stelle angeben (z. B. „Römer 12,2“ bzw. „Romans 12:2“). Kurze Zitate, nicht ganze Kapitel. Den genauen Wortlaut aus den Versdateien der App übernehmen, nicht aus dem Gedächtnis: `~/Developer/disziplin-app/lib/content/de/bible_verses.dart` (Luther 1912) und `~/Developer/disziplin-app/lib/content/en/bible_verses.dart` (WEB). Steht ein Vers dort nicht, nur zitieren, wenn der Wortlaut sicher ist, sonst sinngemäß mit Stellenangabe.

## Sprache

- Deutsch: nach den Regeln des Skills `vermenschlichen` (natürlich, sachlich, keine KI-typischen Wendungen, keine Gedankenstrich-Ketten, keine übertriebenen Adjektive, keine Dreierlisten aus Gewohnheit, keine rhetorischen Fragen als Füllstoff).
- Englisch: plain, warm American English, kurze Sätze, kein Marketing-Ton, keine Floskeln wie „In today’s fast-paced world“, „delve“, „game-changer“, „journey“ im Übermaß.
- Kurze Absätze (höchstens vier Sätze). Fettdruck sparsam.

## Suchbegriff

Jeder Artikel hat einen Hauptsuchbegriff (steht im Themenplan). Er gehört in den Titel, in die Beschreibung, in den ersten Absatz und in eine Zwischenüberschrift, ohne ihn unnatürlich zu wiederholen. Verwandte Begriffe und Fragen im Text abdecken.

## Front Matter

Deutsch, Datei `_posts/JJJJ-MM-TT-de-<slug>.md`:

```yaml
---
title: "Titel mit Suchbegriff (höchstens ca. 60 Zeichen)"
description: "Beschreibung für Google, 120 bis 155 Zeichen, mit Suchbegriff und Nutzen."
date: 2026-11-07
lang: de
ref: <gemeinsamer-schluessel>
permalink: /ratgeber/<slug>/
krise: true        # nur bei Sucht-, Scham- oder Krisenthemen: zeigt die Krisenhilfe
gesundheit: true   # bei Sucht- und Gesundheitsthemen: Hinweis auf Arzt/Beratung
---
```

Englisch, Datei `_posts/JJJJ-MM-TT-en-<slug>.md`: gleich aufgebaut, `lang: en`, `permalink: /en/guides/<slug>/`, gleicher `ref`, gleiches Datum.

Die Überschrift des Artikels kommt aus `title`, im Text daher keine `#`-Überschrift, nur `##` und `###`.

## Interne Links

Auf andere Artikel verlinken, aber nur auf solche, die es schon gibt oder die im selben Vorrat mit früherem oder gleichem Datum erscheinen (siehe Themenplan). Form: `[Ausrutscher richtig nehmen](/ratgeber/rueckfall/)`. Zur App höchstens einmal auf `/` bzw. `/en/` verlinken.

## Ablauf pro Woche

1. Claude schreibt den nächsten Vorrat (sieben Tage) nach dem Themenplan, Deutsch und Englisch.
2. Claude prüft jeden Artikel gegen diesen Leitfaden und baut die Seite lokal.
3. Andreas liest gegen und pusht. Die GitHub-Automatik schaltet jeden Morgen den Artikel des Tages frei.
