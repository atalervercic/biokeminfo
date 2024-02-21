# Python

[Python](https://www.python.org/) je popularen programski jezik in je nameščen že kot del nekateri operacijskih sistemov (macOS, nekatere distribucije Linux) oz. ga je tam izredno preprosto namestiti, na voljo pa je tudi za okolje Windows. Aktualna verzija je 3 (t.j. Python 3.x), na nekaterih starejših sistemih lahko naletimo še na prejšnjo verzijo (2.x). Načeloma programi, napisani v Python 2, delujejo tudi v verziji 3, je pa vsekakor priporočljivo, da uporabljate najnovejšo verzijo, sploh zaradi združljivosti z novejšimi paketi.

## Namestitev
Ko namestimo Python gre pravzaprav za namestitev prevajalnika, to pa lahko storimo na več načinov, med drugim:
* namestimo osnovni paket z uradne strani [Python](https://www.python.org/),
* namestimo distribucijo [Anaconda](https://anaconda.org), ki vsebuje Python in kopico drugih paketov.

### Namestitev prek osnovnega paketa
Z [uradne spletne strani](https://www.python.org/downloads/) si prenesite zadnjo verzijo namestitvenega programa za vaš operacijski sistem in ga zaženite.

JupyterLab (ter druge pakete, npr. BioPython) namestite z uporabo upravljalnika paketov `pip`. Na primer, BioPython namestite tako: `pip install biopython`. Kratka navodila za JupyterLab, vključno z namestitvijo, so [tukaj](jupyterlab.ipynb).

### Namestitev v okviru Anaconde
Z [uradne spletne strani](https://anaconda.org/) prenesite namestitveni paket ([povezava](https://www.anaconda.com/products/individual) za vaš operacijski sistem in zaženite namestitev.

Anaconda pride s svojim upravljalnikom paketom `conda`, ki ga lahko poganjate v lupini (terminalu), lahko pa uporabite tudi grafični vmesnik znotraj Anaconda Navigatorja. Prek tega sistema je dostopnih veliko paketov, ne pa vsi. Priporočljivo je, da pakete najprej poiščete in poizkusite namestiti z uporabo ```conda```, tudi JupyterLab ([navodila](jupyterlab.ipynb)). Če nekega paketa ni na voljo, pa z uporabo `conda` namestite `pip` (ukaz: `conda install pip`), nato pa s `pip` namestite željen paket.

## Virtualno okolje
Priporočljivo je, da si razne programe, ki jih morda potrebujete samo za test, nameščate v virtualno okolje (*virtual environment*) in si z njimi ter morebitnimi dodatno potrebnimi programi/knjižnicami, od katerih so prvi odvisni (t.i. *dependencies*), ne smetite osnovne instalacije Pythona:
* navodila za virualno okolje prek [Anaconde](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html);
* navodila za virtualno okolje prek [pip](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).

Če želite uporabljati obstoječo instalacijo JupyterLab v okviru Anaconde je morda najbolj smiselno, da si naredite virtualno okolje v Anaconda, nato pa znotraj njega nainstalirate pip (```conda install pip```) ter potrebne ostale pakete.

### Uporaba v Binderju
Če se želimo izogniti spreminjanju naše lokalne instalacije Pythona, prav tako pa ne želimo ustvarjati lokalnih virtualnih orodij, lahko nekatere pakete uporabljamo tudi prek JupyterLaba v Binderju in sicer si jih namestimo z uporabo ```pip```. Na primer, namestitev PyMed v virtualnem okolju v Binderju dosežemo tako:
```
!pip install pymed
```

Ko jedro v Binderju ugasnemo, se virtualno okolje pobriše. **Pozor, ko okno brskalnika, v katerem interagiramo z Binderjem, zapremo, se pobrišejo tudi naše spremembe datotek!**

## Tečaji Pythona

Na spletu je brezplačno dostopnih veliko tečajev Pythona, prek katerih se lahko naučite osnov programiranja v tem jeziku ali pa zgolj obnovite svoje znanje. Tukaj je navedenih zgolj nekaj:
* [Python Village](http://rosalind.info/problems/list-view/?location=python-village) na portalu Rosalind
* [How to Think Like a Computer Scientist](http://openbookproject.net/thinkcs/python/english3e/) (Learning with Python 3)
* [Learn Python](https://www.learnpython.org/)
* [Python for Absolute Beginners](https://www.udemy.com/course/free-python/?LSNPUBID=JVFxdTr9V80&ranEAID=JVFxdTr9V80&ranMID=39197&ranSiteID=JVFxdTr9V80-DTy5bPmtnIIYmHBmoUs_Qw&utm_medium=udemyads&utm_source=aff-campaign) na portalu Udemy
* [Python for Total Beginners](https://www.udemy.com/course/python-3-for-total-beginners/?LSNPUBID=JVFxdTr9V80&ranEAID=JVFxdTr9V80&ranMID=39197&ranSiteID=JVFxdTr9V80-.KxFZERGV5HVjrqvHOnOTQ&utm_medium=udemyads&utm_source=aff-campaign) na portalu Udemy
* [Scientific Computing](http://disi.unitn.it/~teso/courses/sciprog/index.html) - spletna stran, kjer najdete nekaj osnov i Pythona in BioPythona


Obširen seznam tečajev najdete tudi na uradni [wiki-strani Python](https://wiki.python.org/moin/BeginnersGuide/Programmers).
