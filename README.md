# MDG branch of ForgeDevEnv

A modified version of [CleanroomMC/ForgeDevEnv](https://github.com/CleanroomMC/ForgeDevEnv) with some QoL improvements.

# Differences from RFG branch

The fork keeps the upstream `net.neoforged.moddev.*` plugin ids but is published to Maven Central as
`io.github.ruixuqi:moddev-gradle` rather than to the Gradle Plugin Portal, so `settings.gradle` points those ids at it.
May have issues; report them [here](https://github.com/RuiXuqi/ModDevGradle).

No more `rfg.deobf` or `fg.deobf`. Use `modImplementation` `modCompileOnly` `modRuntimeOnly` for remapping, and plain
`implementation` for libraries that must not be remapped.

For IntelliJ users, it is recommended to switch
to [RuiXuqi/MinecraftDev](https://github.com/RuiXuqi/MinecraftDev/releases) for AT completion. Also RFG and Unimined
support have been merged there.
