# PaleoMag Converter

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Purpose

This script was created to convert individual sample files previously
made by Data Splitter into generic PmagPy format. Files produced by this 
script can be used with PmagPy Demag GUI and paleomagnetism.org. Field intensity
is output in A/m assuming a sample volume of 10cc. 

![Demo data.](/assets/input-output.png)

## How to use

1) Put individual sample files (such as those split by [Data Splitter](https://github.com/katiebristol/data_splitter)) that you want 
converted into the /input/ folder.
2) Set AF or thermal demag via line 32 (default is AF):

```next_line = " ".join(str(x) for x in next_line_array).replace("Cm","A")``` for AF demag

```next_line = " ".join(str(x) for x in next_line_array).replace("Cm","T")``` for thermal demag

3) Run the script
4) Check the /output/ folder for your converted files. 

## Inputs

This script requires .dat files that you want converted placed into the
/input/ folder. 

## Outputs

This script will create converted files with the same name. 
The converted files will write to the /output/ folder. 

## Notes

This script was made in conjunction with the Data Splitter script.
It is intended to be used afterwards to convert data to PmagPy generic/paleomagnetism.org friendly formats.

## License

This script is published under the [MIT license](LICENSE.txt).