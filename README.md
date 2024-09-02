# _la selector_

_la selector_ can help you select the most suitable language based on the IETF language tag.

## Installation

```
npm i laselector
```

## Usage
```
const { selectLanguage } = require('laselector')
// import { selectLanguage } from 'laselector'

// define `languages`
const languages = {
  default: 'it',
  supported: [
    'it',
    'fr',
    'nl',
    'da',
    'wal',
    'es-MX',
    'pt-PT',
    'ru-RU',
    'tr',
    'tr-CY'
  ]
}

for (const tag of [
  null,             // it
  'nob',            // da
  'wal',            // wal
  'pt',             // pt-PT
  'pt-PT',          // pt-PT
  'pt-BR',          // pt-PT
  'de',             // it
  'de-CH',          // fr
  'tr',             // tr
  'tur-CY',         // tr-CY
  'ro',             // it
  'ro-MD',          // ru-RU
  'ru',             // ru-RU
  'rus',            // ru-RU
  'cu-RU',          // ru-RU
  'uk',             // ru-RU
  'kk-KZ',          // ru-RU
  'fr',             // fr
  'ar',             // it
  'ar-EG',          // it
  'ar-MA',          // fr
  'af-ZA',          // nl
  'ca',             // es-MX
  'ca-ES-VALENCIA'  // es-MX
]) console.log(`${tag} => ${selectLanguage(tag, languages)}`)
```

## Contributing
Contributions are only allowed in TON:
```
UQCYqT9-ycmXE3o57Cac1sM5ntIKdjqIwP3kzWmiZik0VU_b
```
