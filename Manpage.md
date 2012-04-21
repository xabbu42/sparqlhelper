# NAME

sparqlhelper - Simplify SparQL query formulation on the command line.

`sparqlhelper` uses the given sparql where clause to construct a
complete query, by selecting distinct values for all not repeated
variable names longer than one char in the where clause. So the query
`?s a ?class` selects and outputs all distinct classes in the data
set. Moreover, known prefixes used in the where clause are added from
the data of http://prefix.cc.

The complete sparql query is per default just output to stdout, but
can be directly passed on to arq for convenience. This is enabled by
passing some arq options like `--data` or `--service` to the command
line. In this case, also all known prefixes from prefix.cc are added
to the query to simplify the output.

# SYNOPSIS

sparqlhelper \[OPTIONS\] QUERY

    --help,-h      Brief help message.
    --ask,-a       Use ask instead of select query.
    --explain,-e   Explain and log query execution.
    --data,-d      Data file to use (passed on to sparql).
    --service,-r   Service endpoint to use (passed on to rsparql).
    --loc,-l       TDB location to use (passed on to tdbquery).
    --source,-s    Data source (can be a file with rdf data, a endpoint url or a tdb location)
    --prefix,-p    Add a prefix to the query in the form prefix=uri.
                   Known prefixes from prefix.cc are recognized instead 
                   of a uri.



# AUTHOR

    Nathan Gass <gass@search.ch>