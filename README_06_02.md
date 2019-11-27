# Important: Now you can see a pattern:
1. Launch a coroutine that runs on the main or UI thread, because the result affects the UI.
2. Call a suspend function to do the long-running work, so that you don't block the UI thread while waiting for the result.
3. The long-running work has nothing to do with the UI. Switch to the I/O context, so that the work can run in a thread pool that's optimized and set aside for these kinds of operations.
4. Then call the database function to do the work.
