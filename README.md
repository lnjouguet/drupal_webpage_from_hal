# Drupal module to include an html list of publications from Hal directly in your website #

## How does it works ? ##

This plugin creates a new filter which can be activated or not.

Once installed, create a new node and put on the body this modele:

`{{ type="webpage_from_hal" url="http://hal.univ-grenoble-alpes.fr/Public/afficheRequetePubli.php?auteur_exp=boris,morel&CB_auteur=oui&CB_titre=oui&CB_article=oui&langue=Francais&tri_exp=annee_publi&tri_exp2=typdoc&tri_exp3=date_publi&ordre_aff=TA&Fen=Aff&css=../css/VisuRubriqueEncadre.css"}}`

By this filter, Drupal gets the url and includes the html content directly on your body.

## Install ##
  1. This module requires [saga_base](https://github.com/Saga-UGA/saga_base) module.
  1. To install both plugins, refer to the official [Drupal documentation](https://drupal.org/node/895232).

## Activate ##
  1. The Drupal filters are managed on `text formats` section (/admin/config/content/formats).
  1. Choose which text format uses this filter.
  1. Enable `Include html content from hal url` filter.

**Note:**
> Caution, this filter should be placed among the top ones. If an other filter alters html content, there is a good chance that this filter does not retrieve the tag and so don't work !  
  
## Support ##

GitHub is the good way to contribute on this project.
  - Issue
  - Pull request
  - [...]
