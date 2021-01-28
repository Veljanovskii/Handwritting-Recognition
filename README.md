

## Pokretanje projekta 
[Preuzeti model datoteku](https://www.dropbox.com/s/lod3gabgtuj0zzn/model.zip?dl=1) koja je obučena na IAM skup podataka.
Sadržaj preuzete datoteke `model.zip` smestiti u `model` direktorijum ovog repozitorijuma.
Nakon toga, otići u `src` direktorijum i pokrenuti program komandom `python main.py`.


## Obuka modela

### Za IAM skup podataka

Pratiti sledeće instrukcije:

* Registrujte se na ovaj [sajt](http://www.fki.inf.unibe.ch/databases/iam-handwriting-database)
* Preuzeti `words/words.tgz`
* Preuzeti `ascii/words.txt`
* Kreirati direktorijum za skup podataka na disku, a u njemu dva poddirektorijuma: `img` i `gt`
* Staviti `words.txt` u `gt` direktorijum
* Staviti sadržaj direktorijuma `words.tgz`(`a01`, `a02`, ...) u `img` direktorijum

### Pokretanje obuke

* Obrisati datoteke iz `model` direktorijuma
* Otići do `src` direktorijuma i izvršiti `python main.py --train --data_dir putanja/do/IAM`
* Obuka će automatski prestati nakon izvesnog broja epoch-a bez poboljšanja
