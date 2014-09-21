### OperationalKeyValue

Demonstrates observing a current NSOperation class.

NSOperation subclass uses simple, synthesized accessors for `executing` and `finished`. But for `NSOperation` to function properly (i.e. to be properly released when done, to honor dependencies, to honor `maxConcurrentOperationCount`, etc.), it is also important that this subclass issue the `isExecuting` and `isFinished` notifications as outlined in the documentation.