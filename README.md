#TOOLS STORE

Tool store is basically a file containig all tools &  its functions ,errors used during 4years of my Btech Journey

##1.FFMPEG

-FFMPEG is a universal media converter tool which to convert one media format to another like converting .mp4 to .jpeg
-first command = ffmpeg -i <inputfile> <outputfile>
e.g: ffmPeg -i Nature.mp4 -vframes 1 a.jpeg -- is used when we need to just covert 1 frame of .mp4 to .jpeg using -vframes option between input file and output file

-second command -- ffmpeg -i Nature.mp4 thumbnail.gif-- here we changed .mp4 to gif format

-third command -- ffmpeg -i Nature.mp4 -t 3 cod.gif -- here, we shortened the .gif file taking -t 3 which contains output of duration of first 3 sec 

-fourth command -- ffmpeg-i Nature.mp4 -vf "fps=10,scale=320:-1" modified.gif--here we applied filters to gif file i.e fps and scale with height -1 making it smoother and shorter"

ERROR 1 - ffmpeg -i Nature.mp4 thumbnail.jkdd --this code breaks because there is an error in code as .jkdd isn't a standard extension for the filename so that .mp4 could be changed to .jkdd ,that's why this shows an error

ERROR 2- ffmpeg -i Nature.mp4 -vf "fps=10,sale:320:-1" --here error comes as ffmpeg could not tell which filter it belongs to, as there was typo in scale option.

##2. QRENCODE.

- QRENCODE  is basically a tool for creating qr code for given input and save it as png or eps image .
- for detailed documentation use "man qrencode" command in terminal.

-first command -- qrencode -o qr.png "not enough" -- this command outputs qr.png image containg string of texts "not enough".
here is the general form for 1st command -- qrencode -o <filename.png> "string of characters to be contained in qr code created " -- always put text into double quotes and -o means output .

-second command -- qrencode -o git.png "https://github.com/yasharya444/concept_trial.git" -- this code outputs git hub repo link into git.png image , making link access via qr code generated.

-ERROR 1 -- qrencode -n qr.png "not enough" -- This command breaks as -n is an invalid option it shall be -o to give output.

Note: HERE , qrencode in all commands is necessary as it represents which tool is being used and even typo in it causes command to break.

