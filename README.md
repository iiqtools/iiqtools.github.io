# IIQ Tools JDP (beta)

Tired of lack of code validation and formating in SailPoint IdentityIQ? Try it in real Java ...

This plugin provides tools for generating BeanShell code from linked Java classes for SailPoint IdentityIQ


## Installation

Install IIQ Tools JDP Plugin from update site: http://iiqtools.com/jdp/update-site/
![Alt text](images/install/install-001.png?raw=true "Title")

## Usage

Create a new Java Project
![Alt text](images/project/project-001.png?raw=true "Title")   

Create new source folder 'dev'
![Alt text](images/project/project-002.png?raw=true "Title")   

Add IIQ Tools Library on the build path
![Alt text](images/project/project-003.png?raw=true "Title")   

Optional - specify location of the IdentityIQ libraries
![Alt text](images/project/project-004.png?raw=true "Title")
![Alt text](images/project/project-006.png?raw=true "Title")
![Alt text](images/project/project-007.png?raw=true "Title")
  
Unzip SSB files on the project folder
![Alt text](images/project/project-008.png?raw=true "Title")

Create a new IIQ Artefact
![Alt text](images/project/project-010.png?raw=true "Title")

Create a new Java Class
* `@Artefact` - mandatory annotation.
  - name - relative (to Java Project) path to the related xml artefact
  - xpath - a node inside xml to update
* `@ArtefactBody` - the main method that body is extracted and copied into target XML node. All other methods are copied as is.
* `@ArtefactIgnore` - fields and methods marked with this annotation will be excluded from result script.

Click the IIQ Artefact button on the main toolbar while the Java class is selected
![Alt text](images/project/project-012.png?raw=true "Title")

Review changes made in the xml file
![Alt text](images/project/project-013.png?raw=true "Title")

