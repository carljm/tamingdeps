<!SLIDE>

# option 2 #

<!SLIDE incremental>

## dump some tarballs in a directory ##

* `--find-links` can inject arbitrary URLs into the link-scraping
* point it at a web-served directory of sdists with indexes on
* this option can also go directly in a requirements file
* file:// URLs work too, pip will get the directory listing
* if you don't want PyPI used at all, add `--no-index`
* easily populate with `pip install -d my-sdists-dir/ SomePackage`

<!SLIDE commandline incremental>


`--find-links http://internal.example.com/sdists/`

or

`--find-links file:///path/to/my/sdists/`

    $ tree
    .
    |-- Django-1.3.tar.gz
    `-- django-floppyforms-0.4.2.tar.gz


<!SLIDE incremental>

## find-links ##

* trivial to maintain manually
* very fast with `file://` URL and `--no-index`
* can be self-contained with project
