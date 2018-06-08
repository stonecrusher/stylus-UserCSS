# Beschreibung

Neuer Style für zeit.de - realisiert durch CSS, welches durch ein Browseraddon wie [Stylus](https://add0n.com/stylus.html) injiziert wird.

"Mobile first" ist leider häufig falsch umgesetzt und am Desktop nicht zu gebrauchen - die Seiten werden unerträglich lang.  
Dieser UserStyle ist meine Art, um mit den lächerlich riesigen Teaser-Bildern und den enormen Überschriften umzugehen.

Artikelseiten mit Kommentaren sind ca. 33% kürzer. Der Style ist nicht auf Schönheit ausgelegt, sondern um etwas mehr Übersicht zu schaffen.


## Optionen:
- Kommentare entfernen
- Teaserbild auf Artikelseiten entfernen
- Videobereich entfernen
- Seitlichen "Beliebte Artikel"-Kasten entfernen (bleibt weiter unten auf der Hauptseite erhalten)
- ZeitPLUS Artikel entfernen
- Seitliche Navigation zum "nächsten Artikel" entfernen
- Aktualisierungsbenachrichtigung entfernen
- Header minimieren (Achtung: Entfernt auch Suche und Login!)



# Installation

[![Install directly with Stylus](https://img.shields.io/badge/Install%20directly%20with-Stylus-238b8b.svg)](https://github.com/stonecrusher/UserCSS-zeit/raw/master/zeit-condensed.user.css)



# Weitere Informationen


## Erweiterte Blockierregeln für uBlock Origin

Stylus kann Elemente nur per CSS ausblenden, was gewisse Beschränkungen mit sich bringt. Mit uBlock Origin lassen sich auch Ressourcen ganz blockieren (verkürzte Ladezeiten!) und Elternelemente nach Eigenschaften ihrer Kinder blockieren.

```
!2018-05-02

!Einträge aus Hauptmenü entfernen
!zeit.de##.nav__ressorts-list > li:has(>a[href*="/spiele"])
!zeit.de##.nav__ressorts-list > li:has(>a[href*="/hamburg"])
!zeit.de##.nav__ressorts-list > li:has(>a[href*="/d17"])

!Soziale Netzwerke: Teilen, Folgen, Jobangebote
zeit.de##.sharing-menu,.follow-us,.jobbox-ticker

!Mehr Werbung blockieren
zeit.de##.cp-region:has(>[data-ct-context="parquet-verlagsangebot"])
||quiz.zeit.de/
||audev.zeit.de/
zeit.de##.cp-area--minor:has(>.frame>iframe[src*="quiz.zeit.de/"])
zeit.de##.x-spacing:has(>.zg-wiegehtesihnen)
zeit.de###main > .cp-region--solo:has(>div>#servicebox)
zeit.de##article[data-unique-id*="xml.zeit.de/vorabmeldungen/"]
zeit.de##form:has(>.newsletter-teaser-text)
zeit.de##.article-heading:style(padding:0 !important)
zeit.de##.article-heading__kicker:style(margin-bottom:0 !important)
||static.zeit.de/static/js/config_adreload.json
ze.tt##.ph-notification
```

### Anleitung

Den Textblock markieren & kopieren.  
Dann Dashboard öffnen (Schieberegler-Icon ganz rechts) --> Meine Filter --> Rechtsklick & Einfügen --> Änderungen anwenden


## Weitere Skripte

Für funktionelle Erweiterung per JavaScript (z.B. mit [Greasemonkey](https://www.greasespot.net/) / [Tampermonkey](https://tampermonkey.net/) oder ähnlichen Addons) stehen folgende praktische Skripte zur Verfügung:

- [Automatische Weiterleitung auf Komplettansicht bei mehrseitigen Artikeln](https://greasyfork.org/de/scripts/32064)
- [Filtern & Hervorheben von Schlagzeilen sowie auto-refresh](https://greasyfork.org/de/scripts/27523) (nur für den [Newsticker](https://www.zeit.de/news/index))


## Sonstiges

Getestet mit Firefox59 & Chrome65 auf dem Desktop. Ich bin dankbar für [Feedback](https://github.com/stonecrusher/UserCSS-zeit/issues).


## Changelog

- 2018-05-02: UserCSS-Version auf GitHub bereitgestellt; Fix für "Meistgelesene"-Sidebar; Fix für Artikel Headerbild; Namespace entfernt; Abstände Subheader auf Artikelseiten verkleinert.
- 2017-08-20: Added Userscript to description; New setting "minimal header"; Hide .ad-container.
- 2017-06-30: Changed default settings to my personal needs.
- 2017-05-15: Option to remove fullpage overlay asking to refresh the page for latest news.
- 2017-05-10: Option to remove invisible links (left and right sidebar) when viewing article with javascript disabled; Default: Do not remove (as most users have javascript enabled).
- 2017-04-13: Extended option to remove article top picture to also remove top videos.
- 2017-04-12: Option to remove ZeitPlus-articles; Edited option to remove most read, most commented, most shared; Minor fixes in footer.
- 2017-04-07: Condensed the Liveblog a little bit.
- 2017-04-06: Removed footer logo and footer margin.
- 2017-03-17: Updated "teaser-fullwidth" image position.
- 2017-01-26: Updated new main teaser "teaser-classic"; Removed ads from navigation; Added more options; Updated description.
- 2016-12-27: Added option to remove comment section.
