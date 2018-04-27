
# checkout-cfa-exp-api

+ [License Agreement](#licenseagreement)
+ [Use Case](#usecase)
+ [Considerations](#considerations)
+ [Customize It!](#customizeit)
	* [config.xml](#configxml)
	* [businessLogic.xml](#businesslogicxml)
	* [endpoints.xml](#endpointsxml)
	* [errorHandling.xml](#errorhandlingxml)


# License Agreement <a name="licenseagreement"/>
Note that using this template is subject to the conditions of ?

# Use Case <a name="usecase"/>
As a ? I would like to...

# Considerations <a name="considerations"/>

To make this Anypoint Template run, it must be customized to add the API RAML, API implementation logic, deployment names

###FAQ

 - Where can I ...?
- Can I modify the Field Access Settings? How?


# Customize It!<a name="customizeit"/>

To use the template:
1. Rename all the config.x.properties files' with api name then in each file replace api.name and api.version configuration values with the API values found in the Anypoint API Platform definitions.
2. Replace the this.experience.api.client-id and this.experience.api.client.secret values with the client credentials register for this application.
3. Modify the pom.xml and replace: 
  1. the artifactId with the correct name. This name is used when the project is deployed using maven.
  2. the version with the correct project version (such as 1.0.1). This version is used when the deployment executable is created.
4. Replace all the RAML definition files in the src/main/api directory with the RAML definitions to be used for the new API.
5. Regenerate flows from RAML and rearrange the generated code to fit with the project's file structure.
6. Add the appropriate inbound payload and outbound payload transformations.  A generic outbound payload transformer (serialize-in-requested-format) is provided in the common-utils.xml.  The transformer assumes the payload is in a java.util.Map compatible format and does not assume a specific data structure.  Note that xml attributes will not be transformed correctly with the generic transformer.  If this is required, then DataWeave should be used to perform the transform.
7. Lastly, replace this README.md file with one appropriate for the project you are creating.

Hint: Use the file search for "skeleton" to find all the places to change.
