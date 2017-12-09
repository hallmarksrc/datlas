# `Datlas`

`Datlas` is a python package for high performance data modeling.

Given the rapidly increases in data volumes, standard python data
structures such as tuples, lists, and dicts can no longer satisfy the
needs of modern computation- and data-intensive applications.
Array- and table-oriented packages such as `numpy` and `pandas` have
became the foundations of python data processing.
However, `numpy` arrays and `pandas` dataframes don't integrate with
python's object-oriented programming paradigm well.
This makes data modeling difficult.
Developers either fall back to the traditional procedural programming
approach and use these packages as containers to handle their data; or
forgo the performance benefit of these packages to pay the object
overhead.

`Datlas` provides the best of the both worlds by storing object data
in `numpy` arrays or `pandas` dataframes and mapping views of data
entries into objects.
This approach is very similar to object–relational mapping (ORM), such
as Apple's Core Data, that provide an object-native interface to a
high performance data serving backends.
The main differences here is that the data backends don't have to be a
relational database.
Instead, any high performance data tool can in principle be used as a
`datlas` backend.
