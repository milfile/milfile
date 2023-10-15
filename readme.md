# milfile

Milfile, <i>stylized</i> milfile is a WIP markup language based off Markdown and HTML. below is a list of valid syntax, tags, etc.


## Header1

```milfile
+ header1test
```

Result:

# header1test

## Header2

```milfile
++ header2test
```

Result: 

## header2test

## Header3

```milfile
+++ header3test
```

Result:

### header3test

## Header4

```milfile
++++ header4test
```

Result:

#### header4test

## Header5

```milfile
+++++ header5test
```

Result:

##### header5test

## Header6

```milfile
++++++ header6test
```

Result:

###### header6test

## Comments

```xml
<!-- comment -->
```

## Scripting

Options:

- VBScript (limited)
- PHP
- JavaScript (through PHP/HTML, not supported)

Alternatively, milfile can parse:

+ HTML (through PHP, not supported by milfile)
+ CSS (through HTML, not supported by milfile)
+ JavaScript DOMs (through PHP/HTML, not supported)
+ XML (supported, php and vbscript cannot be executed until cancel)

```milfile
~! Register

<?php
%loadsql=true;
%user="username";
?><p>If you wish to register, please enter your proposed <? %user?> below</p>
```

below is a client-side example (vbscript):

```milfile
<?php ?><center><?mil>404... `!something went wrong!`
<?milv vbscript=

msgbox("An error has occured, we'll try to keep running.")
?milv>
```

