*This repository is a mirror of the [component](http://component.io) module [matthewmueller/helix](http://github.com/matthewmueller/helix). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/matthewmueller-helix`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# helix

  jquery-like dom manipulation. Tiny (1kb minified & gzipped)

## Installation

    $ component install matthewmueller/helix

## API

### Helix(el)

Create a Helix instance.

```js
var $ = Helix(document.getElementById('person'));
```

### $(selector)

Select an element.

```js
$('.name')
$('#nav')
```

### #\[attr\](val)

Get and set attributes that are on the selected element.

```html
<input class="user" id="user" type="text" name="user">
```

```js
$('.user').type('radio').name('person')
$('.user').type() // radio
```

### #text(val)

Get and set text

```js
$('.name').text('Matt')
$('.name').text() // Matt
```

### #html(val)

Get and set HTML

```js
$('.name').html('<strong>Matt</strong>')
$('.name').html() // <strong>Matt</strong>
```

### #addClass(cls)

Add a class

```js
$('.name').addClass('person')
```

### #removeClass(cls)

Remove a class

```js
$('.name').removeClass('person')
```

### #toggle(cls)

Toggle a class

```js
$('.name').toggle('person')
```

### #attr(attr, val)

Get and set attribute that doesn't already exist

```js
$('.name').attr('data-author', 'matt')
```

## License

  MIT
