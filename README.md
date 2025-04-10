1. Proxy Pattern – Homework

What problem has been solved?
The problem was optimizing the loading of high-resolution images for the real estate agency's website. 
Without a proxy, each image would load at once, which would slow down the site dueto the large amount of data. 
The proxy allows you to display thumbnails immediately, and full images are uploaded only when necessary.

How did the template simplify or optimize the design?
The Proxy template shares responsibility:
ImageProxy manages access and deferred loading, while HighResolutionImage is responsible for working with the image itself. 
This reduces memory consumption and speeds up the initial loading of the page. Adding a Protected Image Proxy enhances security by limiting image uploads to authorized agents only.


2. Flyweight Pattern – Homework

What problem has been solved?
The problem was excessive memory consumption when creating thousands of markers with repeating styles (icon, color). 
Without the Flyweight template, each marker would store its own style data, which would lead to duplication and inefficient use of resources.

How did the template simplify or optimize the design?
The Flyweight template divides data into internal (common styles in MarkerStyle) and external (unique coordinates and name in MapMarker).
The Marker Style Factory ensures that styles are created only once and reused, which reduces memory consumption and simplifies style management in the application.
