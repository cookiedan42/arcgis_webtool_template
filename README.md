# arcgis_webtool_template

arcgis `.pyt` python toolboxes can be uploaded as webtool  
however there are pitfalls in import parsing


## import of individual python files
`import x` will include the `x.py` file in the build  
`from x import y` will not include `x.py` file in the build

## import of packages/modules  
including `samplemodule/` using the method of path string will upload the `samplemodule/` directory into the build  
However, `import samplemodule` will not work because ???
