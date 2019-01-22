 #Progress Bar
 
 ##This is a simple progress bar on page load, this is important when working ajax on your page

 ```js  // it is a good practice to define the progresser at the begin' of the script, and use the method loader in the whole script anywhre you need it;
   /*... TIP: You can passe a string color as the background color of the container, e.g,let progresbar = new Progresser("#fff"); default is white+transparence of 0.5 in rgba */ 
  let progresbar = new Progresser(); 
  // the progresser returns a resolved promise
  let promise = Promise.resolve();
  // passe the loader to the button click Event
  document.querySelector("button").addEventListener("click",()=>{
  // the promise is rosolved
  promise.then(()=>{
  // loader takes 1 parameter wich are numbers that are in milleseconds for the progressbar duration
  progresbar.loader(1000);})
});```