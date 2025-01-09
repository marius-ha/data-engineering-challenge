# Data Engineering Challenge 🚀 
[Switch to the English README](https://github.com/marius-ha/data-engineering-challenge/blob/main/README-EN.md)



Tach auch! Willkommen beim Data Engineering Projekt – hier jibbet wat mit Docker, Python, der Open-Meteo API und 'ner Ladung Daten! Guck dir die Anleitung ma in Ruhe an und leg direkt los mit'm Projekt.

## Wat du brauchst

### Git

Noch kein Git am Start? Kein Ding! Hol’ et dir hier: [Git Downloads](https://git-scm.com/downloads)

### Docker Desktop

Für die Challenge brauchst’e Docker Desktop: [Docker Desktop](https://www.docker.com/products/docker-desktop)

#### Für Windows-Leute: WSL2 is Pflicht

Wenn du Windows nutzt, check ma, ob WSL2 installiert is. Hier findste 'ne Anleitung: [WSL2 Installation Guide](https://docs.docker.com/desktop/wsl/)

### VSCode

Als Entwicklungsumgebung nutzen wir 'nen vordefinierten Docker-Container. Da sind schon 'n paar nützliche Pakete vorinstalliert. Damit dat funzt, brauchste VSCode. Wenn du schon 'ne andere IDE hast, die mit nem Docker-Container klarkommt, auch gut!

## Projekt-Setup

1. Hol dir das Repo:

    ```bash
    git clone https://github.com/marius-ha/data-engineering-challenge.git
    cd data-engineering-challenge
    ```

2. Mach das Projekt in Visual Studio Code auf – der Devcontainer regelt dat schon!

3. Wenn wat fehlt, installier’ dat einfach mit `pip`.

## Wat wir machen

Unser Test-Projekt hat 'ne paar Aufgaben für dich:

1. **Mit der Open-Meteo API das Wetter checken:**
    - Hol dir die [Wetterdaten](https://open-meteo.com/) über die Open-Meteo API.
    - Nutz die `request` Library von Python.
    - Guck dir historische Wetterdaten (stundenweise) für **Essen** an. Uns interessieren vor allem:
        - Temperatur
        - Luftfeuchtigkeit
        - Regen
        - Wettercode
        - Windgeschwindigkeit
        - Oberflächendruck
    - Denk dir ‘n cooles Logging aus – bei Fehlern oder wenn alles klappt. Dat hilft beim Debuggen und macht Eindruck. 👍
    - Zeig, watte drauf hast, wenn’s um APIs und Datenextraktion geht.

2. **Daten in DuckDB pumpen:**
    - Schieb die Daten in 'ne lokale [DuckDB](https://duckdb.org/).
    - Damit’s nich langweilig wird: Entscheide beim Start, welche Lade-Strategie genutzt wird:
        - **Full-Refresh:** Alles im Data Warehouse wird überschrieben und neu eingefügt.
        - **Incremental:** Nur neue Daten werden ins Data Warehouse geladen.
    - Guck dir den Response an und überleg, wie die Daten ordentlich in DuckDB geschrieben werden müssen.

3. **Steuerung vom Python-Skript:**
    - Folgende API-Parameter sollste über die Kommandozeile anpassen können:
        - Latitude
        - Longitude
        - Startdatum
        - Enddatum
        - Zeitzone

4. **Docker-Container:**
    - Pack deine Python-Anwendung in 'nen Docker-Container.
    - Am Ende soll der Container laufen und die Parameter für den API-Aufruf übergeben können. Das Logging soll dann in der Konsole erscheinen.

5. **...and beyond:**
    - Halt den Code sauber und kommentier schlau.
    - Definier Funktionen und Klassen, wo dat Sinn macht.
    - Nutz `git`, um dein Projekt zu versionieren und push am Ende alles ins Repository, damit wir uns dein Ergebnis angucken können.

## Let’s Code und Glück Auf ⚒️!

Viel Erfolg und vor allem viel Spaß beim Coden! Wenn’s Fragen gibt, meld dich. Happy coding! 🚀✨

## Anhang

### Nützliche Links

- [Open-Meteo Dokumentation](https://open-meteo.com/en/docs)
- [DuckDB Dokumentation](https://duckdb.org/docs/sql/introduction)