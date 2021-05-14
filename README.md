## Image processing API
- Resize any jpg image by setting its name and the desired width and height as parameters in the URL.
- The image created will have the same name as the original, and the width and height chosen, for easy identification.
- If an image with the width and height chosen has already been created, the server responds with the existing image, instead of processing it again.

### To run on local
- Download the project
- Run ```npm install```

### How to use it
- Run ```npm run build```
- Set the image you want to resize under ```build/assets/originals``` (The file must be a .jpg)
- Start the app with ```node build/.```
- Go to ```http://localhost:3000/api/images```
- Set the name of the image (filename) and the desired width and height as parameters in the URL, for example: ```http://localhost:3000/api/images?filename=santamonica&width=400&height=400```
- You'll get the resized image in the browser, and you can see it as well under ```build/assets/thumbnails```