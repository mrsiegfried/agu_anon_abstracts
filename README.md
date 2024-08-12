# agu_anon_abstracts
Small piece of code to expedite anonymized review of abstracts for the AGU Fall Meeting<br>
Written by M. Siegfried, sometime in the late 2010s or early 2020s
siegfried@mines.edu

This is pretty straight forward: the notebook takes in what the AGU session convener website spits out (or at least used to!) and anonymizes the information so the co-conveners can review abstracts without knowledge of the author list. The AGU website (at least used to) download an `.xls` file, so you will have to open that file and re-save it as an `.xlsx` file before you get started. After you do that, open up the notebook, set what the input and output file names are/should be, then run it and it will save two files: 
1. `[out_name].xlsx`, which is an anonymized spreadsheet that only has abstract ID, presentation preference, whether it's invited, and the title. This file can be very quickly turned into a rubric to send to co-conveners (i.e., add whatever columns you want for review criteria)
2. `[out_name].txt`, which is formatted to be opened in MS Word (or similar). If you open it in Word it will place each anonymized abstract on its own page with the abstract ID, whether it is invited, whether it requested only poster, the title, and the abstract text. This can be exported as a PDF and sent around with the anonymized review spreadsheet, so abstracts can be reviewed by the co-conveners anonymously.


## Install and running
1. Clone repo into the folder you want `git clone https://github.com/mrsiegfried/agu_anon_abstracts.git`
2. Install environment: `conda env create -f environment.yml`
3. Activate environment: `conda activate agu_anon`
4. Install kernel into JupyterLab: `python -m ipykernel install --user --name agu_anon`
5. Launch JupyterLab (`jupyter lab`), edit the file name variables as needed, and run the cells

