# starter_traject

This project transforms MARC records into Solr documents using the [Traject](https://github.com/traject-project/traject) tools developed by [Bill Dueber](https://github.com/billdueber/) and [Jonathan Rochkind](https://github.com/jrochkind). This repo was adapted by [Ruth Kitchin Tillman](https://github.com/ruthtillman) from Penn State's Traject project. The project does not include instructions for using Solr, as it is intended for library workers to experiment with building textual indexes via the debug mode.

See my [tutorial for using this repo on your Windows machine](http://ruthtillman.com/tutorial-setting-up-a-traject-project-on-your-windows-machine/).

Setup:

Ignore `gem install bundler` if you already have it installed.

```
git clone https://github.com/ruthtillman/starter_traject.git
cd starter_traject
gem install bundler
bundle install
```

(If on Windows, you may have to clone first, then open your Ruby terminal and change directories to your starter_traject project, then run `gem install bundler` followed by `bundle install`.)

For testing purposes you can run `traject` with the `--debug-mode` flag to display the output to the console (and not push the data to Solr).

```
traject --debug-mode -c sample_config.rb /full/path/to/marcfile.mrc
```

To write it out to a file, use the `> filename.txt` command to write it to a text file, e.g.

```
traject --debug-mode -c sample_config.rb /full/path/to/marcfile.mrc > sample_index.txt
```
