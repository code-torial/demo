In the previous step, we defined the click handler method `newImage`. How do we get this method to reload the image? We should call `getImageUrl` again, right?

The problem is that the URL returned from this method is always the same, so Vue will not re-render the page and nothing will happen!

To get around this, we're going to do something tricky and add a `date` parameter to the image URL and assign to it the current date and time as a timestamp. 

`date` is not an option of CATAAS but adding this unique value ensures that every call to `getImageUrl` returns a unique string.

Tasks:

1. After line 7 where we set the `height` parameter, set another parameter `date`. The value should be the current date as a timestamp which you can get by calling `Date.now()`.
2. In the `newImage` method, delete the console log and instead call `getImageUrl` again and assign the output to `imgUrl`. *Hint: remember it's a ref*.

With that done, the reload button will work!
