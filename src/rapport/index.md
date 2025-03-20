# Rapport de veille - les IA Musicales

## 1. Introduction - sujets principaux du rapport


Ce rapport porte sur sur l'avancée des outils fonctionnant avec l'IA pour la génération musicale, notamment ceux portés par Meta, les enjeux autour cette technologie, et comment les cadres législatifs de l'IA et de la musique s'entrecroisent sur ce sujet.

## 2. Découverte et Technologies


    
**MusicGen API** : Service permettant de transmettre différents inputs au modèle MusicGen de Meta via une API. Les inputs consistent en un dataset, le type de sample souhaité ("audio" ici), la vitesse du sample et une description textuelle. Il y a une communauté assez active pour que des librairies facilitant son utilisation / déploiement existent.
    - Différence avec **AudioGen** : MusicGen est spécialisé dans la création musicale et n'est pas conçu pour créer des sons plus généralistes. Cette restriction volontaire permet de gagner du temps de le paramétrage des requêtes transmises au modèle. 
    - **Similarité d'utilisation** : Bien qu'ils aient des des applications distinctes, les deux services font partie de l'écosystème **AudioCraft** de Meta ce qui résulte en des fonctionnements et requêtes similaires. 

On peut aussi citer Magenta de Google et JukeBox d'OpenAI, mais dont les communautés sont moins (voire pu) actives.
## 3. Événements et Conférences

Mes recherches sur les réseaux sociaux et le web ne m'ont pas permis de trouver d'événements ou conférences portant spécifiquement sur la génération musicale via IA, le sujet étant encore très "jeune" (Audiocraft cité plus haut est sorti en Août 2023). La **Conference on AI and Music Creativity**  mais portait cette année plutôt sur la créativité musicale assistée par l'IA l'année dernière. Le sujet de la génération musicale par IA se limite pour l'instant à des articles de blogs & des posts sur les réseaux sociaux, même si la création musicale et l'informatique / l'ia ont toujours été un sujet de discussion de nombreux événements.     
## 4. Analyse de Marché

### Startups
- **Beatoven.ai** : a été certifié par https://www.fairlytrained.org/ pour leur utilisation d'un dataset éthique rémunérant les artistes dont proviennent leurs banques
- **Mubert** : a récemment sorti une feature "image to music" 

On constate beaucoup d'[[Echecs et abandons]] dans le secteur.
### Finance et investissement

Meta est la GAFAM ayant le plus récemment investie dans cette technologie en sortant MusicGen en août 2023. Google a de son côté sorti un modèle Open Source : Magenta, dont le dernier commit date de novembre 2021, mais qui dispose d'une communauté assez active. OpenAI a été la première à publier son modèle open source, Jukebox, il y a 4 ans. Cependant, celui-ci n'est plus tenu à jour depuis ce moment. 
## 5. Politique, Lois et Régulations

- **Changements DEI**: Cette année pourrait être un point de bascule pour les initiatives d'équité, de diversité et d'inclusion, face à des défis légaux et corporatifs croissants.
- **AI act** : L'Union européenne a adopté une législation encadrant l'intelligence artificielle. La France a accepté ce règlement européen sur l'IA, mais sous certaines conditions visant à préserver l'innovation.
    - Les conditions posées par la France sont le respect de l'équilibre entre transparence et préservation des secrets industriels.
    - 
(j'ai gardé ces informations car également en lien avec le sujet)

Également, le gouvernement français a lancé plusieurs initiatives pour promouvoir l'intelligence artificielle telles que le plan national pour l'IA annoncé en 2018, et soutient son développement en général. Plus largement, il a récemment annoncé l'arrivée de Mistral, censé concurrencer ChatGPT (bien qu'on sorte ici de la génération musicale). Le gouvernement d'Edouard Philippe a publié en 2019 un [appel à projets](https://www.gouvernement.fr/actualite/communique-de-presse-intelligence-artificielle-cap-sur-la-mutualisation-et-le-partage-de-donnees) visant à soutenir la création et/ou l’enrichissement et/ou l’exploitation de très grandes bases de données mutualisées, centralisées ou distribuées, permettant l’élaboration d’applications industrielles de l’IA. [Bercy soutient également que l'IA](https://www.economie.gouv.fr/entreprises/intelligence-artificielle) est un levier de croissance et d'innovation pour les entreprises.

Au niveau de l'IA musicale, la principale question soulevée au niveau de l'Occident (concernant la paie des artistes) est celle de la copie ou de l'inspiration : les musiques crées par IA sont elles des copies d'œuvres d'artistes ou seulement inspirées ? 

### Culture

Comme pour la génération d'images, de vidéos ou les autres formes d'applications créatives pour lesquelles on peut utiliser l'IA, la génération musicale fait débat autour de la question des droits d'artistes et de l'impact qu'aura la technologie sur la carrière de ceux-ci si elle est utilisée à mauvais escient.

## 7. Trouvailles

    
https://huggingface.co/blog/run-musicgen-as-an-api : simple tutoriel permettant de comprendre le fonctionnement de l'api de Musicgen, étant un débutant dans l'utilisation de modèles je considère que c'est une bonne porte d'entrée 

https://www.youtube.com/watch?v=Ey75Xw_ikqs : vidéo assez courte permettant de mieux situer le contexte juridique et culturel qui se pose autour de la génération musicale. La vidéo interview également le CEO de Spotify sur le sujet et aborde les évolutions possibles de la technologie 

### Outils pratiques découverts

Tous les outils de génération musicales listées ci-dessus, plus particulièrement leurs apis, comme celles de [MusicGen](https://facebookresearch.github.io/audiocraft/api_docs/audiocraft/models/musicgen.html#audiocraft.models.musicgen.MusicGen) , [beatoven](https://www.beatoven.ai/api) ou celle de [Mubert](https://mubert.com/blog/introducing-mubert-api-2-0).
### Ressources marquantes

https://www.york.ac.uk/news-and-events/news/2023/research/ai-generated-music-inferior-to-human-composed/ 
Globalement cet article résume tous les risques techniques et juridiques pouvant être énoncés sur la technologie jusqu'à maintenant (celle-ci n'ayant pas encore tellement évoluée depuis 2023 ) et permet de contrebalancer les discours trop optimistes sur celles-ci : les deux chercheurs dont parle l'article ont élaboré des directives de test sur ces IA, ces tests ont démontré que leurs algorithmes présentaient bien des faiblesses les menant aux erreurs de droits d'auteurs (comme on a pu le voir avec les IA générant des images) en copiant beaucoup trop de portions de musiques existantes pour l'instant. De plus, un échantillon de testeurs aveugles a préféré dans tous les cas la musique humaine...



## 8. Conclusion
### Analyse et Perspectives

De mon point de vue, la génération musicale par IA est une technologie prometteuse en tant qu'assistant des artistes ou sound designers, et son automatisation par des équipes techniques permettrait de faire gagner un temps considérable sur bon nombre de projets de tous types. Mais elle est encore trop immature pour pouvoir concurrencer techniquement à elle seule la créativité humaine sur le plan "artistique", a les mêmes problèmes techniques que les autres IA notamment au niveau du copyright des oeuvres qu'elle peut générer, et la question de la provenance des datasets doit se poser. Ce sont selon moi des freins importants au développement de cette technologie pour les entreprises souhaitant investir dedans (cf les différentes fermetures listées ci dessus). Reste à voir ce que Meta réalisera avec leur outil et **l'orientation** qu'ils lui donneront.

### Propositions d’action

Je vois en cette technologie l'opportunité d'automatiser des bases de samples via un script permettant de me générer une librairie basée sur des mélodies dont je m'inspire. Cela me permettrait de me former à l'utilisation de ce genre de technologies et de me faire gagner du temps sur la création de samples.

## Ressources

Compilation des ressources marquantes qui ont nourri la veille :  
- [Jukebox sur GitHub](https://github.com/openai/jukebox/)  
- [Magenta.js sur GitHub](https://github.com/magenta/magenta-js/commits/master/)  
- [Documentation MusicGen](https://facebookresearch.github.io/audiocraft/api_docs/audiocraft/models/musicgen.html#audiocraft.models.musicgen.MusicGen)  
- [MusicGenSolver Documentation](https://facebookresearch.github.io/audiocraft/api_docs/audiocraft/solvers/musicgen.html#audiocraft.solvers.musicgen.MusicGenSolver)  


