# OpenCart Testing Suite

## Usage

### Wait just a second!
This project is included in Forever Store via a composer link.  You
don't need to check this out in addition to the Forever Store!  In the
event you want to set it up in a new instance of a store, look below.

### Prerequisits
* Forever Store running on your development environment

### Steps to use
* make a tests directory off of the root of the repo
* add a composer.json file wihtin the folder, and add the following:

```javascript
{
	"require": {
		"beyondit/opencart-test-suite": "0.2.1"
	}
}
```
* run `composer update` to download the necessary project dependencies
* create a UnitTest and extend it from OpenCartTest class, e.g.:

```php
class MyTest extends OpenCartTest {	
    public function testSomething() {			
    }	
}
```
* run `vendor/bin/phpunit MyTest` inside your test folder
