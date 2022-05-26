.. cognite-sdk documentation master file, created by
   sphinx-quickstart on Thu Jan 11 15:57:44 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Cognite Python SDK Documentation
================================

This is the Cognite Python SDK for developers and data scientists working with Cognite Data Fusion (CDF). The package is tightly integrated with pandas, and helps you work easily and efficiently with data in Cognite Data Fusion (CDF). 

.. contents::
   :local:

Installation
^^^^^^^^^^^^
To install this package:

.. code-block:: bash

   <dependency>    
    <groupId>com.cognite</groupId>
    <artifactId>cdf-sdk-java</artifactId>
    <version>1.15.0</version>
   </dependency>

This is just a copy paste from the repository

.. code-block:: bash
   
   // Create the Cognite client using API key as the authentication method
   CogniteClient client = CogniteClient.ofKey(<yourApiKey>)
   .withProject("myCdfProject")
   .withBaseUrl("https://yourBaseURL.cognitedata.com");  //optional parameter
        
   // ... or use client credentials (OpenID Connect)
   CogniteClient client = CogniteClient.ofClientCredentials(
        <clientId>,
        <clientSecret>,
        TokenUrl.generateAzureAdURL(<azureAdTenantId>))
        .withProject("myCdfProject")
        .withBaseUrl("https://yourBaseURL.cognitedata.com"); //optional parameter     
      

To install with pandas, geopandas and shapely support (equivalent to installing `cognite-sdk`).
However, this gives you the option to only have pandas (and NumPy) support without geopandas.

.. code-block:: bash

   pip install cognite-sdk-core[pandas, geo]


Contents
^^^^^^^^
.. toctree::
   cognite

Examples
^^^^^^^^
For a collection of scripts and Jupyter Notebooks that explain how to perform various tasks in Cognite Data Fusion (CDF) using Python, see the GitHub repository `here <https://github.com/  cognitedata/cognite-python-docs>`__.