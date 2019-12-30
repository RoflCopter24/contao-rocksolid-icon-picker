# RockSolid Icon Picker Contao Extension

Fork for usage with the Contao asset system or webpack assets with manifest.json
( for example when using https://github.com/terminal42/contao-standard )

## Installation

```sh
$ composer require roflcopter24/contao-rocksolid-icon-picker
```

## Usage

```php
$GLOBALS['TL_DCA']['tl_content']['fields']['icon'] = [
    'inputType' => 'rocksolid_icon_picker',
    'eval' => array(
        'iconFont' => 'images/fa-solid-900.svg', # <-Internal/'virtual' asset path in manifest.json
        'iconFontPathPrefixSvg' => 'images', # <- Webpack sorts svg files in the 'images' directory
        'iconFontPathPrefixFont' => 'fonts' # <- Actual fonts for clients are in this folder
    ),
];
```

## Documentation:

-   English: https://rocksolidthemes.com/en/contao/plugins/custom-content-elements
-   German: https://rocksolidthemes.com/de/contao/plugins/custom-content-elements
