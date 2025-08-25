<div style="background-color: #262335; padding: 20px; border-radius: 10px;">

# HTML-skjema guide

Her får du en enkel guide for å lage skjemaer i HTML.

## Steg 1: Start med `<form>`

Alle skjemaer starter med `<form>`-taggen, og denne må ligge inne i `<body>`-elementet.

```html
<body>
    <form>
        <fieldset>
            <!-- Skjema-innhold her -->
        </fieldset>
    </form>
</body>
```

Taggen `<fieldset>` brukes for å gruppere relaterte felter sammen. Dette gir bedre struktur og gjør skjemaet mer oversiktlig, både visuelt og for hjelpemidler som skjermlesere.

## Eksempel på et enkelt skjema

![](Login.png)

### Kodeeksempel

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Skjema</title>
        <link rel="stylesheet" href="Style.css">
    </head>
    <body>
        <form id="container">
            <fieldset>
                <legend>Login</legend>
                <label for="Username">Username:</label>
                <input type="text" name="Username" id="Username" required>
                <br><br>
                <label for="Password">Password:</label>
                <input type="password" name="Password" id="Password" required>
                <input type="submit" name="submit" id="submit" value="Login">
            </fieldset>
        </form>
    </body>
</html>
```

**Tips:**  
- Bruk `<legend>` for å gi en overskrift til gruppen med felter.
- `required` gjør feltet obligatorisk.
- Gruppér relaterte felter med `<fieldset>` for bedre struktur og tilgjengelighet.

Nå har du et oversiktlig og brukervennlig HTML-skjema!