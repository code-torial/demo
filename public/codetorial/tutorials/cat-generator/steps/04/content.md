Let's now get the "Moar plz" button working (line 25). This will reload the cat image and show a new one.

To do this, we'll first create a click handler method. We'll then bind this method to the click event of the button in the template. We'll then use this method to reload the image.

Tasks:

1. In the `setup` function, create a method `newImage`. In the function body, log a message to the console "clicked".
2. Return the `newImage` method from `setup` so it can be used in the template.
3. Bind `newImage` to the button's click event.

With that done, clicking the button will call the `newImage` method which will log a message to the console.
