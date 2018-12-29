# ALAC (Apple Lossless Audio Codec) command-line utils

## mkalac

Converts ape+cue, wv+cue, flac+cue, flac to ALAC (.m4a) files. \n
This utility is only tested on MacOS Mojave so be careful when running in the other platform

#### Dependencies:
Install the following packages: `ffmpeg flac shntool cuetools`

#### Usage:
	mkalac  <cuefile>                     # with auto encoding
	mkalac  <cuefile> <-e> <encoding>     # with encoding in the option -e, use 'iconv -l' to view the supported encoding
	mkalac  <flacfile>
	mkalac  <directory>                   # with auto encoding for cue files
	mkalac  <directory> <-e> <encoding>   # with encoding in the option -e, use 'iconv -l' to view the supported encoding
