<!SLIDE>

## re-downloading is too slow ##

<!SLIDE>

in `~/.pip/pip.conf`:

    @@@ ini
    [global]
    download-cache=/path/to/some/dir

<!SLIDE>

`PIP_DOWNLOAD_CACHE=/path/to/some/dir`


<!SLIDE>

## oh noes! PyPI is down! ##

<!SLIDE>

in `~/.pip/pip.conf`:

    @@@ ini
    [global]
    use-mirrors=true

<!SLIDE>

`PIP_USE_MIRRORS=true`
