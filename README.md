# moon

Data

see downloads.txt

Downloading:

```
$ cat downloads.txt | parallel --bar wget {}
```

convert to tifs

```
$ find *.asc | parallel --bar 'gdalwarp {} {=s:JP2:tif:=}'
```

create vrt in tmp
```
$ mkdir tmp
$ gdalbuildvrt -a_srs EPSG:4326 tmp/ahn.vrt *.tif
```

warp

```
$ docker run -it -v d:\gisdata\moon:/data geodan/terraintiler -b 3 -s 5
```
