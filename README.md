# IM
#author -kst 
#project time taken : 12/13/2022 -12/15/2022
#This code is defining a number of functions for preloading, swapping, and restoring images in a webpage. The code uses the MM_ prefix for its function and variable names, which was a convention used in older versions of the Macromedia Dreamweaver web development software.

#The MM_preloadImages function is used to preload a set of images so that they will be ready for use when needed. This can improve the performance of the webpage by avoiding delays caused by loading the images on demand. The function takes a list of image URLs as arguments and creates a new Image object for each URL. It then sets the src property of each Image object to the corresponding URL, which causes the browser to begin loading the image.

#The MM_swapImgRestore function is used to restore the original src values for all images on the page that have been swapped using the MM_swapImage function. This can be useful if the src values of the images have been changed to show a hover or active state, and the images need to be reset to their original state.

#The MM_findObj function is used to find an element with the given name or ID in the current document. The function first looks for the element using the document.all collection, and then it looks for the element in each of the forms and layers collections in the document. If the element is not found in any of these collections, the function uses the getElementById method to search for the element by its ID. The function returns the element if it is found, or null if it is not found.

#The MM_swapImage function is used to swap the src value of one or more images on the page with a different value. The function takes a list of arguments, where the first argument is the name or ID of the image element to be swapped, the second argument is the new src value to use, and the remaining arguments are additional image/src pairs to be swapped. The function uses the MM_findObj function to find each image element and then sets its src value to the corresponding new value. The function also saves the original src values of the swapped images in the MM_sr array, so that they can be restored later using the MM_swapImgRestore function.

#The code also includes some additional logic for preloading the images when the page loads and for setting up event handlers to automatically call the MM_swapImage and MM_swapImgRestore functions when the user moves the mouse over or out of an image.
