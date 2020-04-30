# MergedSpawnrAPI

This API resource allows your plugin to find out the details of merged spawners, which are created by MergedSpawner plugin. 
If you're a plugin developer, you can add this resource in your dev environment to add the integration of MergedSpawner function into your plugin without purchasing MergedSpawner.

## Using maven repository
`MergedSpawnerAPI` is hosted on TeamVK's public maven repository and you can reference it in your dev environment.

### Gradle
Here is an example of a fragment of the script you can add to your build.gradle.

```
plugins {
    id "com.github.unafraid.gradle.git-repo-plugin" version "2.0.4.1"
    id "java"
    id "maven-publish"
}

// this will allow you to use github() to specify the github hosted maven repository
apply plugin: "com.github.unafraid.gradle.git-repo-plugin"

repositories {
    jcenter()
    mavenCentral()
    github("teamvk", "maven-repository", "origin", "master", "release")
}

dependencies {
    // ... other dependencies
    compile group: 'org.spigotmc', name: 'spigot', version: spigot_version
    compile group: 'com.vk2gpz.mergedspwner', name: 'MergedSpawenrnAPI', version: '12.4.8'
    // ... other dependencies
}
```

## [API Documentation](javadoc/index.html)

## [Donation](http://PayPal.Me/vk2gpz)
It would be greatly appreciated for your donation to continue providing support for this plugin.
