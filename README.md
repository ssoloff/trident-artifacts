# trident-artifacts

The [Trident](https://github.com/kirill-grouchnikov/trident) animation library artifacts

The purpose of this project is simply to publish various Trident animation library artifacts to a public repository so they can be easily used by dependent projects.

## Usage

By default, the Trident animation library primary artifact is published (e.g. _trident-<version>.jar_).  For example, to publish version 1.4.00 of the Trident animation library primary artifact to Bintray, use the following command:

    $ ./gradlew -Pversion=1.4.00 bintrayUpload

The secondary artifacts may be published by specifying the `packageName` project property.  For example, to publish version 1.4.00 of the Trident animation library tst artifact to Bintray, use the following command:

    $ ./gradlew -PpackageName=tst -Pversion=1.4.00 bintrayUpload
