All of our app code exists in the `App.vue` component which you should currently see in the editor.

Note that there is a reactive variable `imgUrl` (declared on line 6) bound to the `src` attribute of an `imgUrl` tag in the template (line 17). 

To display a cat image, `imgUrl` should be assigned a URL string. We'll generate one using CATAAS over the following steps.

To complete this step, do the following:

1. Declare a function `getImageUrl` (put it above the component definition on line 4) and make it return an empty string
2. Make it so that the reactive variable `imgUrl` is initialized with the string returned from `getImageUrl`. *Hint: pass it to `ref`*. 
