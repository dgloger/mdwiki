# Benutzung mit GitHub

Folgende Schritte habe durchgeführt, siehe [MDwiki-Repository](https://github.com/dgloger/mdwiki)  auf GitHub.

1. [Vorlage für MDwiki](https://dynalon.github.io/mdwiki/#!tutorials/github.md) [forken](https://help.github.com/articles/fork-a-repo) und unter _Settings_ einen sinnvollen Namen wählen, z. B. „mdwiki“

2. [SSH-Schlüssel auf GitHub übertragen](https://help.github.com/articles/generating-ssh-keys#step-3-add-your-ssh-key-to-github)

3. Lokale Kopie erstellen
   
        cd Programme/Projekte/github/mdwiki
        git clone git@github.com:dgloger/mdwiki-seed.git
   
4. Startseite umbenennen

        git mv mdwiki.html index.html
   und Dateien ändern, z. B. in _navigation.md_ das Gimmik „Fork me on GitHub“ deaktivieren. [Startseite](index.html) in Browser laden.

5. Dateien hinzufügen

        git add 'Benutzung mit GitHub.md'

6. Commit für lokale Änderungen erstellen und auf GitHub übertragen

        git commit -a -m "Rename startpage to index.html, switch of 'Fork me on GitHub' in navigation.md and add 'Benutzung mit GitHub.md'"
        git push