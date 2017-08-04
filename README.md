# Note

This is a yet another fork of http://git.bytbox.net/sloc

It exists solely because upstream seems dead :/

You can install my own version of sloc with

```console
$ go got github.com/dmerejkowsky/sloc
```

Following in the rest of upstream's README

# SLOC - Source Lines Of Code

`sloc` is a simple, do-one-thing-well program to calculate code statistics: the
number of lines in a project, and how much of that is code versus comment.

    $ sloc ~/misc/opt/go
        Language  Files    Code  Comment  Blank   Total
           Total   2808  512357    87177  67791  667325
              Go   2048  295054    62020  37973  395047
               C    474  166702    22330  21849  210881
            HTML     58   25627      183   4241   30051
        Assembly    131    9974      161   1491   11626
            YACC      6    5245      363    449    6057
          Python      6    2940      789    495    4224
      JavaScript      6    2526      496    585    3607
             XML      9     974       15     90    1079
           Shell      9     905      380    155    1440
             CSS      6     899       24    119    1042
            Perl      9     854      159    135    1148
            Bash     13     483      151    122     756
            Make     33     174      106     87     367

`sloc` cannot understand gitignore or hgignore, nor can it distinguish between
"real" source and auto-generated files, so for best results, run it on a fresh
repository with no compilation done.

You can generate JSON output with the `-json` flag, if that's easy to parse in
the programming/scripting language of your choice.

Install `sloc` with:

    $ go get github.com/dmerejkowsky/sloc

## `reposloc`

For graphing amount of code over time (as revealed by a git or mercurial
repository), a `reposloc` perl script is provided. This is not installable via
the `go` tool. Consult the man page for usage information.
