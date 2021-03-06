# ALAC (Apple Lossless Audio Codec) command-line utils

## mkalac

	Converts ape+cue, wv+cue, flac+cue, flac, wav to ALAC (.m4a) files.

	This utility is only tested on MacOS Mojave so it may not work in the other platform, 
	but it should be safe to try as it won't delete any of your files.

#### Dependencies:
	This project is dependent on packages: `ffmpeg flac shntool cuetools`.
	Use 'brew list' to check your installed packages.
	Use 'brew install ffmpeg flac shntool cuetools' to install
	

#### Usage:


	Copy 'mkalac' to your Mac's /usr/local⁩/⁨bin/ folder⁩
	Then below should work - 
	
	mkalac  <cuefile>                     # with auto encoding
	mkalac  <cuefile> <-e> <encoding>     # with encoding in the option -e, use 'iconv -l' to view the supported encoding
	mkalac  <wavfile>                     # with auto encoding
	mkalac  <wavfile> <-e> <encoding>     # with encoding in the option -e, use 'iconv -l' to view the supported encoding
	mkalac  <flacfile>
	mkalac  <directory>                   # with auto encoding for cue files
	mkalac  <directory> <-e> <encoding>   # with encoding in the option -e, use 'iconv -l' to view the supported encoding
	
	For Chinese users, if you met 'iconv' errors, please try encoding GB18030 or BIG5
	example:
	mkalac <Yourpath>/YourFileName.cue -e GB18030
	mkalac <YourPath>/YourFileName.wav -e BIG5
