# patch-composer

This project is an example on how to patch a composer library

## Installation
use `composer install` to download all libraries

## Example

Start by copying the original file to a root directory using `cp vendor\symfony\var-dumper\Dumper\HtmlDumper.php patches\`

<strong>The files must have same names and all commands are based on unix</strong> 

Create a patch file using `diff -u vendor\symfony\var-dumper\Dumper\HtmlDumper.php patches\HtmlDumper.php > var_dumper.patch`

## Running
Use `php -S localhost:8000 -t ./` to start project on port 8000.
