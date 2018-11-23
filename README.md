# carbon-colombia

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]


Se agregan los festivos de Colombia, con el fin de poder agregar dias hábiles.

## Install

Via Composer

``` bash
$ composer require torreswil/carbon-colombia
```

## Usage

``` php
$fecha = CarbonColombia::create(2019,04,16);
$fecha->addBussinessDays(5);
echo $fecha->toDateString();
//imprime 2019-04-25

$fecha = CarbonColombia::create(2019,04,16);
$fecha2 = CarbonColombia::create(2019,04,25);
echo $fecha->diffInBussinessDays($fecha2);
//imprime 5
```

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Testing

``` bash
$ composer test
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) for details.

## Security

If you discover any security related issues, please email wtorresariza@gmail.com instead of using the issue tracker.

## Credits

- [Wilfredo Torres][link-author]
- Inspirado en: [luisplata/DiasFestivosColombia][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/torreswil/carbon-colombia.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/torreswil/carbon-colombia/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/torreswil/carbon-colombia.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/torreswil/carbon-colombia.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/torreswil/carbon-colombia.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/torreswil/carbon-colombia
[link-travis]: https://travis-ci.org/torreswil/carbon-colombia
[link-scrutinizer]: https://scrutinizer-ci.com/g/torreswil/carbon-colombia/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/torreswil/carbon-colombia
[link-downloads]: https://packagist.org/packages/torreswil/carbon-colombia
[link-author]: https://github.com/:author_username
[link-contributors]: https://github.com/luisplata/DiasFestivosColombia
