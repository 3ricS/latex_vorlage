# Vorlage für LaTeX

## Systemvoraussetzungen
Python sowie das Paket `pygments` muss zur besseren Anzeige von Code installiert sein (Installation: siehe unten).

Falls eine minimalistische Version mit weniger Funktionen ausreicht, wird kein Python benötigt. Dazu muss mittels auf den Branch `minimal` gewechselt werden:
```
git checkout -b minimal
```

### Bibtex
Für das Literaturverzeichniss wird Bibtex in Verbindung mit biber genutzt.
In den Einstellungen vom Texstudio muss unter dem Menüpunkt **Erzeugung** das Standard Bibliografieprogramm auf biber umgestellt werden.

### minted
Für die deutlich bessere Einbindung und Syntaxhervorhebung von Quellcode wird das Paket [minted](https://github.com/gpoore/minted) verwendet.
Um das Paket verwenden zu können, wird Python 2.7.X und das Python-Paket pygments benötigt.

[Anleitung Stackoverflow](https://tex.stackexchange.com/questions/108661/how-to-use-minted-under-miktex-and-windows-7)

1. Python 2.7.X [herunterladen](https://www.python.org/downloads/) und installieren. Beim installieren ist darauf zu achten dass Python auch in den Umgebungsvariablen angepasst wird.
2. Pythons Paketverwaltung pip installieren
3. Das Paket pygments installieren
    * ```pip install pygments```
4. Den Zugriff auf externe Programme für den Compiler ````-shell-escape```` erlauben.
    * in Den Einstellungen von TexStudio unter dem Menüpunkt **Befehle** den Befehlt für PdfLaTeX mit ````-shell-escape```` ergänzen. Aus dem Standard Befehl ```pdflatex.exe -synctex=1 -interaction=nonstopmode %.tex``` wird dann ```pdflatex.exe -shell-escape -synctex=1 -interaction=nonstopmode %.tex```

# Programme zur Bearbeitung
Die Vorlage wurde mit [LaTeX](https://www.latex-project.org/) erstellt.
Als Editor kann [TeXstudio](https://www.texstudio.org/) genutzt werden. Hier müssen die Standarteinstellungen des Compilers
des Literaturverzeichnisses auf biber.exe umgestellt werden.

Zur grafischen Bearbeitung des Literturverzeichnisses kann [JabRef](https://www.jabref.org/) genutzt werden.
