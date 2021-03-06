---
theme: datev-scc
lineNumbers: false
info: |
  ## Slidev
  Das Powerpoint für Entwickler
drawings:
  persist: false
download: true
title: Intro to Slidev
layout: intro
---

# Intro to Slidev

Das Powerpoint für Entwickler

<carbon-link /> [enolive.github.io/intro-to-slidev](https://enolive.github.io/intro-to-slidev)

<MyVCard />

---
layout: cover
class: text-3xl
---

# Warum?

<carbon-arrow-right /> Powerpoint & Co sind nicht für Entwickler gemacht!

<style>
  h1 {
    @apply !text-2xl;
  }
</style>

---
layout: quote
author: "Kamelopedia: Porno-Point-Präsentation"
link: http://kamelopedia.net/wiki/Porno-Point-Pr%C3%A4sentation
---

Die Porno-Point-Präsentation ist ein **modernes Folterinstrument** auf Basis des **allseits verhassten Diaabendes** bei Freunden und den Schwiegereltern

<style>
p {
  @apply font-light;
}
</style>

---

# PowerPoint nicht automatisch schlecht!

<Youtube id="Iwpi1Lm6dFo" width="600" height="400" />

---
class: text-3xl
---

# Inhalt vor Layout!

|                                             |                 |                  |
|---------------------------------------------|-----------------|------------------|
| [Patat](https://github.com/jaspervdj/patat) | Terminal        | Markdown         |
| [Reveal JS](https://revealjs.com/)          | Browser         | HTML + Markdown  |
| [Slidev](https://sli.dev)                   | Browser         | Markdown + VueJS |

---

# Syntax Highlighting

<div v-click-hide>

Code wird automatisch hervorgehoben!

```java
class App {
  public static void main(String[] args) {
    System.out.println("Hello, World!");
  }
}
```

</div>

<div v-after>
  
... Auch für exotischere Sprachen 😉.
  

```haskell
fizzBuzz :: Int -> [String]
fizzBuzz n = take n $ zipWith max fizzBuzzes numbers
  where
    fizzBuzzes = zipWith (++) fizzes buzzes
    fizzes = cycle ["", "", "Fizz"]
    buzzes = cycle ["", "", "", "", "Buzz"]
    numbers = show <$> [1..]
```

</div>


---

## Diagramme

<div grid="~ cols-2 gap-4">

<div v-click-hide>
  
Diagramme mit [Mermaid](https://mermaid-js.github.io) direkt einbetten!

```mermaid {scale: 0.5}
classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```

</div>

<div v-after>
  
...auch ausgefallenere Dinge als UML 😉.

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

</div>

</div>


---
layout: cover
class: text-3xl
---

# Versionierung

<carbon-arrow-right /> Plain-text einfacher als Binary Files!

<style>
  h1 {
    @apply !text-2xl;
  }
</style>

---
class: fade
---

# Slidev Quick Facts

<v-clicks>

- [sli.dev](https://sli.dev)
- Basiert auf Vue.JS 3.x
- Responsive
- Markdown Syntax
- CSS Customizing möglich inkl. [Windi CSS](https://windicss.org/)

</v-clicks>

---

# Wie fange ich an?

<div class="fade">

<v-clicks>

1. Installation mit `npm init slidev`
2. Inhalt in `slides.md` schreiben!
3. Theme anpassen

</v-clicks>

</div>

<v-click>

```yaml
theme: datev-scc
```

</v-click>

---
layout: image
image: https://source.unsplash.com/random?coding
---

# Demo 👩‍💻

<style>
  h1 {
    @apply text-shadow-xl;
  }
</style>

---

# Editor

[VS Code](https://code.visualstudio.com/) mit Extensions für [Windi CSS](https://marketplace.visualstudio.com/items?itemName=voorjaar.windicss-intellisense) und [Slidev](https://marketplace.visualstudio.com/items?itemName=antfu.slidev)

<div v-click>

Meine `settings.json`

```json
{
  "css.validate": false,
  "editor.quickSuggestions": {
    "strings": true
  },
  "windicss.includeLanguages": {
    "markdown": "html",
    "md": "html"
  }
}
```

</div>

<!--
Zur Not geht aber auch der Web Browser!
-->

---
layout: cover
---

# 🙇 Danke! 🙇

- <carbon-link /> [sli.dev](https://sli.dev)
- <carbon-logo-github /> [github.com/enolive/intro-to-slidev](https://github.com/enolive/intro-to-slidev)
- <mdi-npm /> [npmjs.com/package/slidev-theme-datev-scc](https://www.npmjs.com/package/slidev-theme-datev-scc)
- <fa-youtube/> [How to avoid death by PowerPoint](https://www.youtube.com/watch?v=Iwpi1Lm6dFo)

<MyVCard />
