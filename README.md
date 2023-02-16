# UNIX-EEOB-546-Assignment
This is for my assignment


UNIX Assignment
Data inspection
Attributes of fang_et_al_genotypes.txt data
here is my snippet of code used for data inspection of the Fang-et_al_genotypes.txt file.
$ wc fang_et_al_genotypes.txt
$ awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt
$ du -h fang_et_al_genotypes.txt
$ file fang_et_al_genotypes.txt
$ grep -v "^#" fang_et_al_genotypes.txt | cut -f3 | sort | uniq -c | sort -n

By inspecting this file I learned that:
1. This file has 2783 lines, 2744038 words, and 11051939 characters :($ wc fang_et_al_genotypes.txt)
2. The size of this file is 6.1M : ($ du -h fang_et_al_genotypes.txt)
3. There are 986 columns in this file : ($ awk -F "\t" '{print NF; exit}' fang_et_al_genotypes.txt)
4. ASCII text is used in encoding this file : (file fang_et_al_genotypes.txt)
5. For maize: There are 290 group of ZMMIL, 1256 group of ZMMLR, and 27 group of ZMMMR : ($ grep -v "^#" fang_et_al_genotypes.txt | cut -f3 | sort | uniq -c | sort -n)
6. For teosinite: There are 900 group of ZMPBA, 41 group of ZMPIL, and 34 group of ZMPJA 

Attributes of snp_position.txt data
here is my snippet of code used for data inspection of the Fang-et_al_genotypes.txt file.
$ wc snp_position.txt
$ awk -F "\t" '{print NF; exit}' snp_position.txt
$ du -h snp_position.txt
$ file snp_position.txt
$ grep -v "^#" snp_position.txt | cut -f3 | sort | uniq -c | sort -n

By inspecting this file I learned that:
1. This file has 984 lines, 13198 words, and 82763 characters :($ wc snp_position.txt)
2. The size of this file is 38k : ($ du -h snp_position.txt)
3. There are 15 columns in this file : ($ awk -F "\t" '{print NF; exit}' snp_position.txt)
4. ASCII text is used in encoding this file : (file snp_position.txt)
5. We have a total of 10 Chromosmes and greatest number of snps (155) is in chromosome 1 while the lowest numner of snps (53) appears in chromosome 10. There 6 snps in multiple locations and 27 snps are in an unknown locations: ($ grep -v "^#" snp_position.txt | cut -f3 | sort | uniq -c | sort -n)


Data processing
