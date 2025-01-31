//[buildless-plugin-gradle](../../../../index.md)/[build.less.plugin.gradle](../../index.md)/[BuildlessExtensionAPI](../index.md)/[RemoteCacheSettings](index.md)

# RemoteCacheSettings

interface [RemoteCacheSettings](index.md) : [BuildlessExtensionAPI.CacheSettings](../-cache-settings/index.md)

###  Remote Cache Settings

Specifies settings which configure Gradle's remote build cache; these may be provided in lieu of settings specified directly with Gradle, and are preferred over directly specifying settings. By default, the remote build cache is enabled in all circumstances.

Push of objects is enabled by default. Object push (uploading to the cache) can be disabled by setting [push](push.md) to `false`, or by using any of the condition builders specified by the [MutableCacheSettings](../-mutable-cache-settings/index.md) or [MutableRemoteCacheSettings](../-mutable-remote-cache-settings/index.md) types.

#### Inheritors

| |
|---|
| [MutableRemoteCacheSettings](../-mutable-remote-cache-settings/index.md) |

## Properties

| Name | Summary |
|---|---|
| [enabled](../-cache-settings/enabled.md) | [JVM (Gradle)]<br>abstract val [enabled](../-cache-settings/enabled.md): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Indicates whether a given cache sub-system should be enabled or disabled (either a local cache or remote cache). If a caching sub-system is &quot;disabled,&quot; it is not used *at all* for the current build. |
| [push](push.md) | [JVM (Gradle)]<br>abstract val [push](push.md): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Whether build outputs will be uploaded to the cache as needed; enabled by default. |
