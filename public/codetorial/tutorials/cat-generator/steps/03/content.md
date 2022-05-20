So how do we get a cat image from CATAAS? Quite simply, we use the URL `https://cataas.com/cat` and a random image will be returned. 

However, we can also add search parameters to the URL to further specify what we want. For example, `https://cataas.com/cat?width=300` will return a cat image with a width of 300. 

*You can see the full set of options for CATAAS [here](https://cataas.com/#/).*

Let's now properly define the `getImageUrl` function so that it creates an image URL for use with CATAAS. 

1. On the first line of `getImageUrl`, create a variable `url` and assign to it a new instance of the native JavaScript interface [URL](https://developer.mozilla.org/en-US/docs/Web/API/URL). The argument should be the CATAAS base URL `https://cataas.com/cat`. *Hint: use the `new` keyword as `URL` is a constructor*.
2. Use the `set` method of the `searchParams` property of the `url` object to set a `width` of `300`.
3. Repeat 2 and also set a `height` of `300`.
4. Return a string containing the whole url from `getImageUrl`. *Hint: use the `toString` method of the url*. 

With that done, you should now see a random cat image in the page!
