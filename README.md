# Übung: MailButton Component

## Aufgabe
Erstelle eine Komponente "MailButton" die einen E-Mail-Link als Button darstellt.

## Anforderungen

### 1. Template
In der Komponente soll ein Link verwendet werden:
```html
<a href="mailto:adresse">adresse</a>
```

### 2. Props
- `mail`: string (Pflichtfeld mit E-Mail-Validierung)

### 3. Design
Der Link soll aussehen wie ein Button mit modernem Design.

## Starter Code

```vue
<template>
  <!-- TODO: E-Mail Link als Button -->
</template>

<script setup lang="ts">
// TODO: Props mit E-Mail Validierung definieren

</script>

<style scoped>
/* TODO: Button-Styling für den Link */

</style>
```

## Anforderungen im Detail

### Props Validierung
- E-Mail muss @ enthalten
- E-Mail muss gültiges Format haben
- Console-Warnung bei ungültiger E-Mail

### Button-Design
- Padding: 0.5rem 1rem
- Background: #3b82f6 (blau)
- Text: weiß
- Border-radius: 4px
- Hover-Effekt: dunkleres blau (#2563eb)
- Keine Unterstreichung
- Cursor: pointer

## Erwartete Verwendung

```vue
<template>
  <div>
    <MailButton mail="kontakt@firma.de" />
    <MailButton mail="support@example.com" />
    
    <!-- Sollte Warnung in Console zeigen -->
    <MailButton mail="ungueltige-email" />
  </div>
</template>
```

## Erwartetes Ergebnis
- Klickbarer Button der E-Mail-Programm öffnet
- Button-Design statt Standard-Link-Aussehen
- Validierung warnt bei ungültigen E-Mails
- E-Mail-Adresse wird als Button-Text angezeigt
