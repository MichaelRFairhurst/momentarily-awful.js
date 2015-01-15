# momentarily-awful.js
 bring a moment of awfulness to your codebase with this amateur-inspiring date formatting library, which makes it a principle to allow infinite formatting possibilities by treating dates as objects with functions that return numbers.

Also, the source code is tiny, weighing in at jut 65 bytes.

=========================

## Usage

momentarily-awful.js formats are a superset of javascript. There is one special character in momentarily-awful.js formats

* `d` - indicates the date you are formatting

But don't let that turn you off, because all of JavaScript is made available to you as well!

## Example formats:

* Get day - `momentarilyAwful(date, "d.getDay()+1");`
* Get month - `momentarilyAwful(date, "d.getMonth()+1");`
* Get year - `momentarilyAwful(date, "d.getFullYear()");`

## Plugins

To reduce boilerplate you can easily define modules:

    'using momentarilyAwful';
    function m(d) {
        return d.getMonths() > 9 ? d.getMonths() + 1 : '0' + (d.getMonths() + 1);
    }

And use it just as easily:

    momentarilyAwful(date, "m(d)");
