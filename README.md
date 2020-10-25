[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

# pdfsplitter

`pdfsplitter` is a simple python script which runs on linux systems
and uses [`pdftk`](https://wiki.ubuntuusers.de/pdftk/) to split
a pdf into evenly sized chunks.

The default chunk-size is 90 and may be changed with the `-c` option (see `--help` for a list of all arguments). Example:

```bash
pdfsplitter -c 2 example-document.pdf
```

Will create multiple pdfs with 2 pages each (this can exclude the last chunk which may shrink to the appropriate value).
Chunk-sizes which are smaller than or equal to zero are forbidden.
