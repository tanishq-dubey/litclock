# litclock
Python version of the literary clock made by tjaap

This is a simple literary clock inspired by the [Kindle instructable by tjaap](https://www.instructables.com/id/Literary-Clock-Made-From-E-reader/).
Instead of running on a Kindle however, this runs in your terminal.

A literary clock is a timekeeping device that uses quotes from literature to tell the time.

## Installing
_pip version coming soon™️_

Simply place `litclock.py` in your `PATH`.
In addition, place the 'times.csv' either in `~/.litclock` or a directory of your choosing.

## Running

### First run 
If you are ok with `~/.litclock` as a directory for your CSV and data files, you can simply run `litclock` and be on your way. Otherwise...

If you have placed your `times.csv` in a custom directory, you must first run `litclock` as:

`litclock -r /path/to/your/times/file.csv`

This will generate a precomputed times table (for speed) and store it in '~/.litclock/data.pkl`.

If you require the precomputed array in a different location, you may specify so with 

`litclock -o /path/to/your/output.file`

If a seperate data output location is set, then on ever run, you must run as `litclock -i /path/to/your/output.file`

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
 - [ ] Prefrences file settings
 - [ ] Publish to pip
 - [ ] macOS Screensaver version (in a seperate repo)
