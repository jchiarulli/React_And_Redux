# Single Page Apps

- React apps are typically SPA's
- Only ever one HTML page served to the browser
- React then controls what a user sees on that page
- Doesn't mean app consists of only a single page means that only one page is served to the browser from the server at any given time
- Make the initial request to the server with index.html as the equest to get the initial page
- Once the response from the server is received React takes over the application and if we go to a different page then React intercepts the request and handles it by loading in the corresponding component
- This removes additional requests to the server and makes the app quicker and slicker
- Showing different components to the user depending on their actions all on the frontend

## Multi Page Apps

- User typically goes to an address which sends a request to the server then the server looks at the url and sends back a response containing the html page containing the provided url
- When the user goes to a different address an additional request is made the server looks at the url and sends back the corresponding html page
