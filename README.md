# Publicly Open Mapping Files

POMF is a set of open, unencumbered Minecraft mappings, free for everyone to use under the Creative Commons Zero license. The intention is to let 
everyone mod Minecraft freely and openly, while also being able to innovate and process the mappings as they see fit.

The current version targets Minecraft version **18w49a**.

## Contributing

Please remember that copying and pasting mappings from alternate projects under more restrictive licenses (such as MCP) is **completely forbidden** without explicit permission from the 
owners of said mappings. Discussing the naming approaches used in said projects is also not welcome - you have been warned.
However, it is a good idea to consult name changes with other people - use pull requests or our community spaces to ask questions!

### Getting Started

1. Fork and clone the repo
2. Run `./gradlew pomf` (Linux, macOS) or `gradlew pomf` (Windows)
3. Profit

## Gradle

POMF uses Gradle to provide a number of utility tasks for working with POMF.

### `download`
Downloads the client and server Minecraft jars for the current Minecraft version to `.gradle/minecraft`

### `mergeJars`
Merges the client and server jars into one merged jar, located at `VERSION-merged.jar` in the POMF directory where `VERSION` is the current Minecraft version.

### `setupPomf`
`download` and `mergeJars`

### `pomf`
`setupPomf` and download and launch the latest version of Enigma automatically configured to use the merged jar and the mappings.
