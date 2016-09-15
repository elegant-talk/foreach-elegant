<!-- TITLE/ -->

<h1>foreach-elegant</h1>

<!-- /TITLE -->


<!-- BADGES/ -->



<!-- /BADGES -->


<!-- DESCRIPTION/ -->

A foreach that supports arrays and objects, provides the value and key/index, as well as break support on return false

<!-- /DESCRIPTION -->


<!-- INSTALL/ -->

<h2>Install</h2>

<a href="https://npmjs.com" title="npm is a package manager for javascript"><h3>NPM</h3></a><ul>
<li>Install: <code>npm install --save foreach-elegant</code></li>
<li>Module: <code>require('foreach-elegant')</code></li></ul>

<!-- /INSTALL -->


## Usage

``` javascript
var foreach = require('foreach-elegant')
function iterator (value, key, list) {
    console.log('received', key, '=', value, 'from', list)
    if ( key === 'b' || value === 'y' ) {
        console.log('ending iteration early')
        return false
    }
}

foreach({a:1, b:2, c:3}, iterator)
foreach(['x', 'y', 'z'], iterator)

foreach({a:1, c:3}, iterator)
foreach(['x', 'z'], iterator)
```

<!-- HISTORY/ -->

<h2>History</h2>

<a href="https://github.com/bevry/foreach-elegant/releases">Discover the release history by heading on over to the releases page.</a>

<!-- /HISTORY -->


<!-- BACKERS/ -->

<h2>Backers</h2>

<h3>Maintainers</h3>

No maintainers yet! Will you be the first?

<h3>Sponsors</h3>

No sponsors yet! Will you be the first?



<h3>Contributors</h3>

These amazing people have contributed code to this project:

<ul><li><a href="http://balupton.com">Benjamin Lupton</a> — <a href="https://github.com/bevry/foreach-elegant/commits?author=balupton" title="View the GitHub contributions of Benjamin Lupton on repository bevry/foreach-elegant">view contributions</a></li></ul>



<!-- /BACKERS -->


<!-- LICENSE/ -->

<h2>License</h2>

Unless stated otherwise all works are:

<ul><li>Copyright &copy; 2016+ <a href="http://bevry.me">Bevry Pty Ltd</a></li></ul>

and licensed under:

<ul><li><a href="http://spdx.org/licenses/MIT.html">MIT License</a></li></ul>

<!-- /LICENSE -->
