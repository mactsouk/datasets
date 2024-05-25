# datasets
Data sets for experimenting with Visualization tools and data mining techniques.


### For the `./EEG/EEG_LSF5.txt.gz` data file, we need to put each value in a separate line, which can happen as follows:

`zcat ./EEG/EEG_LSF5.txt.gz  | sed 's/\\n/ /g' | tr " " \\n\n | > file.txt`

Based on the file size, we can split each file using `head` and `tail`. The file size can be calculated using `wc`.

### Remove traling zeros off a floating number
`sed 's/0\{1,\}$//'`

