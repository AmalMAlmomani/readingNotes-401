# Redux - Asynchronous Actions

  - Thunk middleware for Redux.

## What is React Suspense?
  - Suspense is a new React feature that was announced recently at the JSConf Conference in Iceland.
  - It aims to help with handling async operations respectively in regard to CPU power and data fetching.

## Why React Suspense?
  - There’s a good chance you’ve come across SPAs that make use of a loading icon as an indicator that data is being fetched
  - This is a common method used to ensure good UX for apps that are fetching data from external sources.
  - All you have to do is check if the data has been successfully fetched, and if not, show a spinner.


## The key module that makes Suspense work is the createFetcher function. Available on npm as the simple-cache-provider, it works as outlined below:

   - In the render() method, read a value from the cache
   - If the value is already cached, the render continues like normal
   - If the value is not already cached, the cache throws an error
   - When the promise resolves, React continues from where it stopped


