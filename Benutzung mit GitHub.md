# Benutzung mit GitHub

Folgende Schritte habe durchgeführt, siehe Repository [mdwiki](https://github.com/dgloger/mdwiki).

1. [Vorlage für MDwiki](https://dynalon.github.io/mdwiki/#!tutorials/github.md) [forken](https://help.github.com/articles/fork-a-repo) und unter _Settings_ einen sinnvollen Namen wählen, z. B. „mdwiki“

2. [SSH-Schlüssel auf GitHub übertragen](https://help.github.com/articles/generating-ssh-keys#step-3-add-your-ssh-key-to-github)

3. Lokale Kopie in _Programme/Projekte/github_ erstellen
   
        git clone git@github.com:dgloger/mdwiki-seed.git
   
4. Startseite umbenennen

        git mv mdwiki.html index.html
   und Dateien ändern, z. B. in _navigation.md_ das Gimmik „Fork me on GitHub“ deaktivieren. [Startseite](index.html) in Browser laden.

5. Dateien hinzufügen

        git add 'Benutzung mit GitHub.md'

6. Commit für lokale Änderungen erstellen und auf GitHub übertragen

        git commit -am "Rename startpage to index.html, switch of 'Fork me on GitHub' in navigation.md and add 'Benutzung mit GitHub.md'"
        git push

## Änderungen an mdwiki.html

Urheberhinweis hellgrau darstellen:
```css
    #md-all .md-copyright-footer {
        font-size: smaller;
        padding: 1em;
        color: #aaa;
    }
    #md-all .md-copyright-footer a { color: #aad; }
```

Urheberhinweis verkürzt:

```javascript
b+='Website generated with <a href="http://www.mdwiki.info">MDwiki</a> ',b+="&copy; Timo D&ouml;rr and contributors. "
```

```javascript
b+='generiert mit <a href="http://www.mdwiki.info">MDwiki</a> '
```