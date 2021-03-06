# Tandem Repeats

This function will detect substring patterns of 4 letters ('A','C','G','T') when the letters repeat.

## Getting Started

### Prerequisites

You need **jQuery** to run two functions in `app/tandem.js`. 

If you want to test/demo this project only I provide the jQuery in `lib/jquery` folder. You don't need to install jQuery to run test.

[jQuery](https://jquery.com/download/)  This link will take you to download and install jQuery.

### Installation

Clone a copy git repo by running:

```
git clone git://github.com/theerapatkij/tandem-repeats.git
```

If you don't have git or don't want to use it, please download zip file then unzip to your computer.


## Run & Usage

First, open HTML file name `app/tandem-repeat.html` with your browser. 

Input string and then click the Submit button.

The result will display below in two forms. The string with highlight tandem repeat patterns and JSON.

## Output given test strings

First test string:
```
GTTCACATGAACTTTGTGCATTTCACGTCTAGGGAGGAGGAGCCCTCCTTGCGGCGGATCGTGATAATCGATACGACCCCGAATAGATCTCGCGTATCCCTG
```
Result of first test:
```
[
	{
		"32-GGA": 3,
		"43-CCT": 2,
		"50-GCG": 2
	}
]
```

Second test string:
```
CAATCGAACGGATCGAACAGTGAGCGGCTCTCAACAGCCGGAGTTGGGCTTACCGAAATGCTGGGCGTGCGTTGTGCTGCGGCAATTCTACCCTAAATTTTTTTACCTGGCAAAGTCTACCCTCAGGCTCGCATTTCATGTACGGCTTCTCAGGTTTATTGCTTCCTTGAACACTTTAGGCTCATGGAAGCTGAACCAGCACCCTCGGCACCCAGGCCTCGCCCTGGTGCGTAGACCACTTGCACTTGCACTTGCACTTGCACTTGCACTTGCACCGGTGTTCGTAGGCTTCGTATGCGAACCATTACCCACCTCTCAGTTCAGGCCAACAAAAACATCGGCGGATCGTCGATAACCGGTTGGGGCCTATGCGATAACAATTTCAGCGGCTGCCGGGCTAGTCCATTTCAACAGAAGCAATCCTCAGCAGGTGAATGTCAGTAATACCTTGATGCTCGATGGTGCACTCAGTCACTCCTATTCTACCCGACGAGAATGAGTGATCTCTTTAAGGAGGACAAGTTCGGACGCAAGGGGGCGACTTCAAAACGGGACCACTTTCATATGGATATCGCTATCCTCACAGAAGACGTAAGGCTGTTTGAGTAGCCAGCAAATCGTCCAGATTAGAGAGTTCGGACAAGAACATGAATCTAATGCCACTAACCCTCCGCCGGCTTGTAACTAGAATAGGTTTCCCGATGAATCTAACTCACCGACATTCGAACATGATACGCTGACCCAGCCTGGATCTCGCTACGGCAGTGACTTGTCGCCAGTTCCCCGGGGGCGGTCACTGGCGGGGGTCCGTGGACGAGGCCTCTATCTCACTTACTAAAGAGTTCACAACGATCTTAGATGAGTCAGGCGGCACCCCGCGATGGCTGGTGTATGCGACAGTAGAGCCCGTGCGCGGGCGCATTGTTAGCGGGCACGTGTTTCCCTGCGAAGATTTTGGACTAAATCTTGGGTGCACTCGCCGGGCATCCGTGTCTATTTACTACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACACTGGTAACTTGGACACGTGCTGACACC
```
Result of second test:
```
[
	{
		"64-GCGT": 2,
		"74-TGC": 2,
		"97-TTT": 2,
		"236-CACTTG": 6,
		"326-CAA": 2,
		"338-CGG": 2,
		"345-TCG": 2,
		"424-CAG": 2,
		"487-CGA": 2,
		"511-AGG": 2,
		"584-AGA": 2,
		"670-CCG": 2,
		"866-GGC": 2,
		"998-TAC": 2,
		"1004-TGGTAACAC": 11
	}
]
```

Third test string:
```
AAGCTGTCCCAGCGCCCTGACATTTGCTTCGAGAGATCTGGGGAGGTGCGACGACTCAGAGCGATCCAATGAGCGAAGGCGCGGCGAGATTGAACTACTAAAGTATTATACAAGACGCCCAAGTCAAGATACCGTGTGTGCGTAGCTTTAAATGGGAACATCACTTGCTCGATATTAATAGTAAATGCTGTCTACTTCATATCATATCGAGCTACAGTATGATTCTGCTCCGTTTCCCTGACCCAGAAGGGACTGGCCCCGCATGTAGCGTGGATACTTACAGGTCAATAGTCCAGCTTACACATGTGACTGGTATTTGAAAGCAGATCTGCATGTATGGAGACAGTAGCCCTCGTCGGACTACTTTGTTCCCTCAACACGGATCACAAACGGCTGGATCATCCTACAGTGATTCTAGCTGCTGCGGACTTCCGTATAAGGAAGCCTAGTCTCGGGGCATAAGATGGACGACCTCTGGGCCCGAGCGGAGCCCGCTTTTGACTGACCTTGTGCCAGGAAGTCGCGTACAAGCCGCTATTTTTACAGTCAACTGGGCGATCGTACTTGCAGGGGATATACACGCACGTCCTCATAGTATGTAAACACACGGTTGATACCCCTGTTGGCTGCTTAGCAGGATTCCTTACATTATTAGACTCAGCCCTCTGCCAGCTTGAGTAAAATGAAGGATACGTGCACGGACAATTGACCTCTCCCCGACTTACCAGAATATTGCTTGGTTGTCGCCATTCATTCACATGTTTCCAGAGCAATTTAACCCTGATGCCTTATAACAGTTGGTGATGCTCTCACATAGCGTATAGGGCCCGATTCGTCCTGGGCGAACCCCCCCTAGAAGCCACAGCGATGACGGCGATCACTACCTTTTGACCAGACAAACCTACTCCAGCGGACGATGACAGCTGCCAGTATATCCCTCGGTTTTAACGTATTCCTGGTTTATATCGTTGCATGAATGCCGGTCCTCATAGATTATCCGTGCGAACAAAGTCAGGCTGGGTTGACGGGAGGGAAGATGCCAGTTGGGAGCCGCCATGAAGCTACTCTGCGTGCTAGATAAAGCGAGCCCCTTGCTACCGCATATGAATAACATGCGATAAGTCTATGTTGCCACAAGGGGGGTAGAGCACGGAATGGGCGCCAATGACCTGTTCTTTAGCTGTGTCTCGCTGGAATTCCTCGCATGACCCCTTTCAGGCCTTTCACTCTGTCGCGAAAACTGCGCCGATAGGCCAGTATCCCACGAAGTCAAAACGGATCAAGAAGTATACGCGAGCTCTGTGCGGCTCGAGTTGTTCCGAAGTAGCGCCTTAGGCGAACAGCGAATAATGTCTTCGTAGCATAAGCGGCCCCGCATGTAGGCCGTTTATAAGCGTATACACCAGGCAACGTGAAGAACGCATGGCCTTCTAGTGGACCAATTGACTGCTTGGGGTCACACATCTTTTACCGCCTACGGGTCCCATGCGTCATGGGCCCAGTGACATAAGGACCTGAACACTGAGTCGGCACGTAACCGCAGGAGTAATTCTTGCTACGCAGGCGACGGGGAGAGCAGGTACATCACGCTTACGAGTGACGTCGCTAAGTATGCATAGTAAACTTCCACGTCCCTTTGTCGGAGGTGGCGAGGTTTATGCCTAGCCTCGTAGTCCCTAGGACTCCCTAGCCCGCTAATGTGAGTCACTAGTGATGGGGTTCACAGCTTCCGCGACAGAAAACCTAGCGTAAGCCAACCCAGCAAAGATGTTGACCATGACGCACGGATTATGGTGATAGAAGCCTGTAATACGACTGTGCTATGTGTTCTGCCGAGTAAGTGAAGTTAGAGGCGCTGGTGAATCAGACCTATTAGTCCCCAGTGGACGATCACATCGGAAGCACTACATGTCATGGCCTTCGGGCGCGCTTACACTTATACTCCCGATTTCAAGTAACAATAGTCTAGCGTCCGCGAGCAGTGATAGAGAGTTGCCATGGAGAACCAATTATGAAACCAGATTATACCCACCGGGCGCAGTGAAAGGGATTCACATAATGAGACGGCCACATGTCGCAACTATATAGCCCCCCGTAACGGGCCTATGCCGGAACCGAGTTGATTCAACAGGCCGCTAACTATTTGACCATGAGAATGGAGTCTTGGGTCGTCGATGCCGCAAAGCGAACATTTCCGGAGGCATCTCCCGACCTTTCACTTCTGCAGATGGTGGTCTGGACAACAGCACACCAATCTCAAGCGACTTCCTATCAGCCGACGAGCCCCGTGAGCCTTTGTGAGCCCTACTTGCCGTCACGCCCAGCAACTAGTACATATTTTTCCCCGCGCCCTAAAATTTTGCGTATCGCCCATCCACTCCCCGGTGGGCCAACCATCGCAAACGTGCCAATGGAATCGGCGCTGGCCATTTGACGACATGTGCAACCCACGGACCTGATAACGGGACCACCAAAAGGTTTGTTCCTTCTGTACCATGCCGTAGCGAATCACTTCTGGCGTCCTAACTATATGGAGTAGCAGTCTACGCGGGCCACTGTGGGTCACCTGGGGATAATTCAGGGAGCCGTGAAGTGTCTCAAACGAGTCAATTAATAAGCTACTTCTAATCCACAAAACCGGGAACCCCATGCTCTCAGCCTGGTTGACCGTTTTTCTGGCTAGGGGGTTTCGAGCTACATCTTGGACCGCCGAGGTCTCATACCTTGTGCGGGGTCGCATGAAGTGTGACCAATCAGTGGGATCCACGATCGGGCAACAGTCATCATCGTTTGACACGCGACAACTGATTACTCCTACGACCTGCTGGACAGCGGTGGGTACACCTTCCTAACGGACGTATGCCGGTAAGTTGTAGCACTTTGACGAGATCTATCCCTTCGAGAGGTGTTTGACCCCGTCGACTTGGAGTGTTGACGCGAGGCCTTACTACGTACAGCCTAGCGTTCCATTATACGCCCCGAAGATGCCGAGCTGATGCGAAACGGGAAAAGGGCATTGCGGACGCCGAGTTGCCCTACTAAATTAGACAAATGGCGCCATACTTGGTTATAACTACGCAGCAAAATCACTACTTGTGTTAGAACCAATAGATGAGGGTCAAATCTCCTGTGGCAATAGCCACGCATCAAACATATTACCTAACGGCAGGTACCGAAGCTGCATTGATACCCACCCTATCAGTAACGGTCTGTGAAGGACCCTACCTAGCTCCAATGACATGCGGGATTAGAGCGAACATCCAGTGATAATTTGTAGTCTTGTTCTGGTAAGAGTCCCATTCGGTTTCCACGCCCGGGGGCTTCTCTCTTCGACAGGAGTTGGCGTGACCGCTACTCCACCATTCTCCTCAGCACAGAGGGGATTCCGGGCTCATAATAGGACGAATAGGAACAGGAGCGTTGACTGCTGTTATTCGACTTCCTGAAAGAAGAGTACTCCGTTTTGCATCAGCGACGAGTTTTTCGCTTACTTAGGGGCATAGACGCGTGTTCATTTATGGCGAAACTATGTATAAGCGGAGAGCCTCATAGAACATCTGGAGCGGCACTCTGAAATAAAAGGTATATATACTGCAGAGCAGCGATGGGTGCCATAAGGATTCGTCATATACCAACACTGGACAAAATCGGCGGTTTCGGTTTAGTCTAACTCACGCCACGAATATCAAAGACTATTGGTAACCCGAGTACCGGTCGGTTCGTTGCTGTACTTCTACCTGGTGCAACTCGAACCCGGCGCTGTGTAAAACTTGGCAATCTGCAAAAGTAAAGGCTAACTTTAGTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTTACTCTCTCCTAACGTCGAGTACACGTAGCGTATCAGTGCTCCGAAGCCTGGTGAGGTTGCGAATCTTACGCTCTTACAGGCCCTTGACGATCTCCATGCAACAATGCAAGGACCAGCCTCGGCTAGCGGGCTTAGTGGGTACACTCGATACCGCTGAGCCGCCCGCCTCTTCTCATGAGACACGTCGCCTGTACATACAAAACTAGCGTTGCGTCCAGCGCGCATCCCAAGTTTCAACGGCGACATCTGTTAGGTTGCAGCCACTTTGCGAGCCTGTTAGACGCTGTTATTAACGGAGGCAGACCCGTCCACAAAGTGAAGTTGCTGGGCGTCCCTCTACGAACATCACTGGGTGTCACTTGGCACCACAAGACGCTCACTTGTCGTTACTGGTCAGCTTATATCGACTGCACACATCTCACACGGACATCGATCGCAGTACATTACAATGGCGGAGGCTGCCTGTTGTTTGGCTACCGTGGACAAAGTACAAGTAGGATGGTCCTGCAGTACCTAATACACCGTCTTCACTGCGAAAAACTGCTACCAGCGATATATGTTCCGTATTGCAGGGGATTGTATAGCGTGCACGCTCCATGTGCCCACATCGAAATATAGAGCTACGTTGTGATCCGAGTCGCCCACGCACGGATAGCCGTCTACTCTTTCTCTTTAAGTTTTCGTAAGCCGCCCTCCGTATGCAACTTGGGCGACCGTCACTCGGCAGGGCAGGCTTCGGATGTCGGCTTACCACCAAGTACACACAGTGATTTATTAGAGGGAGGGGAGTTGACGTAAGACATCGCCGCGGAAAACTTCCAGATGAATAGCAAGGGTAGCTAACAGGCGGGGGCGTTTACCCTACCCGACGACGGCCTCATCGGCGCGAGGAAAGGGAATAGGACTAGGTAGTAACCACGCCGAGCGCTCTCGTCGGTGGTTGTAACGGCCGAAAAACCGCCTCGGAGAGGGCAAAAAATGCGCTTAGCCAAAAAGGTCTTGGAGCGTACTCCTCGATACCGTCTCCCCAAATAGGCGAATTACCTAGAATGTACCGAGAAGTCGCTGGTTAGCCCAGTTTCTACCCGTACTTAGGTCGACACGCTACTTTGCCGACGGCCAGCTTTTACCAACTTCCGGGGGGATCTAGGCCGGAAGGACATTAAAAACTCGTTCTGGCTACGAGACAGCGTGCTACGGACGGGACGGGACGGGACGGGACGTTGTGGGGCGAGCTATCGCTGCGACCAACAATGCCAATCGTTCTTAGCAATCCCTAGACGCTGCCTATGGTCTCGTCCGTCGGCTGGCCTAGTGGTTTGACCTGAAAAAACACGCCGTTCCCGTCTTCGGCTTCGGCCTCGAATTGGGCATCGACACGTGCCACAGTGGCTGCACGCGTGCACTAGGAAACATGCAAAGCTGACATAGAGACACGTTTTCCACATACGGCGGTCTGCGTTCTAATTGGTCGGAGATCAGCGGTATTCCGACTTACGCCAATAGATCCCATATTTCCAGGGATCATAGTATTTTGTTCGCCGCGGTAGTACGTTCGGCCGAAACTCTATATTTGCCACTCTGAATCACACGGCGAACCCCCTTATCCATTATTTCACGTTGGCCATGCGCATACTGCCGGTCCGGCTTGATTCTGGAAATTAGTGGATCATCACTACTGCTGCCGCGACCAAATAGCAAGGCGACTATCTGGCCTATTTCGTTTTTGGCCGCTGCCTATTGATAAGTGCTAGAGGCTGCGACCGGATGCAAGCTGAGTGTAGAGAGGGTTTAAGACAGACAAGTTAATTCATCTGGAGGTCGAGGTCGTGCGACTCTGCTACACCGCTCCTACTTTACGCGGAACGAGGCAAGAACTAAAGTTGACTTCAACGAACTCTCACCGCCGTTCGGACGACCTATACCTAGCTAGATCAACCGGTTAATGTAGTTGCTACCCTCGACGCCACGCTCCCCTTGTCAATACCACTCACCGGAGAACGTTACGACGGAGAAATAGAGCGGCAGAAAGCCAACTACTGTTTATACACCAAGGCCTGTTCCCAGATCCAAGGTGTACAGATGTGTACAGATGTGTACAGATGTGTACAGATGTGTACAGATGTGTACAGATGGGATCAGTGGTAAGCCTAGAGGTTCAGTGGTGATTGAAACGGGAAACGCATGACCGCACAGTTTTCGTGCTTCCCCGTACTAAAAGAGGTGACAGCGGATATTAATTAGAACTTTGCCATCGTTAGAAACTGGTCTATTCTTCTCTAGGCTCGTCCCAGGACATACCGGACCCCCTGCTATCCAGCGATTAGCAGTATCAGCCTCCAACTACGGTGAGAATTTGGAGTCGTATATGTATAACACCGTACGCCACAGGACATGATGTAAACCATCGTTTACTCACGGATCCCGAACCCTAATCTCTGACTTATGCGACTGCCGATATCCACTACGCAGAATCTAAACATCCTGTAGTGTCAGTGTTTGAACAATTATGAATGTCTAGTATATACCTCAGCTTTTAGTTAATAAGTATAGAAATGAAGGAGTCCTCACGCCCGATATATGCCAGCTTGCCAAACACGCACGATCCGTCTGGCTGTCCGGAAATTTTTGATTTGAAACATTATGCAGTGGATTCTGGCTCATGTTGAGGGAGACCCAGATGTCACGCTTCGTCTCAAGCACTGTATAGATGTCACGCTTCGTCTCAAGCACTGTATAGATGTCACGCTTCGTCTCAAGCACTGTATTTCTTAGACTCTCGTCGCACCTGTGTAGAATGGAGGGGATCACTGCCCGATAGTAGAACTAGTAGAGCTGGGTATTGCGCCAATGGACTGGACGCTGTCTTTAGACTTTCTATGAGGGAGCTTCCGTTTTCATTTTCTTAAAGCACGGCTACTACGCCGCCCTCTCTAATGGAAAAGGTTCACTGCTGCGTATACCAGGAGTCGGCCGTTGCGGTCTATTTCAACATCTAGTCCTTGCACCCTTTTTGATCAGGTTACCCCCGCGGGAGTTAATGAAGTGACCGGAACCACACGCCACCAAACCACCCGGGGATTTCTTATCCTTGGGATCATAACATTGCTTAGAGAAGCACTTTCATAAGGTTGTGAATGTTAAGCCGGGACGCAAATCTGCTTTTGGGCTGCGCAATAAGCAGTTGGTAATTGTGATATACCGGCGTGGGTTCCGCAGAGTGAGGATCCCGATAAGGGAGAACTTTACTAACAGGGTCCTGGATACGACGCGTCAAGATCGCGCGTGGCCCCGATTGAAGACAAAAGCACTGTACTAGCGAATGTTCCCAACGCCTACTACACAAGAATCAAGCAGGATCACATCGGCAGTTGTGAATATCGAACGATCAACACTTGTTTACGAGCAAGAGCGCAAAGCACAAGACCTATTCGGAATGAGAACATTCGTCTATGGCATCCAGGGTCGCCGATTCGGATTCTCGCCACTTATTACTACTCCTCGGTCGATTATCGCACGGGGTGCGTCCTGGACAATTATATAATTCCTTTGGGCCATAATTCGACCGTGTGGGCTAGAACCTCCGTATTTTAATCTTGTAATCCAGGATTGGCTGGACAATCAGCTGACATAGCGAGTAGGCGTCCTTCCTGTATGGTCGTACCTTTGCAACCTTAGGAGGGTGAAGGTTCGCCTGAATGGTCAGCTATTTAGCTCCTTGCTAAAGCATAATATTTCGGTCAGCCTCTGAGGGTACTTTTGATTTGAAATTACTTTGAGGCGTCTCCGGGGCTAAACCCGTTGGGGGACCGGGAGCCCGCACACAGGGCGTGGTGGCACTTGCACCGAGCTCTGTTCCTTAGATCCATAAATCATCAAGTGTTTGATATTCAACTTAGTCGAGTCCCTACCTATTCATACCTGTCACTGTCCTCCTGTAACTAAGGTACCTGGGAGTTGGATATCAGGGTCATTACATGCGAGGGCCCATTCCCAGTCCGCTGAGCGAATCAGATACGAATACTGTTGCCTGTTTCGGCGGAGGACCCCTTCACATGTGCAGAGAGCGCTCTTACACGGGACGCAGGGTGGTTTACTGTCGAGTGCGTATCACCAGGCGTGGCGCAACGAGTGCACTCCAGCAAAGGAACCGCTGAGTTTCGCTCACTCTCTATAATTACTACACTTTCACACCCGTCAGATGGCCAGGCCCCTGTTCCAATTCTATTGTAGACCTTCCGCTGCGGTATATCATAGCAGTCAACGATTTATTCAACCAGTGAGAATTGTTGGTTTACAGACAGTCGAAGTTTGTGGACGCTCCTTAGAGTTACATGGTGTACTCCCTACAGAGTCTAGGAAAGTCCCGATGACAGAACCATCTCGGACGACGTGCTCGTTAGTCTAAAAACTAATGTACTGTCTAAACAGAGACTGATGAATCGCACCTACGGGGTATCGTAATCACGCGGCTATCCCCGGTGCATATTATCGCGATTAGTGCCCCTAGGGTCATAGCGTATGGTATTTTGAGGTCACATCCTTAGATTCGAAACTAGAGAGGTCCATAGGACCCCGGCATCGTTATAGCGCAACATTCTCGCACCCGAGCATATTCACGTACGACTTCGTTTGCCCTGTCGAGACAACTAACTTCGCGTAATTTGCTAGCTACTAGTAAAGTAAACAAGGTCGTAACGGTTAGGTAACGGTTTAAAAAACGACTATAATTCAACTTTCTGGCTAGGAGCTGTCTGGTTCCCTTAATGGGACCTAGATGTAGTGGCTATATAGTGCGCTGGGTTGAGCACCAGTCTGTATTGTCGGTGAAAATGACGCCATCAACTAAACTATACTGAATGGGTCAAAAAAGTGTGTATTTGCTATCCTCAAAACTAAGCGCTACTGTAACTCCAATCCCGAAGCGAGTACGGTTCTGTGAAATCTTAATATCAGCTTGTATTGTATCTCGGTAGTAAGATAAAACGAAAAGACTTCTATGAAAAGTACCGCAAGAGGATTCCTCAATACTTAGTCGGCGTTGACACTTTGCTACTTTCGTCTTCATAAATATTGTAGAACTCCACGTCTGGCGAACCACGATGGCTGCGTTAGATCTATAAGTCTGGAAATCGGAAAAATTCTATCGCTAAGATCTAGTATCGGTGCGGGTACGTGCAGTTTGACAACCCGATGTTCTTTAATACATGCACCTGCATGCTGAAACGGCTACCCATGGCGAGTTCGAACGCCCCTCAGTAGTAGCCACACAGAGCACTCCCCTTGAGATAAAATTAACCTGCTGTCCGTTGTTAACCTTTCACTTAGTAAATCGACTGACGAGATCACAACCATTCAAACTCCCCGCCCGGAGACCAGCCACAATCGGGTTAATACATACTGGGCTATACAATGTAAGTGAACGGATGTCTTTTCTCAAGCACGATCAGCTTTAGTAATGTCGTGTAGTGATAATGCTCAAGGAACCGATCGACTAGTCGGAAATCGGACGGTGGAAATCTGGTTGGGTCAGTCGATCTCCACCCATTTTCAATTTCACTCCCAAGCACACACCCCTTGGCCTCCAATTTATTTGAACGGCGTGGCGGCTTAGCGCCCCCCCCGAACAGCGTACATAATTAGAACCATAATTGCGCCGCCTTAAACGAGGGCTTACGATCGCAGCGAACGTTACTTCCATAACCCACCTATAACGCATTAAGCACCATCCTCAGCCTGCCCGACTATCATCTGCCATCCAGGAAAGTTTGGGAACCTCTAGCTGACTCGCTCGGCCCCTTCCTTCATTGAGTGAAACCTACTACAGCAGCGTGGGTTTAGAGTATGAAGACCTGCGGACTGAGGTGAGAAGGAGTGACGGTCACCTCAAGTCCTCGTACGCTCATGCGCACGTGATTCCTACCGAACCAGTTACCAAACGTAATCACCTACACTCCTTGCCATTCTTGATTTCAAATTTAACCCTTGGCGGATCGGGAAACCCTGGTATACTCGCAAACTTGCCGAAGCGGAGGGCGATTTGTTCAACTTGTATCGCCCATTCATATATTCAGCTTACGTGCACCTCCATGGGGTCTGCGTTTGCCAGAAACATGTTTAATGTCAAAGACCGTCTAGCGGCACTGATCTATCTGCAAAAAGTTTCAGCACACGCCGGGGAATGCAGATTTCACCTGATATCGTCACAGCGGCTTTAACACTTTATCGTATTATAACGTATCTAACAACACCTAATGTAGCCTGGCGGCCGAGGCCGGAGTGCGATCTGTATTAAAATGCTCCCTACTTCGCCACACGCCCGAGACGCAGCGAGTC 
```
Result of third test:
```
[
	{
		"48-CGA": 2,
		"80-GCG": 2,
		"93-ACT": 2,
		"103-TAT": 2,
		"196-TCATA": 2,
		"352-TCG": 2,
		"359-ACT": 2,
		"397-ATC": 2,
		"417-GCT": 2,
		"466-GAC": 2,
		"498-TGAC": 2,
		"578-CACG": 2,
		"625-GCT": 2,
		"647-ATT": 2,
		"747-CATT": 2,
		"846-CCC": 2,
		"1026-GGGA": 2,
		"1049-GCC": 2,
		"1137-GGG": 2,
		"1281-AAG": 2,
		"1312-GTT": 2,
		"1345-AAT": 2,
		"1413-GAA": 2,
		"2088-CCC": 2,
		"2167-GTC": 2,
		"2228-TGG": 2,
		"2239-ACA": 2,
		"2276-CGA": 2,
		"2432-GAC": 2,
		"2466-ACC": 2,
		"2611-TAA": 2,
		"2706-CCG": 2,
		"2780-TCA": 2,
		"2821-CTG": 2,
		"2945-TAC": 2,
		"3035-CTA": 2,
		"3077-GCA": 2,
		"3088-ACT": 2,
		"3188-ACCC": 2,
		"3220-CCTA": 2,
		"3356-CCA": 2,
		"3364-CTC": 2,
		"3393-ATA": 2,
		"3424-CTG": 2,
		"3446-AAG": 2,
		"3472-CGA": 2,
		"3486-CTTA": 2,
		"3583-TATA": 2,
		"3597-AGC": 2,
		"3648-CGG": 2,
		"3711-CGGT": 2,
		"3803-TACTCT": 18,
		"4004-CAA": 2,
		"4063-GCC": 2,
		"4073-TCT": 2,
		"4097-TACA": 2,
		"4192-TTA": 2,
		"4269-CAC": 2,
		"4334-ATCG": 2,
		"4369-TGT": 2,
		"4548-CACG": 2,
		"4568-CTCTTT": 2,
		"4592-GCC": 2,
		"4628-GGCAG": 2,
		"4655-ACC": 2,
		"4677-TTA": 2,
		"4683-GAGG": 2,
		"4709-CGC": 2,
		"4763-TACCC": 2,
		"4773-GAC": 2,
		"4814-GTA": 2,
		"4836-TCG": 2,
		"4879-AAA": 2,
		"4915-CTC": 2,
		"5044-GGG": 2,
		"5102-ACGG": 2,
		"5110-GACGG": 3,
		"5154-CAA": 2,
		"5202-CGTC": 2,
		"5233-AAA": 2,
		"5253-CTTCGG": 2,
		"5355-CGG": 2,
		"5445-CGC": 2,
		"5452-GTA": 2,
		"5515-ATT": 2,
		"5574-ATC": 2,
		"5580-ACT": 2,
		"5700-AGAC": 2,
		"5723-GAGGTC": 2,
		"5809-CCG": 2,
		"5819-GAC": 2,
		"5831-CTAG": 2,
		"5911-ACG": 2,
		"5941-ACT": 2,
		"5980-GTGTACAGAT": 6,
		"6067-GTG": 2,
		"6141-ATTA": 2,
		"6178-TTC": 2,
		"6300-ATG": 2,
		"6447-TAA": 2,
		"6502-CACG": 2,
		"6533-TTTGA": 2,
		"6685-TCG": 2,
		"6724-TAG": 2,
		"6733-TAG": 2,
		"6757-TGGAC": 2,
		"6822-CTA": 2,
		"6828-CGC": 2,
		"6856-CTG": 2,
		"6968-CCA": 2,
		"6975-ACC": 2,
		"7171-ACG": 2,
		"7241-CTA": 2,
		"7394-TTA": 2,
		"7403-CTC": 2,
		"7550-TCCT": 2,
		"7582-AGG": 2,
		"7634-ATA": 2,
		"7664-TTTGA": 2,
		"7736-GTG": 2,
		"7777-ATC": 2,
		"7812-CCTA": 2,
		"7836-TCC": 2,
		"7942-CGG": 2,
		"7993-GGT": 2,
		"8084-TAC": 2,
		"8192-TTG": 2,
		"8202-ACAG": 2,
		"8292-GAC": 2,
		"8341-TGA": 2,
		"8392-TAT": 2,
		"8553-AACT": 2,
		"8572-GCTA": 2,
		"8582-AGTAA": 2,
		"8621-AAA": 2,
		"8749-AACTA": 2,
		"8772-AAA": 2,
		"8863-TTGTA": 2,
		"8878-GTA": 2,
		"9163-AGT": 2,
		"9205-CTG": 2,
		"9214-GTT": 2,
		"9269-CCCG": 2,
		"9299-ATAC": 2,
		"9493-ATTT": 2,
		"9510-GGC": 2,
		"9522-CCC": 2,
		"9560-CGC": 2,
		"9652-ATC": 2,
		"9692-CTCG": 2,
		"9703-CCTT": 2,
		"9724-CTA": 2,
		"9730-CAG": 2,
		"10052-ATCT": 2,
		"10134-TAT": 2,
		"10149-AAC": 2,
		"10169-GGC": 2
	}
]
```

## Tests

I wrote an automated tests with [Mocha](https://mochajs.org/) on HTML file. You can run by follow below instruction.

### Run test
Open file `tests/tandem-test.html` in browser. You will see a functions name and lists of the test case.

If you want to edit Test cases. Just open `tests/tandem.test.js`.


## Choices, limitations and algorithm performance

Tandem repeat function that I developed will catch every substring that include 4 letters 'A', 'C', 'G', 'T' with repeat pattern in range 3-10 letters.

I choose javascript in HTML file for this work because javascript function on HTML is easy run and test. For whom that I don't know their environment I also choose **Regular expressions** in my code less complex and easy to maintain. 

Maybe other algorithm such as **while loop** with **String operations** is faster than Regular expressions. But If a problem grow bigger, very complex or you need to change something. You have to spend more time to refactoring it.
Although Regular expressions are complicated but I think it is reasonable to use. 
