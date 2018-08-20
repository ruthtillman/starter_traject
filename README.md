# starter_traject

This project transforms MARC records into Solr documents using the [Traject](https://github.com/traject-project/traject) tools developed by [Bill Dueber](https://github.com/billdueber/) and [Jonathan Rochkind](https://github.com/jrochkind). This repo was adapted by [Ruth Kitchin Tillman](https://github.com/ruthtillman) from Penn State's Traject project. The project does not include instructions for using Solr, as it is intended for library workers to experiment with building textual indexes via the debug mode.

Setup:

```
git clone https://github.com/ruthtillman/starter_traject.git
cd starter_traject
bundle install
```

For testing purposes you can run `traject` with the `--debug-mode` flag to display the output to the console (and not push the data to Solr).

```
traject --debug-mode -c sample_config.rb /full/path/to/marcfile.mrc
```

To write it out to a file, use the `> filename.txt` command to write it to a text file, e.g.

```
traject --debug-mode -c sample_config.rb /full/path/to/marcfile.mrc > filename.txt
```
