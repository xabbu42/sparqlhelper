Description
-----------

sparqlhelper is a small wrapper around the
[Jena](http://incubator.apache.org/jena/) suite of command line tools
to query rdf data. 

Installation
------------

sparqlhelper is easiest to install with [cpanminus](http://search.cpan.org/~miyagawa/App-cpanminus-1.1006/lib/App/cpanminus.pm):

    cpanm --no-lwp --no-wget https://github.com/downloads/xabbu42/sparqlhelper/App-sparqlhelper-0.1.tar.gz

If you want to install sparqlhelper manually you can use the following commands:

    wget --no-check-certificate https://github.com/downloads/xabbu42/sparqlhelper/App-sparqlhelper-0.1.tar.gz
    tar -xzf App-psr-0.3.tar.gz
    cd App-psr-0.3
    perl Makefile.PL
    make
    sudo make install


Usage
-----

See the [manpage](blob/master/Manpage.md) for the documentation.
