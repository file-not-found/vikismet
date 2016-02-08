# vikismet
GISKismet for [viking](https://github.com/viking-gps/viking)

## Installation
You will need to install the following modules for vikismet to work
* DBI
* XML::LibXML
* DBD::SQLite

## Changes to GISKismet
* html tags removed from kml output
* empty ssids replaced with --cloaked--
* updates positions of known APs in case of better signal

## Howto
import APs: `vikismet -x kismet_file.netxml -d my_database`
create kml file: `vikismet -q "select * from wireless" -d my_database -o out.kml`
