# CurseGradle

> This is a fork of [CurseGradle](https://github.com/matthewprenger/CurseGradle) by [matthewprenger](https://github.com/matthewprenger).

A gradle plugin for publishing artifacts to [CurseForge](https://www.curseforge.com/).

## Simple Quickstart

For more information red the [wiki of the original project](https://github.com/matthewprenger/CurseGradle/wiki/).

```gradle
plugins {
    id 'de.maxhenkel.cursegradle' version '<VERSION>'
}

curseforge {
  apiKey = '123-456' // This should really be in a gradle.properties file
  project {
    id = '12345'
    changelog = 'Changes' // A file can also be set using: changelog = file('changelog.txt')
    releaseType = 'beta'
  }
}
```
