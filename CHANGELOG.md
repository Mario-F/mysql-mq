## [0.5.1](https://github.com/Mario-F/mysql_mq/compare/v0.5.0...v0.5.1) (2022-05-15)


### Bug Fixes

* updated package.json should also be commited ([879e222](https://github.com/Mario-F/mysql_mq/commit/879e22240443541b8a63400fd8f93d5643ba5988))

# [0.5.0](https://github.com/Mario-F/mysql_mq/compare/v0.4.2...v0.5.0) (2022-05-15)


### Bug Fixes

* go back to commonjs module till upgrade typescript ([67e6987](https://github.com/Mario-F/mysql_mq/commit/67e698718e70afddc18866a0b6c7e551e7b520d7))
* npm token must added to release jobs ([68cab73](https://github.com/Mario-F/mysql_mq/commit/68cab7329fb8a7f43130126a8504061ee43ac2ba))
* use mysql-5.7 for tests ([f7f2ccb](https://github.com/Mario-F/mysql_mq/commit/f7f2ccbf31c8c7526e7e9b5028d77d10b787fde8))


### Features

* add node 18 to tests ([1ee4120](https://github.com/Mario-F/mysql_mq/commit/1ee4120132c2c6b96398c8a70af13ae655984acb))
* added manual release job ([23b15fd](https://github.com/Mario-F/mysql_mq/commit/23b15fdfd490bc2716642fe12380d210db5e70b0))
* added npm step to release ([09c6e58](https://github.com/Mario-F/mysql_mq/commit/09c6e5810f8bd7111be408a66a149c014e3afc9c))
* added semantic-release ([b468101](https://github.com/Mario-F/mysql_mq/commit/b468101bcd3e9f0201fdca59bcc0202c99648d1c))
* added tests for many mysql/mariadb versions ([d7b5449](https://github.com/Mario-F/mysql_mq/commit/d7b5449fed97fb503100cb870c96d70949aeb23d))
* create github actions test workflow ([3b4af9e](https://github.com/Mario-F/mysql_mq/commit/3b4af9e3517256f6c35ff06206f2ad99a7800411))
* use es6 module ([f9eb0e9](https://github.com/Mario-F/mysql_mq/commit/f9eb0e9c005c87064d59d37e0eff7521e0778c8b))

## [0.4.2] - 2018-01-16
### Added
- Query queuing to automatically setup database without waiting for completion
- Changelog (/CHANGELOG.md)
- Docker environment for testing (See README.md)
- Use wtfnode in tests when DEBUG env is set
- Editorconfig and ES-Lint

### Changed
- Reworked query engine to be more robust
- Updated dependencies to latest version
- Updated test to latest versions

## [0.2.0] - 2017-02-02
### Added
- Additional support for promises

### Changed
- Switch to MySQL connections instead of pooling
- Updated dependencies to latest version
- Updated test to latest versions
