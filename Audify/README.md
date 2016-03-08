# moson Project: Audify

## Version 1.0: 08/03/16

### (c) 2016 Paul Vickers

Audify is a Python executable for turning sample data from an Atomic Force Microscope into a 16-bit 44.1 kHz wave audio file.

    usage: Audify [-h] [-i INPUT] [-r RATE] [-o OUTPUT] [-d] [-f] [-n]
                  [-s {tab,comma}] [-m]
    
    optional arguments:
      -h, --help            show this help message and exit
      -i INPUT, --input INPUT
                            Name of input CSV data file
      -r RATE, --rate RATE  Sample rate of original data
      -o OUTPUT, --output OUTPUT
                            Name of output file. If none specfied will have same
                            name as input but with .wav extension
      -d, --debug           Turn on print statements for debugging
      -f, --fade            Turn off the default addition of fade in and out to
                            prevent pops at start and end of audio
      -n, --noskip          Do not skip header row in spreadsheet. Off by default,
                            use -n or --noskip if no header row present
      -s {tab,comma}, --separator {tab,comma}
                            Specify the type of input file: comma separated or tab
                            separated. Default is tab
      -m, --mono            Specify mono output. Default is stereo