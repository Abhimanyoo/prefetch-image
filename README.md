# prefetch-image
Prefetch all images for your web app, especially for mobile/h5 promotion pages.

## Usage

`npm install prefetch-image --save` or
`yarn add prefetch-image`

```javascript
const prefetchImages = require('prefetch-image');
//or
//import prefetchImages from 'prefetch-image';

const images = [
  '/1.png',
  '/2.jpg',
  '/3.png',
];
prefetchImages(images, options)
  .then((result) => {
    //result is an array containing all the "Image" objects
    console.log('all images loaded!');
    //start init your page logic...
  });
```

### Options

*concurrency*: number of images be loading concurrently, default: 6

## LICENSE

MIT
