# initialTimeout

If the first element has not passed through this stage before the provided timeout, the stream is failed with a `TimeoutException`.

@ref[Time aware stages](../index.md#time-aware-stages)

@@@div { .group-scala }

## Signature

@@signature [Flow.scala]($akka$/akka-stream/src/main/scala/akka/stream/scaladsl/Flow.scala) { #initialTimeout }

@@@

## Description

If the first element has not passed through this stage before the provided timeout, the stream is failed
with a `TimeoutException`.


@@@div { .callout }

**emits** when upstream emits an element

**backpressures** when downstream backpressures

**completes** when upstream completes or fails if timeout elapses before first element arrives

**cancels** when downstream cancels

@@@

