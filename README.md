# This repository contains customization made by CNR-ILC. See https://github.com/ufal/lindat-dspace/wiki/Overlays #

## Customizations at 23/06/16 ##

* installations/webapps/oai/static/style.xsl
* installations/webapps/xmlui/themes/UFAL/lib/xsl/core/navigation.xsl
* installations/webapps/xmlui/themes/UFAL/lib/html/about.html
* installations/webapps/xmlui/themes/UFAL/lib/html/privacypolicy.html
* installations/webapps/xmlui/themes/UFAL/lib/js/aai_config.js
* installations/webapps/xmlui/themes/UFALHome/lib/xsl/page-structure.xsl
* installations/webapps/xmlui/i18n/messages.xml

According to Overlays we have defined a git repository and moved all customization under [dspace]/modules
Under [dspace]/modules/ we must create the same structure that we have in source code, for example the customization 
installations/webapps/xmlui/themes/UFAL/lib/html/about.html comes from the source dspace-xmlui/src/main/webapp/themes/UFAL/lib/html

Under [dspace]/modules/ we must have xmlui/src/main/webapp/themes/UFAL/lib/html structure where we save the about.html

#procedures

1. create (mkdir -p) the directory structures
2. copy the files
3. git init under dspace/modules
4. git add <list_added_files>
5. git remote add origin https://github.com/cnr-ilc/ilc4clarin-overlays.git
6. create readme (first time)
7. git commit -m"message" 
8. git push -u origin master
