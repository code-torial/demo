Let's have a quick rundown of our `App.vue` component.

As you'll see, we have a reactive variable `imgUrl` (declared on line 6) which is bound to the `src` attribute of an `imgUrl` tag in the template (line 17). 

The `imgUrl` variable should be assigned a URL string of an image. We'll generate one from the CATAAS API over the next few lessons.

To complete this lesson, do the following:

1. Declare a function `getImageUrl` (put it above the component definition on line 4) and make it return an empty string
2. Make it so that the reactive variable `imgUrl` is initialized with a value returned from `getImageUrl`. *Hint: pass it to `ref`*. 
