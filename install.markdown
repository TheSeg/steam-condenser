---
layout:       default
title:        Installation
---

The latest stable releases of Steam Condenser are listed below:

 * **Ruby**: {{site.scVersions.ruby}}
 * **Java**: {{site.scVersions.java}}
 * **PHP**:  {{site.scVersions.php}}

## Packages

### Ruby

The preferred way to integrate the Steam Condenser gem into your project is
using [Bundler](http://gembundler.com). Just specify a dependency in your
`Gemfile`:

```ruby
gem 'steam-condenser', '~> {{site.scVersions.ruby}}'
```

If you don't use Bundler, you can of course install the gem directly via
[RubyGems](https://rubygems.org):

```sh
$ gem install steam-condenser
```

### Java

The JAR archives for the library itself, the documentation and the source code
are available from [Maven Central](https://search.maven.org).

If you're using Maven you have to define Steam Condenser as a dependency in
your POM file:

```xml
<dependency>
    <groupId>com.github.koraktor</groupId>
    <artifactId>steam-condenser</artifactId>
    <version>{{site.scVersions.java}}</version>
</dependency>
```

If you're using another build tool, please use the appropriate syntax to use
Maven artifacts as a dependency.

The plain JARs can be downloaded [directly from Maven Central](https://search.maven.org/#artifactdetails%7Ccom.github.koraktor%7Csteam-condenser%7C{{site.scVersions.java}}%7Cjar), too.

### PHP

The recommended way to use Steam Condenser is to define a dependency using
[Composer](https://getcomposer.org):

```json
{
    "require": {
        "koraktor/steam-condenser": "{{site.scVersions.php}}"
    }
}
```

If you're not using Composer you can also get a plain source archive:

<div class="download">
  <a href="https://github.com/koraktor/steam-condenser-php/archive/{{site.scVersions.php}}.tar.gz">steam-condenser-php-{{site.scVersions.php}}.tar.gz</a>
  <br>
  <pre>
  SHA1: c92ef25cab70c20820d210e8ce29a0c7d024201e
  MD5:  7f0f5fbe9efaaf0a282a91af90fa76bc</pre>
</div>

## Git repositories

If you want to use the development code or – even better – contribute, cloning
the Git repository of a language specific implementation is the best way to get
started:

### Java repository

```sh
$ git clone git://github.com/koraktor/steam-condenser-java.git
```

### PHP repository

```sh
$ git clone git://github.com/koraktor/steam-condenser-php.git
```

### Ruby repository

```sh
$ git clone git://github.com/koraktor/steam-condenser-ruby.git
```

If you want some of the main files, like the `README`, or this website you
should clone the main repository.

### Main repository

```sh
$ git clone git://github.com/koraktor/steam-condenser.git
```

<br><br>

{% include google_adsense %}
