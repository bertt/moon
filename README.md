# moon

Demo

https://bertt.github.io/moon/cesium/

Data

see downloads.txt

Downloading:

```
$ cat downloads.txt | parallel --bar wget {}
```

convert to tifs

```
$ find *.JP2 | parallel --bar 'gdalwarp {} {=s:JP2:tif:=}'
```

create vrt in tmp
```
$ mkdir tmp
$ mv *.tif ./tmp
$ gdalbuildvrt -a_srs EPSG:4326 tmp/ahn.vrt tmp/*.tif
```

warp

```
$ docker run -it -v $(pwd):/data geodan/terraintiler -b 3 -s 5
```
