<h1 align="center">Laravel Language Manager</h1>

<p align="center">
Langman is a GUI for managing JSON translations for Laravel 9.x. 

Originally fork of [themsaid/laravel-langman-gui](https://github.com/themsaid/laravel-langman-gui), but under active maintenance.
<br>
<br>
<img src="https://s14.postimg.org/j99tukfch/Screen_Shot_2017-05-02_at_9.56.49_AM.png" alt="Laravel Langman">
<br>
<a href="https://packagist.org/packages/efectn/laravel-langman-gui"><img src="https://poser.pugx.org/efectn/laravel-langman-gui/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/efectn/laravel-langman-gui"><img src="https://poser.pugx.org/efectn/laravel-langman-gui/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/efectn/laravel-langman-gui"><img src="https://poser.pugx.org/efectn/laravel-langman-gui/license.svg" alt="License"></a>
</p>

## Installation

Begin by installing the package through Composer. Run the following command in your terminal:

```
$ composer require efectn/laravel-langman-gui
```

Then publish the configuration file & assets:

```
php artisan vendor:publish --provider=Efectn\\LangmanGUI\\LangmanServiceProvider
```

## Usage

Once you have added the Service Provider point your browser to `http://project.dev/langman`, using this interface you'll be able to
browse translation keys in different languages, add/remove keys, scan your project files for missing translations, and finally save
your changes to the language JSON files.

## Backup

Langman stores a backup of your entire `resources/lang` directory into `storage/langmanGUI`, you can use restore the original files
using this backup in case anything went wrong.