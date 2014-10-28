Examples
========
Download MODIS tiles
--------------------
```python
from geobricks_downloader.download.downloader import Downloader


file_paths_and_sizes = [
    {
        'size': None,
        'label': 'H 22, V 05 (21.34 MB)',
        'file_name': 'my_modis_tile.hdf',
        'file_path': 'ftp://ladsweb.nascom.nasa.gov/allData/5/MOD13Q1/2014/001/MOD13Q1.A2014001.h02v08.005.2014018082809.hdf'
    }
]
file_system_structure = '/home/user/Desktop/MODIS'
d = Downloader('modis', file_system_structure, file_paths_and_sizes)
d.download()
```
