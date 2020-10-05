# DCAT Application profile for base registries in Europe (BRegDCAT-AP) Catalog Description Mapping Tool

The BRegDCAT-AP v2.0.1 Mapping Tool will allow European public administrations to create mappings in order to harmonise different data models used for describing BRegDCAT-APs, either within a country or across borders, to another data model, being the BRegDCAT-AP v2.0.1 or any other data model. 

The tool can also visualise the mappings, export them in a machine-readable format, and analyse the coverage between the two mapped data models. The Mapping Tool is key for the 


## Deployment

### Docker

This application has configured to launch a [docker](https://www.docker.com/) cointainer ready to use. This requires that you have [docker](https://www.docker.com/) and [docker-compose](https://docs.docker.com/compose/install/). To run:

    $ cd path_to_mapping
    $ docker-compose up --build

The application can be accessed on http://localhost:40081/

### Local deployment 

This application is based on [drupal](https://www.drupal.com). This projects contains an installation and an initial database (dcat-mapping-database.sql). Follow the Drupal's [documentation](http://drupal.org/documentation) to configure an Drupal project.

To deploy the Public Service Description Editor locally, the administration will require PHP and Drupal environments installed on their webserver. The PHP version used is 5.6.15; the Drupal version is 7.42. Finally, a Virtuoso Triple store is needed to store the data created by the users.

## Virtuoso

Virtuoso endpoints is hardcoded un CPSVAPmapping module in /sites/all/modules/ folder. Review this URL and adapt to your instalation.