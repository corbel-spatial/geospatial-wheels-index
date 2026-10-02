# Geospatial Wheels Index

This is a `pip`-compatible package index for releases in cgohlke's [geospatial-wheels](https://github.com/cgohlke/geospatial-wheels),
which provides precompiled binary wheels for common geospatial Python libraries on Windows.

Simply use `pip install` with the `--index` flag, for example to install `GDAL`:

```shell
pip install --index https://gisidx.github.io/gwi gdal
```

The current release supports Python 3.12 through 3.15 on `win_arm64`, `win_amd64`, and `win32` architectures 
for the following packages:

- [basemap](https://pypi.org/project/basemap/)
- [Cartopy](https://pypi.org/project/Cartopy/)
- [cftime](https://pypi.org/project/cftime/)
- [Fiona](https://pypi.org/project/Fiona/)
- [GDAL](https://pypi.org/project/GDAL/)
- [netCDF4](https://pypi.org/project/netCDF4/)
- [pyogrio](https://pypi.org/project/pyogrio/)
- [pyproj](https://pypi.org/project/pyproj/)
- [rasterio](https://pypi.org/project/rasterio/)
- [Rtree](https://pypi.org/project/Rtree/)
- [shapely](https://pypi.org/project/shapely/)
- [tables](https://pypi.org/project/tables/)

Additional packages from past releases (`h5py`, etc.) are also available in this index. 

To install all packages with `uv`:

```shell
uv pip install --index https://gisidx.github.io/gwi basemap cartopy cftime fiona gdal netcdf4 pyproj rasterio rtree shapely tables
```

Or using `pip`:

```shell
# First install dependencies from PyPI 
pip install affine attrs basemap_data blosc2 certifi click click-plugins cligj matplotlib numexpr numpy packaging py-cpuinfo pyshp
# Then the packages from the index
pip install --index https://gisidx.github.io/gwi basemap cartopy cftime fiona gdal netcdf4 pyproj rasterio rtree shapely tables
```

### Notes

- The index is hosted on this repository's GitHub Pages site: https://corbel-spatial.github.io/geospatial-wheels-index/

- For convenience, a [forked repository](https://github.com/gisidx/gwi) provides this shorter index URL: https://gisidx.github.io/gwi

- The index does not contain any actual wheel files; all links point to the GitHub-hosted assets in [releases](https://github.com/cgohlke/geospatial-wheels/releases)
maintained in the `cgohlke/geospatial-wheels` repository.

- The index automatically syncs with `cgohlke/geospatial-wheels` every Tuesday at 21:00 UTC. Please open an [Issue](https://github.com/corbel-spatial/geospatial-wheels-index/issues) if it's out of date.

- Like the `geospatial-wheels` source, this index is provided "as is" and without warranty of any kind. 

- All aspects of this index are open source and hosted in this repository.
Thus it is fully auditable and you are welcome to fork it to create your own version.
Questions and suggestions are welcome in the [Issues](https://github.com/corbel-spatial/geospatial-wheels-index/issues) section.
