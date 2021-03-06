[com.github.salomonbrys.kodein](index.md) / [toProviderOrNull](.)

# toProviderOrNull

`inline fun <A, T : Any> `[`InjectedProperty`](-injected-property/index.md)`<(A) -> T>.toProviderOrNull(crossinline arg: () -> A): Lazy<() -> T>`

Transforms an injected nullable factory property into an injected nullable provider property by currying the factory with the given argument.

### Parameters

`A` - The type of argument the factory takes.

`T` - The type of object to retrieve.

`arg` - A function that provides the argument that will be passed to the factory.

**Receiver**
The injected factory to curry.

**Return**
An injected provider property that, when called, will call the receiver factory (if not null) with the given argument.

