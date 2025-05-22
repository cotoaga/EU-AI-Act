# EU AI Act Überlebens-Entscheidungsbaum 🤖

> *Oder: Wie du durch die Galaxie der Bürokratie navigierst ohne deinen Verstand zu verlieren*

## Was ist das hier?

Ein **satirischer, interaktiver Entscheidungsbaum**, der die Komplexität des EU AI Acts auf humorvolle Weise aufgreift. Spoiler Alert: Egal welche Antworten du wählst, du brauchst am Ende den KHAOS EU AI Act Kurs! 😉

**WICHTIG:** Dies ist ein **GAG** und **Proof of Concept** – keine echte Rechtsberatung! Für ernsthafte EU AI Act Compliance bitte echte Experten konsultieren.

## Live Demo

🔗 **[Hier ausprobieren!](https://deine-vercel-url-hier.vercel.app)**

## Features

- 🎭 **Humorvolle Interpretation** des EU AI Acts mit Douglas Adams'schen Anklängen
- 🌳 **Interaktiver Entscheidungsbaum** mit Echtzeit-Visualisierung
- 📱 **Mobile-optimiert** mit großen, lesbaren Texten
- 🎯 **Klickbare Knoten** mit Detail-Popups
- 🎨 **Responsive Design** für Desktop und Mobile
- ⚡ **Vanilla JavaScript** – keine Frameworks, läuft überall

## Die kosmische Geschichte

1. Das Universum wurde erschaffen, was viele Leute sehr ärgerlich machte und im Allgemeinen für keine gute Idee befunden wurde.
2. Unsere Vorfahren stiegen von den Bäumen, erschufen kurz danach Feuer, Rad und den Eingangsstempel der Behörden.
3. Dies besorgte mächtige Bürger so sehr, dass sie im Jahr 2024 den EU AI Act erschufen.

## Technische Details

### Aufbau
- **Eine einzige HTML-Datei** (`index.html`) mit eingebettetem CSS und JavaScript
- **SVG-basierte Visualisierung** des Entscheidungsbaums
- **Dynamische Knoten-Generierung** basierend auf Benutzerentscheidungen
- **Responsive Layout** mit flexiblen Container-Strukturen

### Browser-Kompatibilität
- ✅ Chrome/Edge (moderne Versionen)
- ✅ Firefox (moderne Versionen)
- ✅ Safari (moderne Versionen)
- ✅ Mobile Browser (iOS Safari, Chrome Mobile)

### Performance
- 📦 **Keine externen Abhängigkeiten** außer D3.js für SVG-Manipulation
- ⚡ **Schnelle Ladezeiten** durch minimalen Overhead
- 🔧 **Automatische iframe-Größenanpassung** für nahtlose Einbettung

## Installation & Deployment

### Lokale Entwicklung
```bash
# Repository klonen
git clone [dein-repo-url]
cd eu-ai-act-decision-tree

# Einfach die index.html in einem Browser öffnen
open index.html
# oder einen lokalen Server starten
python -m http.server 8000
```

### Vercel Deployment
```bash
# Vercel CLI installieren (falls nicht vorhanden)
npm i -g vercel

# In das Projektverzeichnis wechseln
cd eu-ai-act-decision-tree

# Deploy
vercel

# Produktions-Deploy
vercel --prod
```

### Einbettung in andere Websites
```html
<iframe 
  id="eu-ai-tree" 
  src="https://deine-vercel-url.vercel.app" 
  style="width: 100%; border: none; height: 800px;" 
  scrolling="no">
</iframe>

<script>
  // Automatische Höhenanpassung
  window.addEventListener('message', function(event) {
    if (event.data && event.data.type === 'resize') {
      document.getElementById('eu-ai-tree').style.height = event.data.height + 'px';
    }
  });
</script>
```

## Architektur

### Spielzustände
```javascript
const gameStates = {
  q1: { type: 'question', content: '...', displayName: '...', options: [...] },
  e1: { type: 'endpoint', content: '...', displayName: '...', options: [...] },
  // ... weitere Zustände
}
```

### Visualisierung
- **SVG-Knoten** mit dynamischer Positionierung
- **Kurvenverbindungen** zwischen den Zuständen
- **Klickbare Popups** mit Detailinformationen
- **Farbkodierung** für besuchte/aktuelle/zukünftige Zustände

### Responsive Breakpoints
- **Mobile**: < 768px (vertikales Layout)
- **Desktop**: ≥ 768px (horizontales Layout mit Seitenansicht)

## Anpassungen & Erweiterungen

### Neue Fragen hinzufügen
1. Neuen Zustand in `gameStates` definieren
2. Koordinaten in `calculateNodePosition()` hinzufügen
3. Verbindungen in bestehenden Zuständen ergänzen

### Styling anpassen
Alle Styles sind im `<style>`-Block definiert und können einfach modifiziert werden:
- `.node-text` für Knoten-Beschriftungen
- `.popup-info` für Detail-Popups
- `.option` für Antwort-Buttons

### Inhalte übersetzen
Alle Texte sind in den `gameStates` zentralisiert und können einfach übersetzt werden.

## Bekannte "Features" 😄

- **Deterministische Ausgabe**: Alle Wege führen zum KHAOS-Kurs (by design!)
- **Bürokratie-Simulation**: Absichtlich verschachtelte Entscheidungslogik
- **Douglas Adams Tribut**: Kosmische Einleitung und surrealer Humor
- **Realitäts-Check**: Wiederkehrende Erinnerung daran, dass niemand die EU-Verordnung wirklich versteht

## Disclaimer

⚠️ **Dieser Entscheidungsbaum ist SATIRISCH gemeint!**

- **Keine Rechtsberatung**: Für echte EU AI Act Compliance konsultiere bitte qualifizierte Juristen
- **Proof of Concept**: Demonstriert, wie KI bei der Entwicklung interaktiver Inhalte helfen kann
- **Educational Purpose**: Zeigt kreative Ansätze für komplexe Themen auf

## Credits & Inspiration

- 🚀 **Douglas Adams** für den Humor und die kosmische Perspektive
- 🤖 **EU AI Act** für die unerschöpfliche Quelle bürokratischer Komplexität
- 🎨 **D3.js** für die SVG-Visualisierung
- 🧠 **KI-gestützte Entwicklung** als Demonstration moderner Entwicklungsansätze

## Beitragen

Du hast Ideen für weitere humorvolle Entscheidungspfade oder technische Verbesserungen?

1. Fork das Repository
2. Erstelle einen Feature-Branch (`git checkout -b feature/mehr-sarkasmus`)
3. Committe deine Änderungen (`git commit -m 'Füge galaktischen Humor hinzu'`)
4. Push zum Branch (`git push origin feature/mehr-sarkasmus`)
5. Erstelle einen Pull Request

## Support & Kontakt

Fragen, Anregungen oder willst du lernen, wie man mit KI solche Projekte entwickelt?

- 📧 **Email**: kurt@cotoaga.net
- 🌐 **Website**: [cotoaga.net](https://cotoaga.net)
- 🎓 **Workshops**: Erfahre in unseren EU AI Act Workshops, wie du KI verantwortungsvoll und effektiv einsetzt

---

*Gebaut mit ❤️, viel ☕ und einer gesunden Portion 😂 über die wunderschöne Welt der EU-Bürokratie.*