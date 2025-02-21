# Time-alignment of CESA transcripts (with conversion to WebVTT format)
This R script was used to autogenerate timestamps in CESA transcripts for each speaker turn based on existing timestamps occuring every minute. After formatting the transcript according to WebVTT standards, the duration between each timestamp is calculated and divided in equal increments between different speakers.

### How to use:
- Download and open the R script
- Set the `files_dir` variable on line 27 to a local directory folder that contains .txt transcript files (with timestamps formatted like `[00:00:00]` sprinkled throughout, including a final timestamp at the end)
- Edit the name of the subfolder to place the outputted files on line 28 (new or existing)
- Run in sections or all at once; the resulting files should be in the `files_dir/subfolder` path

### WebVTT validation of resulting files
To validate the files are correctly formatted as WebVTT files, this [web-based validator](https://w3c.github.io/webvtt.js/parser.html) can be used. To validate in bulk, the bulk validation tool can be used.
