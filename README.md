# IIQ Tools JDP (beta)

This plugin provides tools for generating BeanShell scripts from related Java classes for IdentityIQ

## Installation

Install IIQ Tools JDP Plugin from update site: http://iiqtools.com/jdp/update-site/

![Alt text](images/install/install-000.png?raw=true "Title")


## Usage

Create a Java Project and configure Java Build Path.
![Alt text](images/project/project-001.png?raw=true "Title")
![Alt text](images/project/project-002.png?raw=true "Title")
![Alt text](images/project/project-003.png?raw=true "Title")
![Alt text](images/project/project-004.png?raw=true "Title")
![Alt text](images/project/project-005.png?raw=true "Title")

Create new source folder `dev`
![Alt text](images/project/project-006.png?raw=true "Title")
![Alt text](images/project/project-007.png?raw=true "Title")

Create a new Java Class
* `@IIQArtefact` - mandatory annotation.
  - name - relative (to Java Project) path to the related xml artefact
  - xpath - a node inside xml to update
* `@IIQArtefactBody` - the main method that body is extracted and copied into target XML node. All other methods are copied as is.
* `@IIQArtefactIgnore` - fields and methods marked with this annotation will be excluded from result script.
![Alt text](images/project/project-008.png?raw=true "Title")

Create a new IdentityIQ Rule
![Alt text](images/project/project-009.png?raw=true "Title")

Click the IIQ Artefact button on the main toolbar while the Java class is selected
![Alt text](images/project/project-010.png?raw=true "Title")

Review changes made in the xml file
![Alt text](images/project/project-011.png?raw=true "Title")

