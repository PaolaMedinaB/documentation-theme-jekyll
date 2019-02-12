---
title: Conocimientos previos
tags:
  - getting_started
keywords: "features, capabilities, scalability, multichannel output, dita, hats, comparison, benefits"
last_updated: "July 16, 2016"
Resumen: "En esta sección te contamos los conocimientos que deberías adquirir antes de empezar a trabajar con APEX "
published: true
sidebar: mydoc_sidebar
permalink: mydoc_supported_features.html
folder: mydoc
---

Before you get into exploring Jekyll as a potential platform for help content, you may be wondering if it supports some basic features needed to fulfill your tech doc requirements. The following table shows what is supported in Jekyll and this theme.

## Conocimientos previos
Para empezar a trabajar con Oracle Application Express(APEX) es recomendable tener los siguientes conocimientos previos:

* Fundamentos de base de datos (Diseño de bases de datos por medio de un Modelo Entidad-Relación)
* SQL (Consultas básicas)
* Manejo de algún motor de base de datos (MySQL, Oracle, SQL Server de Microsoft, PostgreSQL, DB2, etc...)
* Fundamentos de HTML 
* Manejo de Linux (por consola)
* Git y Github (para el control de versiones y flujo de trabajo en equipo)
* JIRA (herramienta para la administración de tareas de un proyecto)


## Features not available

The following features are not available.

Features | Supported | Notes
--------|-----------|-----------
CMS interface | No | Unlike with WordPress, you don't log into an interface and navigate to your files. You work with text files and preview the site dynamically in your browser. Don't worry -- this is part of the simplicy that makes Jekyll awesome. I recommend using WebStorm as your text editor.
WYSIWYG interface | No | I use WebStorm to author content, because I like working in text file formats. But you can use any Markdown editor you want (e.g., Lightpaper for Mac, Marked) to author your content.
Different outputs | No | This theme provides a single website output that contains documentation for multiple products. Unlike previous iterations of the theme, it's not intended to support different outputs from the same content. However, you can easily set things up to do this by simply creating multiple configuration files and running different builds for each configuration file.
Robust search | No | The search feature is a simplistic JSON search. For more robust search, you should integrate Swiftype or Algolia. However, those services aren't currently integrated into the theme.
Standardized templates | No | You can create pages with any structure you want. The theme does not enforce topic types such as a task or concept as the DITA specification does.
Integration with Swagger | No | You can link to a SwaggerUI output, but there is no built-in integration of SwaggerUI into this documentation theme.
Templates for endpoints | No | Although static site generators work well with API documentation, there aren't any built-in templates specific to endpoints in this theme. You could construct your own, though.
eBook output | No | There isn't an eBook output for the content.

{% include links.html %}
