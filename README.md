transapi-client
===============

The client library for the TransAPI API for MCServer.

Installation
------------

 1. Copy transapi.lua into your plugin folder.
 2. Create a directory in your plugin folder called `languages`.
 3. Create a file named [whatever].lua in the languages directory, and add translations to it as per the examples file.
  Your should probably have languages in their own files.

API
---

GetTranslation( Slug (string), cPlayer ) - Returns the translated string for the provided cPlayer object.
GetConsoleTranslation ( Slug (string) )  - Returns the translated string for the console.

Pitfalls
--------

 * TransAPI should not be used for startup logging, as it requires the TransAPI helper plugin to be loaded before yours.
 * TransAPI requires that the global var `g_Languages` is not defined or used outside of itself.

Licensing
---------

The TransAPI client lib is licensed under the MIT license, so you are free to improve and build upon it.
