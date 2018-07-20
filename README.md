
<p align="center">
<img src="img/trainmaltalogo.png" width="600">
</p>


# Introduction to Unix and R

- Date: 26th July 2018, 9am - 1pm (CET)
- Course: [TrainMalta](https://www.um.edu.mt/project/trainmalta) Summer School 2018: [Epigenomics](https://www.um.edu.mt/project/trainmalta/notices/summerschool2018epigenomics)
- Location: Informatics Lab, University of Malta
- Trainers:
  - Luigi Grassi, Department of Haematology, University of Cambridge (UK) Email: Luigi.grassi [at] bioresource.nihr.ac.uk
  - Daniel D'Andrea, Section of Inflammation and Signal Transduction, Imperial College London (UK) Email: d.dandrea [at] imperial.ac.uk
  - Sergio Martínez Cuesta, Department of Chemistry and CRUK-CI, University of Cambridge (UK) Email: sermarcue [at] gmail.com
- [Plan for today](https://www.um.edu.mt/__data/assets/pdf_file/0006/358098/TrainMalta_SummerSchool_Programme-final.pdf)
- [Etherpad](http://pad.software-carpentry.org/TrainMaltaSummerSchool2018)



## Introduction to Unix

(Based on materials from Luigi Grassi's Introduction to Unix and R, TrainMalta Summer School 2016)


### Outline

- The structure of Unix: files and directories
- Exploring the command line
- Unix tools
- Users and permissions
- Standard input/output, redirections, pipes
- Task control
- Environment variables and bashrc
- Text editor (nano)
- Compressing and archiving
- Locating files


### The structure of Unix: files and directories

Unix is made up of files and directories.

An example of a basic directory structure:

<p align="center">
<img src="img/structure-of-unix-1.png" width="500">
</p>

- `/`: root directory
- `/bin`: basic system commands
- `/data`: storage of datasets
- `/Users`: user directories. Who? imhotep, larry and nelle e.g. `/Users/imhotep`
- `/tmp`: storage of temporary files

Examples of files: `README`, `.bashrc` and `index.html`

- Case sensitive: `README` is a different file from `readme`
- No length limit
- Can contain any character except `\` (including whitespaces)

A path is a sequence of nested directories with a file or directory at the end, separated by the `/` character.

- Absolute path: `/Users/nelle/README`
- Relative path: `nelle/README` (with respect to the current directory `/Users`)



### Exploring the command line

What is the command line? The tool used to execute commands, also known as instructions that tell the computer what to do.

In different contexts, the command line is often called as the terminal, shell, bash, console ...

How does it look like? Open your command line as follows:

<p align="center">
<img src="img/exploring-the-command-line-1.png" width="400"> <img src="img/exploring-the-command-line-2.png" width="400">
</p>

- `$` indicates where you can start typing your commands

Type the command `pwd`, then press `Enter`. This command answers the question: where am I in the directory structure? `pwd` displays the current directory ("working directory").

Other useful basic commands are:

- `whoami`: who am I? what's my user name?
- `hostname`: what is the name of the machine that am I using now?

How can I move up and down in the directory structure? `cd <dir>` changes the current directory to <dir>.

```bash
$ ls       # list directory contents of pwd
$ ls -F    # list directory contents of pwd with an added slash (`/') immediately after each pathname that is a directory
$ ls -l    # provides additional info on files and directories
$ ls -la   # includes hidden files (.name) as well
$ ls -lat  # lists files in chronological order
$ ls -R    # lists subdirectories recursively
$ man ls   # manual on command ls

$ cd <dir_name> # changes/switches into specified directory
$ cd ..         # moves one directory up
$ cd ../../     # moves two directories up (and so on)
$ cd            # brings you to highest level of your home directory
```









## Introduction to R






## Additional materials

R:

- Sofware Carpentry: [Programming with R](http://swcarpentry.github.io/r-novice-inflammation/)
- Sofware Carpentry: [R for Reproducible Scientific Analysis](http://swcarpentry.github.io/r-novice-gapminder/)
- Data Carpentry: [Data analysis and visualization in R](https://datacarpentry.org/R-genomics/)
- Babraham: [Introduction to R](https://www.bioinformatics.babraham.ac.uk/training.html#rintro)

Unix:

- Sofware Carpentry: [The Unix Shell](http://swcarpentry.github.io/shell-novice/)
- Data Carpentry: [Introduction to the command line](https://datacarpentry.org/shell-genomics/)
- CRUK-CI Bioinformatics: [Introduction to the Shell](https://github.com/bioinformatics-core-shared-training/crukci-cluster-transition/blob/master/session1-shell.md)
- Babraham: [Introduction to Unix](https://www.bioinformatics.babraham.ac.uk/training.html#unix)
