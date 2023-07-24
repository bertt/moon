# moon

Data

```
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_0N_60N_000_120.JP2

wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_0N_60N_120_240.JP2
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_0N_60N_240_360.JP2
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_60S_0S_000_120.JP2
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_60S_0S_120_240.JP2
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_256_60S_0S_240_360.JP2
wget http://imbrium.mit.edu/DATA/SLDEM2015/TILES/JP2/SLDEM2015_512_00N_30N_000_045.JP2

```

warp
```
$ docker run -it -v d:\gisdata\moon:/data geodan/terrainwarp -c epsg:9122 

```