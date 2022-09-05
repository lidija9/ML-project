# Autonomna vozila

Projekat ima za cilj da pokaze kako mozemo iskoristi metode masinskog ucenja u cilju obucavanja autonomnog vozila. Zbog kompleksnosti Self Driving problema, fokusiracemo se na jedan deo - detekcija automobila i prepoznavanje saobracajnih znakova.

Autori: Brankica Tubin 1091/2021 i Lidija Tomanic 1034/2020

Broj autonomnih vozila se sve vise povecava iz godine u godinu. Ljudima je tesko da imaju poverenja u automobile i avione koji se krecu bez vozaca i pilota, dok je u zeleznickom saobacaju to vise zastupljeno iz razloga sto voz ne moze da prestize drugi voz prilikom kretanja.
Autonomna vozila koriste senzore, kamere, aktuatore, mikroprocesore u vrlo slozenim algoritmima. Senzori i kamere imaju ulogu “ociju” i “usiju” vozila, koji posmatraju kretanje na putu i salju podatke kontrolnom sistemu. Mikroprocesor obradjuje podatke primljene preko senzora i kamera i salje signal aktuatorima da izvrse odredjene radnje, kao na primer menjanje brzine, kocenje, okretanje volana itd.
Kamere prikupljaju vizuelne podatke iz okoline. Osnovni podaci koji treba da budu u bazi su saobracajni znaci. Kada kamera snimi crveno svetlo, mikroprocesor treba da posalje signal aktuatorima da se vozilo zaustavi, kamera i dalje neprestano prikuplja podatke iz okoline i salje signale kontrolnom sistemu, gde ce mikroprocesor opet poslati signal akturatorima da prebace u prvu brzinu, otpuste kocnicu i pritisnu gas, kada se pojavi zeleno svetlo.
Sve ovo su veoma kompleksne operacije, kompleksni softveri, koji takodje mogu da budu hakovani i da poremete rad senzora, posalju pogresne inforamcije, prate vozilo itd. Kamere treba da budu ciste usled raznih vremenskih uslova, a tu si i drugi zahtevi tehnologije, koji su veoma skupi i time doprinose nedostacima autonomnih vozila.

U ovom radu cemo videti neke nacine manipulacije slikama kao i primenu SVM i deep learning-a u automobilskoj industriji.

Rad je podeljen u dve jupyter sveski radi bolje organizacije:

- sveska_1 - u ovoj svesci je odradjeno ucitavanje skupa podataka - slike na kojima se nalaze, tj. ne nalaze automobili kao i primena SVM u klasifikaciji da li se na slici nalazi ili ne nalazi automobil

- sveska_2 - ucitavamo drugi skup podataka - saobracajne znakove a potom ucimo CNN da prepoznaje koji znak se nalazi na slici

### Literatura

- https://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset
- J. Stallkamp, M. Schlipsing, J. Salmen, and C. Igel, “The German Traffic Sign Recognition Benchmark: A multi-class classification competition” In Proceedings of the IEEE International Joint Conference on Neural Networks, pages 1453–1460. 2011.

- Nikola Tomikj, and Andrea Kulakov, “Vehicle Detection with HOG and Linear SVM” In Proceedings of the Journal of Emerging Computer Technologies
- R. Girshick, J. Donahue, T. Darrell, and J. Malik, “Rich Feature Hierarchies for Accurate Object Detection and Semantic Segmentation,” in 2014 IEEE Conference on Computer Vision and Pattern Recognition, Jun. 2014, pp. 580–587, doi: 10.1109/CVPR.2014.81.
- J. Williams, “Vision meets Robotics: The {KITTI} Dataset | Autonomous Vision,” Max Planck Institute for Intelligent Systems. 
- Grupo de Tratamiento de Imágenes (GTI), “Vehicle Image Database.” https://www.gti.ssr.upm.es/data/Vehicle_database.html.
- N. Dalal and B. Triggs, “Histograms of oriented gradients for human detection”, in International Conference on computer vision & Pattern Recognition (CVPR’05), IEEE Computer Society, vol. 1, 2005, pp. 886–893.
- David Watson, Graham Brown, “Cambridge IGCSE Information and Communication Technology Third Edition”, Hodder Education, 2021.

