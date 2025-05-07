# Autostereogram Tool

This tool allows you to generate autostereograms using:
- different types of depth maps.  
- different types of noise.

[Try it](https://lucacattan3o.github.io/autostereogram-tool/index.html) in your browser.

It's developed in JavaScript and p5.js and it's based on a slightly modified version of the great library [Stereogram.js](https://github.com/tony-pizza/Stereogram.js).

## Credits

This tool is developed by [Mekit](https://www.mekit.it) within the project [Residenza Poietica 2024](https://www.metronimie.com/it/residenza-poietica-2024) for the performance [Del nostro scavo continuo](https://www.metronimie.com/it/eventi/del-nostro-scavo-continuo-performance-di-restituzione-di-residenza-poietica-2024).

Developer: *[Luca Cattaneo](https://lucacattan3o.github.io/)*  
Artists: *Emanuele Caprioli, Caterina Dufì and Simone Spampinato*  
Artistic Direction: *Amalgama*  
Design e Project Management: *Alice Turina*

## How to use it

Use the controls on the right panel to generate an autostereogram. 
Below is some information on how to use the various panels.

### Canvas

Set the *Width* and *Height* of image you want to produce. Rember that a wide format willis more suitable for an autosteoreogram.  
These settings will affect both the depth map and the autostereogram.

You can use the *Multiply* option to scale your output.

### Depth Map

The *Depth Map* is the grayscale image that will be used in the generation of the autostereogram. 
The brightness of each pixel indicates its relative distance; brighter pixels are closer, and darker pixels are farther away. 

You can choose between four types of depth map generation:

- **Rivers**: edit the various parameters to obtain the generation of different types of rivers.

- **Image**: use this mode to upload a custom *Depth Map Image* like [this one](https://upload.wikimedia.org/wikipedia/commons/8/82/Esempio_di_Depth_Map.jpg).

- **Paint**: Use this mode to paint the *Depth Map* with your mouse. Change the brush color to draw at different depth levels.

- **Well**: This mode creates a specific number of concentric circles at different depths. If you are struggle visualizing autostereograms, use the *Well* mode to generate a small figure in the center, this will help you.

*Rivers* and *Well* mode were used to generate the outputs for the artistic performance.

### Stereogram Generation

Coming soon

#### Advanced Panel

Coming soon

## Tips for viewing autostereograms

Coming soon

