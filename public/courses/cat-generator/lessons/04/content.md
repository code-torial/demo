Let's now get the "Moar plz" button working (line 25). This will reload the cat image and show a new one.

To do this, we'll create a method in our `setup` function, then bind this method to the click event of the button in the template.

Tasks:

1. In the `setup` function, create a method `newImage`.
2. Return the `newImage` method from `setup` so it can be used in the template.
3. Bind `newImage` to the button's click event.

With that done, clicking the button will call the `newImage` method.

How do we get this method to reload the image? It seems like we should probably call `getImageUrl` again. The problem is that the URL returned from this method is always the same, so Vue will not re-render the page and nothing will happen.

Instead, we're going to do something tricky and add a `date` parameter to the image URL and assign to it the current date and time as a timestamp. This ensures that every call to `getImageUrl` returns a unique string.

Tasks:

1. After line 7 where we set the `height` parameter, set another parameter `date`. The value should be the current date as a timestamp which you can get by calling `Date.now()`.
2. In the `newImage` method, call `getImageUrl` again and assign the output to `imgUrl`.

Now, the reload button will work!
