# GitHub Pages Deployment

## Einmalige Einrichtung

1. **GitHub Repo anlegen**  
   Neues öffentliches Repo erstellen, z.B. `inqa-handwerk`

2. **Diesen Ordner hochladen**  
   Den gesamten `landingpage/`-Ordner in das Repo pushen:
   ```
   cd landingpage/
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/DEIN-USERNAME/inqa-handwerk.git
   git push -u origin main
   ```

3. **GitHub Pages aktivieren**  
   Repo → Settings → Pages → Source: `main` / `/ (root)` → Save

4. **Subdomain einrichten (optional)**  
   Unter cognicore.de einen CNAME auf `DEIN-USERNAME.github.io` zeigen lassen  
   Dann im Repo eine Datei `CNAME` anlegen mit dem Inhalt:
   ```
   handwerk.cognicore.de
   ```

5. **Calendly-Link eintragen**  
   In `index.html` alle Vorkommen von `https://calendly.com/DEIN-LINK` ersetzen

## Ordnerstruktur
```
landingpage/
  index.html
  DEPLOY.md
  assets/
    carousel/
      handwerk_01.png
      handwerk_02.png
      handwerk_03.png
      handwerk_04.png
      handwerk_05.png
    logos/
      inqa-coaching-logo.png
      bmas-foerderlogo.png
```
