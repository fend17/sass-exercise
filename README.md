# SASS

## Installation

Lättast är att använda [Scout App](http://scout-app.io/) som är ett grafiskt gränssnitt för sass. Du kan också köra sass via terminalen och det finns installationsinstruktioner här: [Install SASS](http://sass-lang.com/install).

## Övningar

### Övning 1

Filen `_variables.scss` är tom. I den ska alla variabler för sassen ligga. Man gör ett värde till en variabel om den är återkommande, om man använder värdet på flera ställen. Ett vanligt användningsområde är att lägga alla färger i variabler. Filer med understreck kallas för `partials` och kommer inte att skapa nya css-filer. De kan enbart importeras.

```scss
$primary: #456;
$secondary: #789;
```

### Övning 2

Koden i `_button.scss` är vanlig CSS. Din uppgift är att konvertera den så att den använder sig av **nesting**, `@extend` eller `&` (parent). Den går att lösa på flera sätt. I mitt lösningsförslag så är en lösning med `@extend` och en annan med nesting och `&`. Övningen är för att öva på funktionerna i sass och är inte nödvändigtvis den mest optimerade koden.

_nesting_
```scss
/* Becomes: .header h1 {} */
.header {
  img {
    min-height: 20rem;
  }
}
```
_parent_
```scss
/* Becomes .header-image */
.header {
  &-image {
    min-height: 20rem;
  }
}

```

## Övning 3

CSSen för navigationen ligger i `_navbar`. Optimera koden med sass genom att använda nesting, `&` samt variabler.

## Övning 4

Fortsätt att skapa resten av layouten med hjälp av sass. Det saknas en __sidebar_, en __main_ och en __footer_. Fortsätt att skapa layouten med hjälp av `partials`, `nesting`, `&` samt variabler.

## Övning 5

Lägg till sass på ett eget projekt och optimera koden. Gör om delar av din kod från Arboreal-projektet till sass. **Gör det på en kopia av koden. När du använder sass så skriver du över din egen css. Så var försiktig så att du alltid har en backup på koden**.