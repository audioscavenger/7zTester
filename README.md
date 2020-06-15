# 7zTester
Benchmark for 7zip: compress a list of files with different settings and factors, produces a CSV 

## Purpose:
- Benchmark for 7zip: compress a list of files with different settings and factors:
   + Temporary folders: to test if drive overhead really matters
   + methods by their extention: zip, 7z, add your own...
   + compression levels: 0 1 3 5 7 9
- finally gather time and size data to produce a CSV output you can play with
- for more information on 7z switches, see https://sevenzip.osdn.jp/chm/cmdline/switches/


## Usage:
1. setup _:defaults_, _:init_ and _:prechecks_ in the batch
2. run the batch and enjoy
3. parameters accepted: -D -V -l


## Features:
- auto-detection of 7zip on your system
- colors
- a wealth of parameters can be ajusted
- parametric output field list easy to update


## Requisites:
- 7z.exe
- awk.exe (optional)
- get_date_format.cmd
- get_timelapse.cmd
- 64bit Windows recommended


## Changelog:
* 1.1  accomodate special chars
* 1.2  default compression level is 5, among 1,3,5,7,9
* 1.3  CSV field names and list is parametrable
* 1.4  CSV and LOG using CPU name
* 1.5  fix OUTPUTFOLDER
* 1.6  make sure testFile EXT is included in zipFile name


## TODO LIST:
- [ ] add files to tests as parameter
- [ ] add :arguments function to process more agruments
- [ ] add unzip to tests decompression speed?
- [ ] include get_timelapse.cmd and get_date_format.cmd in this batch to get rid of requisites?
- [ ] try and get rid of these unix binaries?

Screenshots
-----------
![Output](https://github.com/audioscavenger/7zTester/blob/master/assets/7zTester-1.6-output.png)

