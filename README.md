# Storefront
This repo contains JSON and image data for OSC-ToolKit's Storefront.  

## status.json
`status.json` is used by the ToolKit to check if the Storefront is undergoing some planned modifications or not.
```json
{
  
  "online"            : false,
  "reason"            : "The Storefront is undergoing maintenance.",
  
  "statLinkExists"    : true,
  "statLinkCaption"   : "More Information",
  "statLinkURL"       : "https://github.com/OpenShopChannel/Storefront"
  
}
```  
`online` : Is the Storefront online?  
`reason` : If offline, will display the string assigned.  
`statLinkExists` : Shows a button below reason.
`statLinkCaption` : Caption for the button.
`statLinkURL` : URL to load in an external browser on click of the button.  

## links.json
`links.json` gives a list links for the ToolKit to use when building URLs.
```json
{

  "catalogue"   : "catalogue/",
  "news"        : "news/"

}
```
## catalogue/index.json
`index.json` gives categories in an array that ToolKit can access.
```json
{
  "sfCategories" :
  [
    {

      "catName": "Games",
      "catDesc": "Pass the time with these fun apps!",

      "catURL": "games/",
      "catVisible": true

    }
  ]
}
```
`catName` : Name of category.  
`catDesc` : A short description of category.  
`catURL` : The URL for the category.  
`catVisible` : Determines if the category is visible or not.  

## news/index.json
`index.json` gives news items in an array.
```json
{
  "newsIndex" :
  [
    {

      "artTitle"   : "1.2.0 is Here!",
      "artSummary" : "1.2.0 brings new fixes and new things to do online.",

      "artURL"     : "articles/120ishere-001.json",
      "artImgURL"  : "img/120ishere-001-thumb.png"

    }
  ]
}
```
`artTitle` : Title of article.  
`artSummary` : Summary of article.  
`artURL` : URL to the article.  
`artImgURL` : URL to the article's image.