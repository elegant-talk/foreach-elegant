<!-- TITLE -->

<!-- BADGES -->

<!-- DESCRIPTION -->

<!-- INSTALL -->

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

<!-- HISTORY -->

<!-- BACKERS -->

<!-- LICENSE -->
