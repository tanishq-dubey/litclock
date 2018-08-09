# litclock
Python version of the literary clock made by tjaap

This is a simple literary clock inspired by the [Kindle instructable by tjaap](https://www.instructables.com/id/Literary-Clock-Made-From-E-reader/).
Instead of running on a Kindle however, this runs in your terminal.

## Installing
_pip version coming soon™️_

Simply place `litclock.py` in your `PATH`.
In addition, place the 'times.csv' either in `~/.litclock` or a directory of your choosing.

## Running

### First run with a custom `times.csv` location
If you have placed your `times.csv` in a custom directory, you must first run `litclock` as:

`litclock -r /path/to/your/times/file.csv`

This will generate a precomputed times table (for speed) and store it in '~/.litclock/data.pkl`. Additional options are specified below

### Otherwise

Simply run `litclock` for default behavior. Initial setup will be done automatically.

Full Usage:
```
usage: litclock [-h] [-c] [-r RAW_INPUT_FILE] [-i INPUT_FILE] [-o OUTPUT_FILE]

optional arguments:
  -h, --help            show this help message and exit
  -c, --colored         Use Colorama ANSI colored output
  -r RAW_INPUT_FILE, --raw-input-file RAW_INPUT_FILE
                        Input CSV file, see README for format. Default is in
                        the same directory as the script named "time.csv"
  -i INPUT_FILE, --input-file INPUT_FILE
                        Custom location for input pickle file. Default is in
                        the same directory as the script named "data.pkl"
  -o OUTPUT_FILE, --output-file OUTPUT_FILE
                        Custom location for output pickle file. Default is in
                        same directory as the script named "data.pkl"
```


## Todo
 - [ ] Prefrences file for
 - [ ] Publish to pip
 - [ ] macOS Screensaver version (in a seperate repo)