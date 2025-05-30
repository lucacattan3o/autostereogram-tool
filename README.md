# Autostereogram Tool

An *autostereogram* is a two-dimensional image traditionally composed of a chaotic pattern repeated multiple times. With a little practice and the correct viewing technique, it is possible to make the hidden three-dimensional image emerge from within it.

![A screenshot of the Autostereogram Tool](/assets/imgs/doc/preview-rivers.png)

This tool allows you to generate autostereograms using:
- different types of depth maps.  
- different types of noise.

[Try it](https://lucacattan3o.github.io/autostereogram-tool/index.html) in your browser. It's also available on [metronimie.com](https://www.metronimie.com/tool/letternoise/).

It's developed in JavaScript and p5.js and it's based on a slightly modified version of the great library [Stereogram.js](https://github.com/tony-pizza/Stereogram.js).

## Credits

This tool is developed by [Mekit](https://www.mekit.it) within the project [Residenza Poietica 2024](https://www.metronimie.com/it/residenza-poietica-2024) for the artistic performance [Del nostro scavo continuo](https://www.metronimie.com/it/eventi/del-nostro-scavo-continuo-performance-di-restituzione-di-residenza-poietica-2024).

Developer: *[Luca Cattaneo](https://lucacattan3o.github.io/)*  
Artists: *Emanuele Caprioli, Caterina Dufì and Simone Spampinato*  
Artistic Direction: *Amalgama*  
Design e Project Management: *Alice Turina*

## How to use it

Use the controls on the right panel to generate an autostereogram. 
Below is some information on how to use the various panels.

### Canvas

Set the *Width* and *Height* of image you want to produce. Rember that a wide format is more suitable for an autosteoreogram.  
These settings will affect both the depth map and the autostereogram.

You can use the *Multiply* option to scale your output.

### Depth Map

The *Depth Map* is the grayscale image that will be used in the generation of the autostereogram. 
The brightness of each pixel indicates its relative distance; brighter pixels are closer, and darker pixels are farther away. 

You can choose between four types of depth map generation:

#### 1. Rivers
Edit the various parameters to obtain the generation of different types of rivers.

[![A depth map generated with the rivers mode](/assets/imgs/doc/depth-map-rivers.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/depth-map-rivers.png)


#### 3. Image
Use this mode to upload a custom *Depth Map Image* like this one.

[![An example of a custom depth map loaded as an image](/assets/imgs/doc/depth-map-image.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/depth-map-image.png)

#### 4. Paint
Use this mode to paint the *Depth Map* with your mouse. Change the brush color to draw at different depth levels.

[![A painted depth map](/assets/imgs/doc/depth-map-paint.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/depth-map-paint.png)

#### Well
This mode creates a specific number of concentric circles at different depths.

[![Depth map: concentric circles with varying brightness at the center of the sheet, indicating different depths](/assets/imgs/doc/depth-map-well.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/depth-map-well.png)

If you struggle visualizing autostereograms, use the *Well* mode to generate a small figure in the center, this will help you.

[![Depth map: small concentric circles with varying brightness at the center of the sheet, indicating different depths](/assets/imgs/doc/depth-map-well-easy.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/depth-map-well-easy.png)

*Rivers* and *Well* mode were used to generate the outputs for the artistic performance.

### Autostereogram Generation

In the *Autostereogram* panel you can choose the type of noise you want for the pattern and actually generate it with the **Generate Autostereogram** button (or the *g* key on the keyboard). 

Noise types:

#### 1. SIRD
The pattern is generated using random dots. This is the best performing pattern: it makes the autostereogram easier to see because it is rich in details.

[![An autostereogram generated using a rivers-type depth map in SIRD mode](/assets/imgs/doc/sird-rivers-as.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/sird-rivers-as.png)

This autostereogram was generated using a rivers-type depth map.


#### Perlin Noise
This pattern is generated using the p5.js perlin noise. It performs well and it is quite easy to see the autostereogram.

[![An autostereogram generated using an image depth map with perlin noise](/assets/imgs/doc/as-perlin-noise-image.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-perlin-noise-image.png)

#### Perlin Noise Sinusoidal
This noise is an evolution of the previous one, it uses perlin noise in combination with the sin() function of p5.js.

[![An autostereogram generated using the well-mode depth map with perlin noise sinusoidal](/assets/imgs/doc/as-sinusoidal-well.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-sinusoidal-well.png)

#### Worley Noise
A procedural texture generated by calculating the distance to a set of randomly distributed feature points. Play with the Noise Scale parameter to create cellular or granular patterns.

[![An autostereogram generated using a painted depth map with worley noise](/assets/imgs/doc/as-worley-paint.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-worley-paint.png)

#### Vertical Lines

Using this pattern you can get very particular geometric visuals, the depth map is not completely hidden but the autostereogram works correctly.

[![An autostereogram generated using a painted depth map with vertical lines pattern](/assets/imgs/doc/as-vertical-paint.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-vertical-paint.png)

#### Letter Noise
A pattern composed of text that is repeated many times until it forms a dense network of words.

[![An autostereogram generated using a well depth map with letter noise](/assets/imgs/doc/as-letter-well-1.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-letter-well-1.png)

In addition to changing the colors, you can reverse the order of the palette using the *Invert Colors* option in any noise types.

[![An autostereogram generated using a well depth map with letter noise](/assets/imgs/doc/as-letter-well-2.png)](https://raw.githubusercontent.com/lucacattan3o/autostereogram-tool/main/assets/imgs/doc/as-letter-well-2.png)


The **Invert Depth Map** option in autostereogram generation reverses the perceived depth. Areas that were designed to appear protruding will recede, and vice versa. This allows for creative control over the 3D effect and can be useful for specific visual outcomes.

In the **Advanced Panel** you can change the way the autostereogram is built: the default values are fine but you're free to experiment.

## Tips for viewing autostereograms

The easiest way to view an autostereogram is to get very close to the paper (or screen), cross your eyes, and slightly blur your vision. 

Slowly moving the autostereogram away, you will begin to perceive something peculiar, unusual; at that moment, with a bit of concentration, it will be possible to focus on the emerged 3D image and move it in space.

Some people, however, manage to view them using parallel viewing; it takes some time and practice to perfect your technique.

