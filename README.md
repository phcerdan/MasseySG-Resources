# MasseySG-Resources
Massey study group resources.

# Repositories
- Python scripts for processing Fasta Files: https://github.com/hulu1/seqIO_basics (Lukas)
- Document and Beamer templates with Massey Logos. https://github.com/hcalitz/MasseyLatexTemplates (Hannes)

  Please be encouraged to modify and improve the templates in your own fork, and place a link here for others to enjoy it.
# Tips and Tricks

## Search bash history with your arrow keys

Usually in `bash` the up and down arrows scroll through recently used commands. 
It is possible (and really useful) to modify this such that when type a few letters
of a command and push up-arrow you scroll through recent commands _that started 
with those letters_. Say you can't remember the paramters you used to create a 
`blast` search yesterday? Type `blastn` then tap up-arrow, you have the whole 
command you used. 

To get this behaviour your need  to create a file called `.inputrc` to your home 
directory with the following.

```
$include /etc/inputrc #location might be os-specific?

"\e[A":history-search-backward
"\e[B":history-search-forward
```

Now, when you start a new bash seesion "up arrow search" will be available. 
This will work on any program that uses `readline`, so you will get the same 
behaviour in interactive R sessipns and ipython consoles.
