# Osan 0 palautukset

## 0.4

```
selain->palvelin: HTTP POST https://fullstack-exampleapp.herokuapp.com/new_note
palvelin-->selain: HTML-koodi ja uudelleenohjauspyyntö

note over selain:
selain saa vastauksena osoitteen
minne se uudelleenohjaa automaattisesti
end note

selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/notes
palvelin-->selain: HTML-koodi
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/main.css
palvelin-->selain: main.css
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/main.js
palvelin-->selain: main.js

note over selain:
selain alkaa suorittaa js-koodia
joka pyytää JSON-datan palvelimelta
end note

selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/data.json
palvelin-->selain: [{ content: "HTML on helppoa", date: "2019-01-01" }, ...]

note over selain:
selain suorittaa tapahtumankäsittelijän
joka renderöi muistiinpanot näytölle
end note
```

## 0.5

```
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/spa
palvelin-->selain: HTML-koodi
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/main.css
palvelin-->selain: main.css
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/spa.js
palvelin-->selain: spa.js

note over selain:
selain alkaa suorittaa js-koodia
joka pyytää JSON-datan palvelimelta
end note

selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/data.json
palvelin-->selain: [{ content: "HTML on helppoa", date: "2019-01-01" }, ...]

note over selain:
selain suorittaa tapahtumankäsittelijän
joka renderöi muistiinpanot näytölle
end note
```

## 0.6

```
selain->palvelin: HTTP POST https://fullstack-exampleapp.herokuapp.com/new_note_spa {content: spa, date: 2019-01-17T07:38:22.536Z}
palvelin-->selain: [{message: note created}]
```

