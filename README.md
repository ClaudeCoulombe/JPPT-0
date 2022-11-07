# JPPT-0 : Je n'ai Pas PéTé mon budget calcul! 
# Génération de textes à zéro dollar de calcul...

## Génération simple de textes en français avec des modèles de Markov

par Claude COULOMBE - Ph. D. / consultant en IA appliquée / Lingua Technologies inc.

JPPT-0, un petit générateur de textes en français basé sur un modèle de langue (i.e. un modèle de prédiction du prochain mot) à base de ngrammes et d'une chaîne de Markov. 

Pour cela, il crée un index de trigrammes et de leur fréquence par un dépouillement très rapide d'un petit corpus en quelques secondes sur un micro-ordinateur ordinaire.

Sur l'idée de la chaîne de Markov, un modèle prédictif ainsi constitué peut générer un texte en se basant sur le mot ou gramme qui est le successeur le plus probable de deux mots donnés. Pour démarrer on fournira les deux premiers mots (un germe) ou autrement le générateur fera un choix aléatoire. 

## Exemples

### Le coeur a ses raisons (Marc Labrèche)

Brett: Cette literie satinée a transformé mon lit en une véritable glissoire de la bouche de Doug, sans le vouloir, contre leur gré, quoi. Brett: Tu sembles tenir la forme? Brad: Brad!! Brad: Oublions nos vieilles querelles... Serrons-nous. Ils s'embrassent. Rideau. Brett: Ne vous inquiètez pas Criquette. Lorsqu'un sourire reptilien. Brett: Oui.. C'est ça?! Brett: Wow. Pardonnez-moi, Brett? Brett: Vous avez fait votre choix? Ridge: Ridge pense... Malgré un doctorat en philosophie et une maîtrise en danse africaine, je?? Doug: Je ne sais pas. Sortons nos jumelles de poches. Si pratiques lors des voyages ou des safaris photos. Ils sortent des jumelles imaginaires.

### Mathieu BOT Côté (Journal de Montréal)

Québec libre. Quelle sera la véritable raison du fait qu'on en arrive à la veille que cela. Après avoir compilé les études portant sur les enjeux du jour au lendemain de l'histoire politique a-t-il? La CAQ est en train de marquer une claire volonté indépendantiste suffirait-il de la loi sur la route du temps, pour rappeler que le sien sans l'évolution des prénoms américains ( Logan, Tyler, Jayden, etc.), les deux avenirs possibles de nombreux pays. Je vous donne-t-il pas naturellement les animer. Plus l'identité québécoise sans un gouvernement enthousiaste désireux de ne pas arriver ». Le sens du silence, de la droite, étrangement, la loi.

### La Génèse

Dieu dit: Que cherches-tu fait? La femme vit que l'un demi-sicle, et se rendit vers Pharaon. Pharaon dit à Laban: Donne-moi. Et ils firent entendre de grandes plaies Pharaon et à ta race. On fit descendre Joseph en égypte, et se présentèrent devant Joseph. Ils s'approchèrent, et il y avait du pain contre vos troupeaux, si l'entrée d'ésaü: elle enfanta un fils. Et Laban lui donna le même ordre au premier-né, que ton âme me bénisse. Isaac dit: Si vous êtes des espions.

## Pourquoi?

Avec JPPT-0, il est possible de créer des modèles capables de générer des textes assez bluffants, du moins amusants ou poétiques, sans avoir à entraîner des modèles d'apprentissage profond pendant des jours sur des corpus représentant une fraction importante du contenu de la Toile.

GPT-2 pour Generative Pre-training Transformer) auraient été entraînés sur un corpus énorme (40 gigaoctets de textes) pendant une semaine sur une architecture comportant 32 processeurs spécialisés dans les calculs matriciels (TPU: Tensor Processor Unit). On estime les coûts de calcul du modèle comportant 1.5 milliards de paramètres à environ 60 000 dollars canadiens. Ce n’est que la pointe de l’iceberg, car on néglige tous les calculs ayant menés à sa mise au point. On estime que l'entraînement de GPT-3, le successeur de GPT-2, qui comporte 175 milliards de paramètres, aurait coûté plus de 5 millions de dollars canadiens en temps de calcul. Ces grands modèles sont hors de portée de toutes les organisations, sauf les plus riches, comme le GAFAM.

En entraînant à faible coût JPPT-0 sur de petits corpus spécialisés, par exemples des lettres de motivation, il est relativement facile de créer de petites applications sans péter son budget calcul.   


## À défaut d'intelligence artificielle, nous avons créé de l'intelligence superficielle!

Les générateurs de texte auto-attentifs du style GPT-X (j'essaie d'éviter le mot « Transformer » qui se rapporte à un dessin animé japonais et qui ne veut strictement rien dire) demeurent très limités sur le plan sémantique. Par contre, ces outils peuvent être utiles pour contrer le « syndrome de la page blanche » et générer des babillages insignifiants... Cela dit, une personne intelligente peut s'en servir en filtrant et corrigeant les idioties.

Soulignons que la Francophonie a maintenant, <a href="https://cedille.ai/">« Cédille »</a>, un « idiot savant » de qualité équivalente à ceux de langue anglaise. D'après mes tests assez limités, « Cédille » est visiblement meilleur en français que les GPT-X multilingues. Aussi, ses réponses son « culturellement » teintées de la culture francophone. Par exemple, il va faire des allusions au Québec, Canada, France, etc.

Notons en terminant que les avancées récentes en traduction automatique neuronale, les modèles neuronaux du langage et le mécanisme d’attention sur lequel est basé l’architecture Transformer utilisée par BERT et GPT-X originent en grande partie des travaux pionniers du MILA et de l’équipe de Yoshua Bengio de l’UdeM qui ont été perfectionnés et industrialisés par Google et OpenAI.

### Sources d'inspiration:

Discussions toujours passionnantes avec mon ami <a href=https://recherche.umontreal.ca/nos-chercheurs/repertoire-des-professeurs/chercheur/is/in15254/>Patrick Drouin</a>, Ph.D. professeur titulaire en traduction et terminologie à l’Université de Montréal.  

https://fr.wikipedia.org/wiki/Cha%C3%AEne_de_Markov

https://www.nltk.org/

https://www.nltk.org/book/

http://stackoverflow.com/questions/18391602/what-does-generate-do-when-using-nltk-in-python

http://www.mikesboyle.com/post/117202964694/python-nltk-wtf-chapter-1-notes-on-things-that

http://www.gilesthomas.com/2010/05/generating-political-news-using-nltk/

http://www.cs.princeton.edu/courses/archive/spr05/cos126/assignments/markov.html

http://stackoverflow.com/users/55562/lakshman-prasad

http://stackoverflow.com/questions/32441605/generating-ngrams-unigrams-bigrams-etc-from-a-large-corpus-of-txt-files-and-t

https://lactualite.com/sante-et-science/faut-il-avoir-peur-des-robots-redacteurs/

## Licence

Copyright (C) 2021-2022 - Claude COULOMBE

Sous licence Apache, Version 2.0 (la "Licence");

Vous ne pouvez pas utiliser ce fichier, sauf conformément avec la licence.
Vous pouvez obtenir une copie de la Licence sur
http://www.apache.org/licenses/LICENSE-2.0

Sauf si requis par la loi en vigueur ou par accord écrit, le logiciel distribué sous la licence est distribué "TEL QUEL", SANS GARANTIE NI CONDITION DE QUELQUE NATURE QUE CE SOIT, implicite ou explicite. Consultez la Licence pour connaitre la terminologie spécifique régissant les autorisations et les limites prévues par la licence.

