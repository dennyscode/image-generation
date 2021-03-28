# Image-Generation

## What´s it
This is a test repository for checking out ![Node-Html-To-Image](https://github.com/frinyvonnick/node-html-to-image)

## What it does
This package (Node-HTML-To-Image) is a simple and working tool to achieve the following tasks:
* Serverside Image Creation
* Dynamic Inputs
* Styling based on CSS
* Markup based on HTML

## How to use

1. Fill dynamic data within:
  * ```javascript
    content.js:
    
    {
        "you": "denny"
    }

  ```
  
2. Markup and Styling within:
  * ```HTML
    index.html:
    
    <!DOCTYPE html>
    <html>
        <head>
            <!-- Do the styling using internal CSS -->
            <style>
                body {
                background-color: linen;
                color: green;
                width: 400px;
                height: 800px;
                }

                .card {
                    border-radius: 15px;
                    background-color: pink;
                }

                h1 {
                color: maroon;
                margin-left: 40px;
                }
                </style>
        </head>
      <!-- Do the Markup using HTML within body -->
      <body>
        <div class="card">
            <h1>Hello {{you}}</h1>
        </div>
      </body>
    </html>

  ```
  
  3. Run the script:
  * ```javascript
    run the following in cli:
    
    npx node-html-to-image-cli ./index.html ./image.png --content ./content.json
    (feed the script using the html-file, output-filename (optional dynamic) and if dynamic add json)
  ```
  
  ## Output
  image.png will be created in the root folder
  
  
  ## For more Information, check:
* ![Generate images from HTML in Node.js](https://dev.to/yvonnickfrin/generate-images-from-html-in-node-js-8p5)
* ![node-html-to-image v1.2 is out 🎉](https://dev.to/yvonnickfrin/node-html-to-image-v1-2-is-out-42f4)
* ![.. or the Repo: Node-Html-To-Image](https://github.com/frinyvonnick/node-html-to-image)

Thanks to ![Yvonnick FRIN](https://github.com/frinyvonnick)
