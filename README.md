# JPPT-0 : Je n'ai Pas PéTé mon budget calcul! 
## Zéro dollar de calcul...

## Génération simple de textes en français avec des modèles de Markov

par Claude COULOMBE - Ph. D. / consultant en IA appliquée / Lingua Technologies inc.

JPPT-0, un petit générateur de textes en français basé sur un modèle de langue (i.e. un modèle de prédiction du prochain mot) à base de ngrammes et d'une chaîne de Markov. 

Pour cela, il crée un index de trigrammes et de leur fréquence par un dépouillement très rapide d'un petit corpus en quelques secondes sur un micro-ordinateur ordinaire.

Sur l'idée de la chaîne de Markov, un modèle prédictif ainsi constitué peut générer un texte en se basant sur le mot ou gramme qui est le successeur le plus probable de deux mots donnés. Pour démarrer on fournira les deux premiers mots (un germe) ou autrement le générateur fera un choix aléatoire. 

## Pourquoi?

Avec JPPT-0, il est possible de créer des modèles capables de générer des textes assez bluffants, du moins amusants ou poétiques, sans avoir à entraîner des modèles d'apprentissage profond pendant des jours sur des corpus représentant une fraction importante du contenu de la Toile.

GPT-2 pour Generative Pre-training Transformer) auraient été entraînés sur un corpus énorme (40 gigaoctets de textes) pendant une semaine sur une architecture comportant 32 processeurs spécialisés dans les calculs matriciels (TPU: Tensor Processor Unit). On estime les coûts de calcul du modèle comportant 1.5 milliards de paramètres à environ 60 000 dollars canadiens. Ce n’est que la pointe de l’iceberg, car on néglige tous les calculs ayant menés à sa mise au point. On estime que l'entraînement de GPT-3, le successeur de GPT-2, qui comporte 175 milliards de paramètres, aurait coûté plus de 5 millions de dollars canadiens en temps de calcul.

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
