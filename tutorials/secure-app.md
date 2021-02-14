---
title: Secure our first application using Keycloak Admin Console
description: This tutorial explains how to secure our first application using Keycloak Admin Console
---

Let’s try to secure our first application. 
First step is to register this application with your Keycloak instance. To do this follow below steps:


1. Open the Keycloak Admin Console

2. Click 'Clients'

3. Fill in the form with the following values:

  Client ID: myclient
  Client Protocol: openid-connect
  Root URL: https://www.keycloak.org/app/

4. Click Save

5. Open https://www.keycloak.org/app/. Change Keycloak URL to the URL of your Keycloak instance. Click Save.

6. Now you can click Sign in to authenticate to this application using the Keycloak server you started earlier.