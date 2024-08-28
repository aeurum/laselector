# _la selector_

_la selector_ can help you select the most suitable language based on the IETF language tag.

## Installation

```
npm i laselector
```

## Usage
```
const { selectLanguage } = require('laselector');
// import { selectLanguage } from 'laselector'

// define `languages`
const languages = {
  default: 'ja',
  supported: [
    'ja',
    'fr',
    'da',
    'wal',
    'tr',
    'tr-CY',
    'en-GB',
    'ru-RU',
    'es-MX',
    'pt-PT'
  ]
}

for (const tag of [
  null,             // ja
  'nob',            // da
  'wal',            // wal
  'pt',             // pt-PT
  'pt-PT',          // pt-PT
  'pt-BR',          // pt-PT
  'it',             // ja
  'it-CH',          // fr
  'tr',             // tr
  'tur-CY',         // tr-CY
  'ro',             // ja
  'ro-MD',          // ru-RU
  'ru',             // ru-RU
  'rus',            // ru-RU
  'cu-RU',          // ru-RU
  'uk',             // ru-RU
  'kk-KZ',          // ru-RU
  'fr',             // fr
  'ar',             // ja
  'ar-EG',          // ja
  'ar-MA',          // fr
  'en',             // en-GB
  'af-ZA',          // en-GB
  'ca',             // es-MX
  'ca-ES-VALENCIA'  // es-MX
]) console.log(`${tag} => ${selectLanguage(tag, languages)}`)
```

## Contributing
Contributions are only allowed in TON:
```
UQCYqT9-ycmXE3o57Cac1sM5ntIKdjqIwP3kzWmiZik0VU_b
```