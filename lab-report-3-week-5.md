# Lab Report 3
## Command: Grep
### grep -h
```
grep -h "base pair" technical/plos/*.txt > bp-results.txt
docsearch:432$ cat bp-results.txt
sequence, which is a specific series of eight base pairs in the DNA of the bacterial
chromosomes, on the order of one or two thousand base pairs of DNA (or less—their length is
Watson-Crick base pairing, the proximity of the synthetic reactive groups elevates their
```
- grep -h displays the matched lines

```
docsearch:445$ grep -h "fugitive" technical/911report/*.txt > bp-results.txt
cat bp-results.txt
In February 1998, the 40-year-old Saudi exile Usama Bin Ladin and a fugitive Egyptian
in tracking fugitives, with much local police knowledge. The department's Drug
fugitives. Responsibility for KSM was transferred to this branch, which gave the CIA
```
- what it's doing and why it's useful

```
grep -h "Larry" technical/government/Alcohol_Problems/*.txt > bp-results.txt
cat bp-results.txt
Larry Gentilello asserted that effective treatments already
Larry M. Gentilello, MD
Response to Dr. Larry Gentilello's Presentation
Jeffrey Runge agreed with Larry Gentilello that health
```
- what it's doing and why it's useful

### grep -l
```
grep -l "base pair" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
technical/plos/journal.pbio.0020190.txt
technical/plos/journal.pbio.0020223.txt
```
- what it's doing and why it's useful
```
grep -l "pathologist" technical/plos/*.txt > bp-results.txt                       
cat bp-results.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/pmed.0020017.txt
technical/plos/pmed.0020045.txt
technical/plos/pmed.0020060.txt
```
- what it's doing and why it's useful
```
grep -l "GABA" technical/biomed/*.txt > bp-results.txt
cat bp-results.txt
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
- what it's doing and why it's useful

### grep -n
```
grep -n "base pair" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
technical/plos/journal.pbio.0020190.txt:22:        sequence, which is a specific series of eight base pairs in the DNA of the bacterial
technical/plos/journal.pbio.0020190.txt:31:        chromosomes, on the order of one or two thousand base pairs of DNA (or less—their length is
technical/plos/journal.pbio.0020223.txt:46:        Watson-Crick base pairing, the proximity of the synthetic reactive groups elevates their
```
- what it's doing and why it's useful
```
grep -n "pathologist" technical/plos/*.txt > bp-results.txt
cat bp-results.txt
technical/plos/journal.pbio.0020012.txt:6:        The pathologist makes do with red wine until an effective drug is available, the
technical/plos/journal.pbio.0020121.txt:120:        it you have,” says veterinary pathologist Beth Williams of the University of Wyoming in
technical/plos/pmed.0020017.txt:58:          All specimens were reviewed by a single reference pathologist (M. F. Z.). Imaging
technical/plos/pmed.0020045.txt:94:          tubular immunostaining was evaluated semi-quantitatively by two independent pathologists
technical/plos/pmed.0020045.txt:192:          independent pathologists in a blinded manner, demonstrated that mean CD36 PTEC scores
technical/plos/pmed.0020060.txt:41:        begin at the autopsy table. Having removed Albert Einstein's brain, pathologist Thomas
```
- what it's doing and why it's useful
```
grep -n "Larry" technical/government/Alcohol_Problems/*.txt > bp-results.txt
cat bp-results.txt
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:251:Larry Gentilello asserted that effective treatments already
technical/government/Alcohol_Problems/Session4-PDF.txt:9:Larry M. Gentilello, MD
technical/government/Alcohol_Problems/Session4-PDF.txt:740:Response to Dr. Larry Gentilello's Presentation
technical/government/Alcohol_Problems/Session4-PDF.txt:1137:Jeffrey Runge agreed with Larry Gentilello that health
```
- what it's doing and why it's useful
