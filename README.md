# menu-breaker.js

JavaScript & jQuery plugin to switch between mobile and desktop menu and change submenus side on browser window resize

## Demo
**[See plugin in action](https://jb1905.github.io/menu-breaker.js/)**

## Usage
At the beginning connect the library with Your project:

**&bull; using script tag in HTML:**
```
<script src="/directory/to/library/folder/menu-breaker.js"></script>
```

**&bull; or via command line and CommonJS/ES6 import:**
```
npm install menu-breaker // npm
yarn add menu-breaker // yarn
```

```
const MenuBreaker = require('menu-breaker'); // CommonJS
import MenuBreaker from 'menu-breaker'; // ES6
```

<br>
Next use library with:

**&bull; Vanilla JavaScript e.g:**
```
const elem = document.querySelector('.desktop');
const menuBreaker = new MenuBreaker(elem, {
  // options...
});
```

**&bull; or jQuery e.g:**

*Connect jQuery in HTML*
```
<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
```

*or include via command line and CommonJS*
```
npm install jquery // npm
yarn add jquery // yarn
bower install jquery // bower
```

```
const jQuery = require('jquery');
```

*and call plugin on element*
```
$('.desktop').menuBreaker({
  // options...
});
```

## Options
Name | Type | Default | Description | Available options
-|-|-|-|-
**navbar-height** | number | `70` | Desktop menu height | e.g: `50`, `86`, etc.
**open-class** | string | `open` | Name of class added to mobile menu, after click `data-open` or `data-open-close` element | name of class
**onMenuOpen** | function | `null` | call function on mobile menu open | `() => { // code }`
**onMenuClose** | function | `null` | call function on mobile menu close | `() => { // code }`
**isMobile** | function | `null` | call function when is mobile menu | `() => { // code }`
**isDesktop** | function | `null` | call function when is desktop menu | `() => { // code }`

## License
This project is licensed under the MIT License
