# dmdSchemeRepository
This is a repository for dmdSchemes. The schemes are in the folder `schemes`.

They are `.tar.gz` files which contains **a folder named  `NAME_VERSION`**. The content of the folder depends on the `schemePackageVersion`.

The folder is copied into the `dmdSchemePackageDir/installedSchemes` folder.

Below, the different versions are explained in detail.

To add a scheme definition please either
- clone the repo and send a pull request
- contact the maintainer of this repo at Rainer.Krug@uzh.ch

## **1.0.0**

### The package contains at least the folllowing files

- `schemePackageVersion`: version of the scheme package format (`1.0.0`)
- `NAME_VERSION.xlsx`: definition including example data
- `NAME_VERSION.xml`: exported from `NAME_VERSION.xlsx` with `output = complete` and `keepData = TRUE`, i.e. it contains the scheme definition and the example data and is equivalent to `NAME_VERSION.xlsx`
- `md5sum.txt`: contains the md5 checksums of all files in the pckage

### Supported but not required are also

- a folder with the name `examples` containing subfolders with foldes containing examples. The name of the example is the name of the subfolder under `examples`. The example can contain an `html` file with the name `name_of_the_example.html` which is opened automatically when calling `make_example("name_of_the_example")`. Otherwise, there are no restrictions to the contents of the example.
