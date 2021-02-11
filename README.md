# Blank repo for Bootstrap Studio to create PHP site
----------
**** Including the PHP form files
> tested on Bootstrap Studio 5.1.1
## Instructions
1. ### Install via npm
> git clone https://github.com/MBaroky/bss-to-php-blank.git

2. ### Create Bootstrap Studio Template with files:
- header.html [then add these blocks of code](#in-header)
- footer.html [then add these blocks of code](#in-footer)
- index.html [then add these blocks of code](#in-index)
- contact.html [then add these blocks of code](#in-contact)

3. ### In export advance options add
`<path where installed bss-to-php-blank>/PHPer.bat`

4. ### On each additional page
> take care don't use name: form.html

> in PHPer.bat:
> at line #8 inside `()` add `, <your file's name without extention>.php`

#### In header
at the beginning of file:

```\<\!--for active case and mobile detect: optional--\>\
<?php
$activePage = basename($_SERVER['PHP_SELF'], ".php");
function isMobile() {
    return preg_match("/(android|avantgo|blackberry|bolt|boost|cricket|docomo|fone|hiptop|mini|mobi|palm|phone|pie|tablet|up\.browser|up\.link|webos|wos)/i", $_SERVER["HTTP_USER_AGENT"]);
}
?>

```

in the end of file:

```\<!\--end of header.php--\>\

```

#### In footer
#### In index
#### In contact


