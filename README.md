# Interpreted Build (BLD.4dbase)

## Description

The BLD component facilitates automatic building of interpreted components. 4D's built-in build feature only supports the creation of compiled components. Of course, "building" an interpreted component is really just a file copy but this component takes care of some other actions that might be referred to as "build automation":

* Launched from within 4D.
* Remove previous build.
* Copy Resources and Macros to output folder, if any.
* Simple versioning system based on the [Design Object Access](http://doc.4d.com/4Dv13.1/help/Title/en/page2577.html) "stamp".

## Contents

* The [Components](interpreted-build/tree/master/Components) folder contains the interpreted component suitable for installation in any [4D v13](http://www.4d.com/products/4dv13.html) database.
* The [Plugins](interpreted-build/tree/master/Plugins) folder contains the required plug-in to complete a build.
* The [matrix](interpreted-build/tree/master/matrix) folder contains the component source code.
* The [doc](interpreted-build/tree/master/doc) folder contains documentation about the component.

## Usage

You must install both the component and MISC I plug-in in order for the build to work correctly.

Execute the shared method "BLD_Build" to build your project.

If you modify the matrix database, you should build a new component.  To build a new component, execute the BLD_Build method from within the matrix database (MISC I is already installed in the matrix database).

If you would like to include BLD.4dbase in a 4D project managed on github, consider using the component-only repository instead.

## Known Issues

None.