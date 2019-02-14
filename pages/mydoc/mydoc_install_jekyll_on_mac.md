---
title: Manual de instalación
tags: [getting_started, troubleshooting]
keywords:
Resumen: "Esta sección describe cómo descargar e instalar Oracle Application Express. La forma de instalar Oracle Application Express depende del tipo de base de datos en la que se esté instalando."
sidebar: mydoc_sidebar
permalink: mydoc_install_jekyll_on_mac.html
folder: mydoc
---


## Arquitectura de APEX 
La arquitectura de APEX es bastante simple. Tienes que tener un navegador que se comunique a través de una aplicación Java de nivel medio (mid-tier) que en nuestro caso es el *Oracle REST Data Service (ORDS)* y que puede ser instalada en Oracle Web Logic Server usando Jetty o Tomcat. Luego esas peticiones se envían a través de la base de datos y todo el procesamiento se realiza en la base de datos Oracle, donde se encuentra el motor apex, y luego envía la petición de vuelta a través del ORDS y de vuelta al navegador.

{% include image.html file="pic3.png" alt="Jekyll" caption="Arquitectura de APEX" %}



## 1. Base de datos Oracle 

La base de datos de Oracle está disponible en cinco ediciones, cada una adecuada para diferentes escenarios de desarrollo e implementación. Éstas son:

* <b>Oracle Database Standard Edition One</b> para pequeñas empresas y entornos de sucursales altamente distribuidos.

* <b> Oracle Database Standard Edition </b> para máquinas más grandes y clustering de servicios con Oracle Real Application Clusters (Oracle RAC).

* <b> Oracle Database Enterprise Edition </b> para aplicaciones de procesamiento de transacciones en línea (OLTP) de gran volumen, almacenes de datos con gran cantidad de consultas y aplicaciones de Internet exigentes.

* <b> Oracle Database Express Edition (Oracle Database XE) </b> es una edición básica de Oracle Database que es gratuita.

* <b> Oracle Database Personal Edition </b> es compatible con entornos de desarrollo e implementación de un solo usuario que requieren compatibilidad total con Oracle Database Standard Edition One, Oracle Database Standard Edition y Oracle Database Enterprise Edition.

Para descargar alguna de las ediciones de bases de datos de Oracle vaya a la página oficial de Oracle: <a href="https://www.oracle.com/technetwork/database/enterprise-edition/downloads/index-092322.html">link de Descarga</a>


## 2. Oracle REST Data Services

Oracle REST Data Services (ORDS) makes it easy to develop modern REST interfaces for relational data in the Oracle Database and the Oracle Database 18c JSON Document Store. A mid-tier Java application, ORDS maps HTTP(S) verbs (GET, POST, PUT, DELETE, etc.) to database transactions and returns any results formatted using JSON.
ORDS ya viene incluido con las instalaciones de Oracle Database y Oracle SQL Developer por lo que no es necesario descargarlo de nuevo. Para obteneer más información de ORDS visite el sitio oficial de Oracle. <a href="https://www.oracle.com/database/technologies/appdev/rest.html"> Sitio oficial de Oracle </a>

## 3. Navegador web

Oracle Application Express requiere un navegador compatible con JavaScript y es compatible con la versión actual y anterior de Google Chrome, Mozilla Firefox, Apple Safari, Microsoft Internet Explorer y Microsoft Edge.

## 4. Oracle Application Express

Cualquier edición de Oracle Database 11 g o superior incluye Oracle Application Express versión 4.2.6.00.03. Por lo que no es necesario descargar APEX nuevamente. Sin embargo se recomienda encarecidamente que se actualice a la última versión de Oracle Application Express para aprovechar todas las funciones más recientes. Para conocer en detalle cómo actualizar a la última versión de APEX vaya a <a href="https://www.oracle.com/technetwork/developer-tools/apex/learnmore/upgrade-apex-for-xe-154969.html">link de actualización de APEX</a>





{% include links.html %}

