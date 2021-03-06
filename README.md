# EI-SE5_2020_2021_eDoudou
Projet_Objets_Connectes

Notre produit est un doudou connecté. Il est destiné aux jeunes parents qui possèdent un nouveau-né. L’objectif de ce produit est, d’une part de monitorer l’environnement de la chambre du bébé pour qu’il puisse passer ses meilleures nuit, et d’autre part de pouvoir alerter les parents si le bébé est vulnérable.

Le syndrome de mort subite du nourrisson (SMSN) désigne la mort inattendue d’un bébé. Ce syndrome se produit généralement durant le sommeil : un bébé en bonne santé s’endort et cesse de respirer, sans cause médicale apparente. Ce syndrome est souvent lié à une mauvaise position du bébé dans le lit (sur le ventre). Pour cela nous avons intégré des capteurs de mouvements pour savoir si le bébé bouge beaucoup et ainsi prévenir les parents au cas où le bébé serait sur le ventre.

Pour que notre produit soit complet, nous avons choisi d’intégrer des capteurs de température et d’humidité pour que le bien-être du nourrisson soit maximal. En effet, le bébé développe son cerveau principalement la nuit. Une chambre à mauvaise température peut troubler son sommeil et ainsi défavoriser sa croissance.

Enfin, nous avons intégré un capteur de bruit qui est capable de reconnaître les cris/pleurs du nourrisson. Ainsi, le dispositif du doudou connecté pourra allègrement remplacer les babyphones, qui peuvent réveiller les parents sans raisons particulières.

# Codes :
Les codes sont disponibles dans le répertoire 'src' 
</br>Les librairies sont le répertoire 'lib' mais ils sont compressés au format .zip car trop lourd pour les uploads sinon.


# Composants :
1/ Micro controlleur: Arduino nano 33 BLE sense
</br>2/ Communication : SigFox Module SFM10R1 Breakout board BRKWS01

# Logiciels :
1/ Arduino IDE pour utiliser les librairies Edge Impulse
</br>2/ PLateformeIO via Visual Studio Code pour le reste

# Traitement des datas
Nous avons opté pour la terchnologie des LPWANs avec l'utilisation de Sigfox pour faire remonter l'information jusqu'à l'utilisateur.</br>
1/ Activer son module sigfox sur Sigfox Backend.
</br>2/ Faire des callBacks vers le cloud Ubidots pour visualiser les datas sur un DashBoard et pouvoir s'occuper des alarmes.
</br>3/ Attention il n'est pas possible de créer des alarmes directement sur Ubidots. il faut les gérer en local sur la carte puis envoyer ces alarmes sur Sigfox puis Ubidots.
