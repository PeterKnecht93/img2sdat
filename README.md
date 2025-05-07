# img2sdat
Convert sparse filesystem images (.img) into sparse Android data images (.dat)

## Requirements
This binary requires Python 3 or newer installed on your system.

## Usage
```
img2sdat.py <partition_img> [-o outdir]
```
- `<partition_img>` = input partition image
- `[-B map_file]` = block map file
- `[-c size]` = cache partition size
- `[-o outdir]` = output directory (current directory by default)

## Example
This is a simple example on a Linux system:
```
~$ ./img2sdat.py system.img -o tmp
```
It will create `system.new.dat`, `system.patch.dat` and `system.transfer.list` in the `tmp` directory.

## Info
For more information about this binary, visit it's [XDA page](http://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952).
