Labeling Paintings with Thematic and Emotional Content
 
 Mašinsko učenje - seminarski rad

 Aleksandra Trailović, Sara Kapetinić

Ovaj rad koristi skup podataka Wikiart I radi klasifikaciju na osnovu teme I emocija.

Zbog nekonzistentnosti skupova, koriscena su dva razlicita za ove dve klasifikacije. Skup za klasifikaciju po temama se moze naci na adresi https://huggingface.co/datasets/huggan/wikiart, dok skup za klasifikaciju po emocijama je sa sajta https://www.kaggle.com/datasets/gabrieletirrito/artemis-full.

Klasifikacija na osnovu tema:
- Koriscena su tri modela na osnovu istrazivackog rada sa Stanford-a
- Modeli su: VGG16, AlexNet I custom model koji je kreiran
- Skup podataka je smanjen zbog performansi I uradjen je oversampling jer su podaci bili nejednako rasporedjeni po klasama
- Kao statistike korisceni su parametri gubitak, tacnost I matrica konfuzije
- Najkrace kroz epohe je prolazio model AlexNet tokom treniranja, a najbolju tacnost je dao VGG16.

Klasifikacija na osnovu emocija:
- Koriscen je restnet18
- Dostigli smo validacionu tacnost od 93%.
- Smanjili smo skup podataka I uradili oversampling kako bi podaci bili ravnomerno rasporedjeni po klasama
- Ciljna promenljiva se sastoji od 8 klasa, a svaka instanca moze pripadati u vise klasa
- Prikazane su I matrice konfuzije sa TP, FN, FP, TN vrednostima po klasama

