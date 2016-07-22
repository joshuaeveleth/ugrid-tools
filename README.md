[![Build Status](https://travis-ci.org/NESII/fm-tools.svg?branch=master)](https://travis-ci.org/NESII/fm-tools)

```
$ python src/fmtools_cli.py convert --help
Usage: fmtools_cli.py convert [OPTIONS]

  Create ESMF unstructured NetCDF files from polygon ESRI Shapefiles.

Options:
  -u, --source_uid TEXT         Name of unique identifier in source shapefile.
                                [required]
  -s, --source PATH             Path to input shapefile.  [required]
  -e, --esmf_format PATH        Path to the output ESMF unstructured NetCDF
                                file.  [required]
  -n, --node-threshold INTEGER  (default=10000) Approximate limit on the
                                number of nodes in an element part. The
                                default node threshold provides significant
                                performance improvement.
  --help                        Show this message and exit.
```

```
$ python src/fmtools_cli.py merge --help
Usage: fmtools_cli.py merge [OPTIONS]

  Create a merged ESMF weights file.

Options:
  -c, --catchment-directory TEXT  Path to the directory containing the ESMF
                                  unstructured files.  [required]
  -w, --weight-directory PATH     Path to the directory containing the weights
                                  files.  [required]
  -m, --master-path PATH          Path to the output merged weight file.
                                  [required]
  --help                          Show this message and exit.
```