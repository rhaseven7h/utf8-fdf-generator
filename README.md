UTF-8 FDF File Generator
========================

PDF file form filler file (FDF) generator.

Generates FDF files based on UTF-16 (you don't have to convert anything) so they support UTF-8 characters.

General Information
-------------------

- For more information see the [Home Page].
- Or the [Repository]

Usage
-----

Its is synchronous, just call it, upon return, the file will be already created and you can use it:

``` JavaScript
generator = require('utf8-fdf-generator').generator;
generator({ myField01: "Gabriel Medina", myField02: "Ciudad Juárez, Chihuahua, México" }, "output.fdf");
// Do whatever you need with file output.fdf here.
```

You usually do something like:

```bash
user@server:~ $ pdftk template.pdf fill_form generated.fdf output final_output.pdf flatten
```

Where:

- `template.pdf` is the original PDF form
- `generated.fdf` is the file we generated
- `final_output.pdf` is the PDF file with fields filled using data from `generated.fdf`


[Home Page]:http://rhaseventh.blogspot.mx/2014/04/node-js-pdf-fill-from-fdf-with-utf-16.html
[Repository]:https://github.com/Rhaseven7h/utf8-fdf-generator

Regards,

[Gabriel Medina] 

Twitter: [@_Rha7_]

[Gabriel Medina]:mailto:rha7.com@gmail.com
[@_Rha7_]:https://twitter.com/_Rha7_
License
----
MIT

**Free Software, Hell Yeah!**

