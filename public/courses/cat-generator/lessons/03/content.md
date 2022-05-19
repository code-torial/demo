Let's now write the `getImageUrl` function. The job of this function is to create an image URL for use with CATAAS.

To get a random cat image from CATAAS we can simply use the URL `https://cataas.com/cat`. However, we can also add search parameters to the URL to further specify what we want.

For example, we could use the url `https://cataas.com/cat?width=300` to get images with a width of 300. You can see the full set of options [here](https://cataas.com/#/).

Tasks:

1. Use the native JavaScript `URL` interface to create a URL object on the first line of `getImageUrl` and assign it to a variable `url`. *Hint: use the `new` keyword as `URL` is a constructor.
2. Use the `set` method of the `searchParams` property of the url to set a `width` of `300` and a `height` of `300`
3. Return a string containing the whole url from `getImageUrl`. *Hint: use the `toString` method of the url*. 

With that done, you should now see a random cat image in the page!
