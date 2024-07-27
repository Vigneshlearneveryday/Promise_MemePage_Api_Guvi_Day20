# Promise Task -1 
***
## Meme page Delivered through the Given Options of API
Web Service Endpoint: https://memedrills.netlify.app

A Promise is a native JavaScript object that represents the eventual result of an asynchronous operation. Promises can be in one of three states:
- **Pending**: The initial state; neither fulfilled nor rejected.
- **Fulfilled**: The operation completed successfully.
- **Rejected**: The operation failed.

## Example Code

Here’s a simple example of how to create and use a Promise:

```javascript
// Create a new Promise
const myPromise = new Promise((resolve, reject) => {
  // Simulate an asynchronous operation
  setTimeout(() => {
    const success = true; // Change to false to simulate failure
    if (success) {
      resolve('Operation succeeded!');
    } else {
      reject('Operation failed.');
    }
  }, 1000);
});

// Handle the Promise
myPromise
  .then((result) => {
    console.log(result); // 'Operation succeeded!'
  })
  .catch((error) => {
    console.error(error); // 'Operation failed.'
  });
