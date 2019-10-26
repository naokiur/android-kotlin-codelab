When your app has complex view hierarchies, findViewById() is expensive and slows down the app, because Android traverses the view hierarchy, starting at the root, until it finds the desired view.
