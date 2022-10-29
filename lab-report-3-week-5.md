# Lab Report 3
## Command: Grep
### grep -h: displays the matched lines
```
grep -h "base pair" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
sequence, which is a specific series of eight base pairs in the DNA of the bacterial
chromosomes, on the order of one or two thousand base pairs of DNA (or less—their length is
Watson-Crick base pairing, the proximity of the synthetic reactive groups elevates their
```
- `grep -h "base pair" technical/plos/*.txt > bp-results.txt` stores the lines in technical/plos/*.txt that contain "base pair" in bp-results.txt. It's useful because it allows us to find short excerpts and get some context around the sentences in which "base pair" is used in.

```
grep -h "fugitive" technical/911report/*.txt > fugitive-results.txt
cat fugitive-results.txt
In February 1998, the 40-year-old Saudi exile Usama Bin Ladin and a fugitive Egyptian
in tracking fugitives, with much local police knowledge. The department's Drug
fugitives. Responsibility for KSM was transferred to this branch, which gave the CIA
```
- `grep -h "fugitive" technical/911report/*.txt > fugitive-results.txt` stores the lines in technical/911report/*.txt that contain "fugitive" in fugitive-results.txt. It's useful because it allows us to find short excerpts and get some context around the sentences in which "fugitive" is used in.

```
grep -h "Larry" technical/government/Alcohol_Problems/*.txt > larry-results.txt
cat larry-results.txt
Larry Gentilello asserted that effective treatments already
Larry M. Gentilello, MD
Response to Dr. Larry Gentilello's Presentation
Jeffrey Runge agreed with Larry Gentilello that health
```
- `grep -h "Larry" technical/government/Alcohol_Problems/*.txt > larry.txt` stores the lines in technical/government/Alcohol_Problems/*.txt that contain "Larry" in fugitive-results.txt. It's useful because it allows us to find short excerpts regarding Larry and his work.

---

### grep -l: displays the list of file names of which contents include matched word
```
grep -l "base pair" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
technical/plos/journal.pbio.0020190.txt
technical/plos/journal.pbio.0020223.txt
```
- `grep -l "base pair" technical/plos/*.txt > bp-results.txt` stores the files names of files in technical/plos/*.txt that contain "base pair" in the file bp-results. It's useful because it allows for the user to easily pull up the files that regard base pair.
```
grep -l "pathologist" technical/plos/*.txt > path-results.txt                       
cat bp-results.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/pmed.0020017.txt
technical/plos/pmed.0020045.txt
technical/plos/pmed.0020060.txt
```
- `grep -l "pathologist" technical/plos/*.txt > path-results.txt` stores the files names of files in technical/plos/*.txt that contain "pathologist" in the file path-results. It's useful because it allows for the user to easily pull up scientific papers in which a pathologist was involved.
```
grep -l "GABA" technical/biomed/*.txt > gaba-results.txt
cat gaba-results.txt
technical/biomed/1471-2091-3-15.txt
technical/biomed/1471-2091-3-16.txt
technical/biomed/1471-213X-1-1.txt
technical/biomed/1471-2164-4-15.txt
technical/biomed/1471-2164-4-25.txt
technical/biomed/1471-2202-2-1.txt
technical/biomed/1471-2202-2-18.txt
technical/biomed/1471-2202-3-11.txt
technical/biomed/1471-2210-1-2.txt
technical/biomed/1471-2210-3-3.txt
technical/biomed/1472-6807-2-1.txt
```
- `grep -l "GABA" technical/biomed/*.txt > gaba-results.txt` stores the files names of files in technical/plos/*.txt that contain "GABA" in the file gaba-results. It's useful because it allows for the user to easily pull up the scientific papers that refer to GABA. 

---

### grep -n: displays the matched lines and its line numbers
```
grep -n "base pair" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
technical/plos/journal.pbio.0020190.txt:22:        sequence, which is a specific series of eight base pairs in the DNA of the bacterial
technical/plos/journal.pbio.0020190.txt:31:        chromosomes, on the order of one or two thousand base pairs of DNA (or less—their length is
technical/plos/journal.pbio.0020223.txt:46:        Watson-Crick base pairing, the proximity of the synthetic reactive groups elevates their
```
- `grep -n "base pair" technical/plos/*.txt > bp-results.txt` stores the file name, line number, and matched line that contains "base pair" in the file bp-results. It's useful because it allows for the user to find a detailed amount of information of the files that contain "base pair".
```
grep -n "pathologist" technical/plos/*.txt > path-results.txt
cat path-results.txt
technical/plos/journal.pbio.0020012.txt:6:        The pathologist makes do with red wine until an effective drug is available, the
technical/plos/journal.pbio.0020121.txt:120:        it you have,” says veterinary pathologist Beth Williams of the University of Wyoming in
technical/plos/pmed.0020017.txt:58:          All specimens were reviewed by a single reference pathologist (M. F. Z.). Imaging
technical/plos/pmed.0020045.txt:94:          tubular immunostaining was evaluated semi-quantitatively by two independent pathologists
technical/plos/pmed.0020045.txt:192:          independent pathologists in a blinded manner, demonstrated that mean CD36 PTEC scores
technical/plos/pmed.0020060.txt:41:        begin at the autopsy table. Having removed Albert Einstein's brain, pathologist Thomas
```
- `grep -n "pathologist" technical/plos/*.txt > path-results.txt` stores the file name, line number, and matched line that contains "pathologist" in the file path-results. It's useful because it allows for the user to find a detailed amount of information of the files that contain "pathologist".
```
grep -n "Larry" technical/government/Alcohol_Problems/*.txt > larry-results.txt
cat larry-results.txt
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:251:Larry Gentilello asserted that effective treatments already
technical/government/Alcohol_Problems/Session4-PDF.txt:9:Larry M. Gentilello, MD
technical/government/Alcohol_Problems/Session4-PDF.txt:740:Response to Dr. Larry Gentilello's Presentation
technical/government/Alcohol_Problems/Session4-PDF.txt:1137:Jeffrey Runge agreed with Larry Gentilello that health
```
- `grep -n "Larry" technical/government/Alcohol_Problems/*.txt > larry-results.txt` stores the file name, line number, and matched line that contains "Larry" in the file larry-results. It's useful because it allows for the user to find a detailed amount of information of the files and lines that contain "Larry".