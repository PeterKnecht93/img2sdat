# img2sdat
Convert filesystem images (.img) into sparse Android data images (.dat)

## Requirements
This binary requires Python 3 or newer installed on your system.

## Usage
```
img2sdat [-b] [-c CACHE_SIZE] [-o OUTDIR] input_image [original_image]
```
- `[-b]` = compress data image with Brotli
- `[-c size]` = cache partition size
- `[-o outdir]` = output directory (current directory by default)
- `<input image>` = input partition image
- `[original image]` = original partition image

## Example
This is a simple example on a Linux system:
```
~$ ./img2sdat system.img -o tmp
```
It will create `system.new.dat`, `system.patch.dat` and `system.transfer.list` in the `tmp` directory.

## Info
For more information about this binary, visit it's [XDA page](http://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952).
