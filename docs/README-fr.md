# Module blockchain pour *Prenez Place ! / Tournée été 2022*

<img src="./assets/banner-0.jpg" alt="banner-0" style="height:256px;" />

## À propos de *Prenez Place !*

> 🌐 [prenez-place.fr](https://prenez-place.fr/)

### Face B de *Prenez Place !*

Depuis 2021, [*Prenez Place !*](https://prenez-place.fr/) questionne les sujets de Monnaie, Communs et Démocratie grâce
à des débats conçus comme un geste artistique, scientifique et citoyen.

Invoquant par nature une intelligence collective et une approche pluridisciplinaire, le projet initie une nouvelle
phase à l'été 2022 : la face B.

<img src="./assets/banner-1.jpg" alt="banner-1" style="height:256px;" />

La face B, dans sa forme nomade, ouverte, est une suite de débats-performances itinérants qui auront lieu, dans un
premier temps, cet été 2022, sur des places, places de marché, des parkings, dans des hôpitaux, des gares, des forêts,
des lieux publics/privés/ouverts.

Ces débats-performances intègreront installations, danse, musique, chant,… et un module blockchain.

### Rôle de la Blockchain dans le projet

Les objectifs sont nombreux. Faire du débat citoyen un objet et un acte artistique. Faire émerger un nouvel espace
démocratique, une nouvelle forme d’agora, de délibération humaine. Dépasser la hiérarchisation systématique de la parole
à l'aide d'un réseau de voix plus décentralisé, soutenant l'émergence de la délibération. Rendre vivante la possibilité
d’un autre tissé, la possibilité d’une autre compréhension et d’autres pratiques de la démocratie et donc de nos
relations aux autres, aux autres espèces du vivant.

La Blockchain et les technologies Web3, ouvertes et décentralisées, questionnent en elles-mêmes les sujets de Monnaie,
Communs et Démocratie. Dans *Prenez Place !*, nous les utilisons aussi comme support d'une mémoire incrémentale et
indélébile des délibérations. Un récit collectif se construit de la conjonction des débats-performances et construit sa
propre mémoire.

### Collections NFT

Des enregistrements audio de ces débats — dans leur entièreté, ainsi que sectionnés en fragments — sont mis à
dispositions sur ces réseaux, comme collections de non-fungible tokens (NFT). Horodatés, certifiés, un lien
infalsifiable unit ces enregistrements et supporte la création d'un récit ouvert.

### Jetons incandescents, créateurs de Commun

Tandis que ces jetons NFT existent en tant que tels, ils ne pourront jamais être possédés. Après leur création, tout
achat ou transfert brûlera nécessairement le jeton concerné. Cette règle est inscrite au sein du contrat de la
collection en autorisant la cession d'un jeton uniquement à destination d'une adresse que personne ne contrôle. Ainsi,
on brûle sur la Blockchain chaque jeton comme dernier geste performatif de création d'un Commun.

### Dispositif de tissage en lien avec la blockchain

Lors des débats-performances, un tissage unique est également confectionné à l'aide d'un métier à tisser Jacquard. Une
information présente sur la blockchain et identifiant de manière unique chaque débat sert d'aléa pour concevoir une
carte perforée unique, ainsi responsable d'un fragment de la tapisserie.

## Fonctionnalités et mode d'emploi

### Architecture technique du module

Ce projet met à contribution diverses technologies Web3, suivant une approche générale qualifiable de [*Protocols, Not
Platforms*](https://knightcolumbia.org/content/protocols-not-platforms-a-technological-approach-to-free-speech).
Ainsi en effet, la solution interagit directement avec les réseaux décentralisés — pour le stockage ou la certification
par exemple — sans jamais nécessité de serveur centralisé.

- Le contract NFT utilisé est formellement compatible avec le standard [ERC-721](https://erc721.org/) dans son
  interface. Il a été édité entre autres pour rendre les jetons incandescents, créateurs de Commun.
- Le réseau [_the InterPlanetary File System_ (IPFS)](https://ipfs.io/) permet de stocker et échanger les métadonnées
  associées aux tokens —
  enregistrements audio, visualisations,…
- La blockchain [Filecoin](https://filecoin.io/) _via_ le service [NFT.Storage](https://nft.storage/) permet d'assurer
  la permanence du stockage et la disponibilité de cette donnée.
- Un autre smart contract est utilisé comme simpler _Store_ pour centraliser logiquement une liste de mots-clés à
  reconnaître durant les débats.
- Différents _sub-graphs_ ont été mis au point sur [TheGraph](https://thegraph.com/en/) pour indexer et faciliter l'exploration des informations ainsi stockées
  sur la blockchain.
- Enfin un client graphique a été mis au point pour assister à l'enregistrement des débats et la création automatique
  des nouveaux jetons.

<img src="./assets/screenshot-dashboard.png" alt="client-dashboard" style="height:256px;" />

On expose ci-dessous avec plus de détails les fonctionnalités principales de ce client graphique. 👇

### Enregistrement des débats

En cliquant sur _Démarrer un nouveau débat_, l'initialisation démarre.
On commence par déclarer le lieu du débat du jour.

<img src="./assets/screenshot-recording-0.png" alt="client-recording-0" style="height:256px;" />

Lorsque le reste du dispositif, audio notamment, est prêt, il reste à cliquer sur le bouton _Démarrer le débat_ pour
lancer l'enregistrement.

<img src="./assets/screenshot-recording-1.png" alt="client-recording-1" style="height:256px;" />

Durant la performance, l'écran permet à la volée, lorsque des mots-clés sont prononcés, de créer des fragments audio
relatifs.
En pratique, si le mot-clé _décentralisation_ est par exemple prononcé lors du débat, il suffit de cliquer sur l'icône
de microphone à côté du mot _décentralisation_ dans la liste — on peut s'aider du champ de recherche textuelle pour le
trouver — pour qu'un extrait sonore des quelques secondes précédant le clic soit enregistré.

Lorsque le débat est fini, il reste à cliquer sur _Terminer le débat_ — une confirmation sera demandée — pour clôturer
l'enregistrement du débat complet.

<img src="./assets/screenshot-recording-2.png" alt="client-recording-2" style="height:256px;" />

### Historique des débats

Le bouton _Historique des débats_ permet logiquement de consulter l'ensemble des débats passés.

<img src="./assets/screenshot-debate.png" alt="client-debate" style="height:256px;" />

### Mots-clés et fragments

Enfin la dernière entrée de l'écran principal permet d'éditer la liste des mots-clés qui seront accessibles durant
l'enregistrement.

<img src="./assets/screenshot-keywords.png" alt="client-keywords" style="height:256px;" />

### Paramètres

En bas à droite de l'écran, un bouton permet d'accéder au paramétrage de l'application.

|                       | Description                                                                                                                                              | Exemple                                      |
|-----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|
| `rpcPath`             | Endpoint RPC de la blockchain hébergeant les contrats NFT.                                                                                               | `https://polygon-rpc.com`                    |
| `ethPrivateKey`       | Clé privée pour créer des NFTs.<br/>Elle doit contrôlée les collections utilisées <br/>et posséder assez d'ether pour subvenir aux frais de transaction. | `0x0000..0000dead`                           |
| `ipfsApiToken`        | Token de l'API du service NFT.Storage.                                                                                                                   | `xxx.yyy.zzz`                                |
| `debatesNftAddress`   | Adresse de la collection NFT des débats complets.                                                                                                        | `0x6AC3F32051D82dd76Df9a1C1C6db44b549135b86` |
| `fragmentsNftAddress` | Adresse de la collection NFT des fragments.                                                                                                              | `0x64F873c5fdc1cE5d61Fd8db2c0d37894C88f1349` |

<img src="./assets/screenshot-settings.png" alt="client-settings" style="height:256px;" />
