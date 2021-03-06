# JAD

JSON Api :heart: Doctrine ORM

[![Build Status](https://travis-ci.org/oligus/jad.svg?branch=master)](https://travis-ci.org/oligus/jad)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

JAD is a library created for rapid development of [JSON API](http://jsonapi.org) backend REST implementation. You can
run JAD as a standalone server with php -S (see [demo](demo/README.md)), or you can use it as a middleware in your framework.

It turns doctrine entities ([doctrine/doctrine2](https://github.com/doctrine/doctrine2)) to a JSON API resource, or 
collection of resources automagically.

## Requirements

You need to have Doctrine installed and preferably setup before you can use Jad.

## Install

`composer require oligus/jad`

## Quick start
```
$jad = new Jad(new Jad\Map\AnnotationMapper($em));
$jad->setPathPrefix('/api/v1/jad');
$jad->jsonApiResult();
```

## Contents

[Mapping your entities](docs/mapping.md)

[Fetching the resources](docs/fetch.md)

[Pagination](docs/pagination.md)

[Ordering](docs/ordering.md)

[Fetching resources with relationships](docs/relations.md)

[Creating a new resource](docs/create.md)

[Updating a resource](docs/update.md)

[Deleting resources / relationships](docs/delete.md)

## Contributing

When contributing to this repository, please first discuss the change you wish to make via issue before making a pull request.

## Authors

* **Oli Gustafsson** - *Initial work* - [oligus](https://github.com/oligus)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details
