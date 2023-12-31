PyFlashToGPS
============

PyFlashToGPS is a command line utility to analyze a flash-tagged FITS video from SharpCap and add GPS accurate
timestamps to the DATE-OBS meta-data for each frame.

usage: PyFlashToGPS [-h] [--verbose] [--QHY174GPS] [--fits FITS_path] flash_times
                
A utility to add GPS accurate timestamps to flash-tagged FITS videos recorded by SharpCap.

positional arguments:
  flash_times       UTC times for first and last flash. Example: "2023-09-02 13:45:10 2023-09-02 13:47:05" (the quotes are needed!)

options:
  -h, --help        show this help message and exit
  --verbose         Verbose output (used during development)
  --QHY174GPS       If file came from a QHY174GPS camera, a comparison report
                    is made between the GPS timestamps
  --fits FITS_path  Full path to FITS folder - enclose in quotes if spaces are present
