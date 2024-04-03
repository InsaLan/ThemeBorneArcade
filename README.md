# Le thème de la borne d'arcade

Bien sur c'est le best! Signé, votre resp élec adoré, Pixelbo !

## Ajouter une couleure pour une collection custom:

Soit {collec} le nom de la colection:

 - Il faut d'abord créer un {collec}.xml dans _inc\systems\metadata-custom\{collec}.xml
 - Dedans, il faut mettre le template puis l'éditer (voir ci-dessous la template)
 - Afin de rajouter l'image de cover, metter {collec}.webp dans _inc\systems\images\{collec}.webp
 - et voilà c'est fait, plus qu'à redémarrer ES-DE

### Template

Et voici le fameux template.xml avec les paramètres qui vont avec:

```xml
<theme>
   <variables>
      <systemName>Zelda</systemName> <!--Nom de la collection-->
      <systemDescription>La meilleure des princesse </systemDescription><!--Description de la collection-->
      <systemManufacturer>&#032;</systemManufacturer> <!--Trad de l'anglais svp-->
      <systemReleaseYear>&#032;</systemReleaseYear> <!--Trad de l'anglais svp-->
      <systemReleaseDate>&#032;</systemReleaseDate> <!--Trad de l'anglais svp-->
      <systemReleaseDateFormated>&#032;</systemReleaseDateFormated> <!--Trad de l'anglais svp-->
      <systemHardwareType>Genre de jeu</systemHardwareType> <!--Type de collection-->
      <systemCoverSize>1-2</systemCoverSize> <!--Taille de l'image-->
      <systemColor>CFA83E</systemColor> <!--Couleur principale de la collection-->
      <!-- (dépend du variant de couleur) -->
      <systemColorPalette1>FF0000</systemColorPalette1> <!--Couleur 1 de la collection-->
      <systemColorPalette2>0000A0</systemColorPalette2> <!--Couleur 2 de la collection-->
      <systemColorPalette3>FFE41B</systemColorPalette3> <!--Couleur 3 de la collection-->
      <systemColorPalette4>23B14D</systemColorPalette4> <!--Couleur 4 de la collection--> 
   </variables>

   <view name="system">
      <text name="system-label">
         <text>${systemHardwareType}</text><!--Vous pouvez utiliser les variables à votre guise cf. https://gitlab.com/es-de/emulationstation-de/-/blob/master/THEMES.md-->
      </text>
   </view>
</theme>
```

## TODO:

 - Script/gui pour automatiser tout ça
 - Mettre avec le script pour les collections :thinking:
---
Crédit à anthonycaccese pour la création du thème [original](https://github.com/anthonycaccese/colorful-simplified-es-de)