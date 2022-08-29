# ldpc_ira_codes

The codes that outperform 5g NR codes for short frames in alist format for simulation with https://github.com/aff3ct simulator.
For details see Documentation folder.

## Logical structure
 Text in English and paper in Russian are in the Documentation folder.
 The code matrix is in the Alist folder.
 The simulator output is in the res folder.

## Dependencies: 

	 https://github.com/aff3ct
	 
## Usage

 1. Install  https://github.com/aff3ct simulator.
 2. Run one of the command strings below:
 
```bash
 aff3ct --sim-type BFER -C LDPC --src-type AZCW -K 172 -N 516 -m 0.00 -M 3.51 -s 0.5 -e 30 --dec-implem SPA -i 50 --dec-h-path ../path/to/dat172.alist > K172N516.txt
```

```bash
 aff3ct --sim-type BFER -C LDPC --src-type AZCW -K 72 -N 216 -m 1.50 -M 5.51 -s 0.5 -e 30 --dec-implem SPA -i 50 --dec-h-path ../conf/dec/LDPC/dat72.alist > K72N216.txt
```