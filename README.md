# TriangleBanner Library
![banner](https://cloud.githubusercontent.com/assets/8935913/25468181/3ba2296e-2ad1-11e7-8df9-3850ad1a7fca.png)
#### Description
The purpose of the this Javascript Library is to create a fast, and interesting option for a banner on websites. All of the project was done in pure javascript with no additional libraries needed.

#### How to use
To use the banner, you will need to include the banner and then create a new TriangleBanner object passing in the id of your canvas element. For example:

```HTML
<script type="text/javascript" src="TriangleBanner.min.js"></script>
<script>
	var Banner = new TriangleBanner("your-canvas-id");
</script>
```
It is that simple to have a banner autogenerate with all the default settings. The canvas object can be of any size and the triangles will generate the fit the entire canvas. You must wrap the canvas in an object such as:
```HTML 
<div style="width: 100%; height: 40%"></div>
```

#### Customizations
###### How to use customizations
To use customizations, it is relatively simple. All you will have to do is add attributes to the canvas tag, for example:
```HTML
<canvas id="canvas-id" outlineStyle=2 ></canvas>
```
This above will give the outlineStyle of 2 for the triangles. The following are all the options currently available:

###### outlineStyle
Outline style has 4 different options that you can use, which modify the line width of the canvas. The following options are available:
- 1 (default)
- 2 
- 3
- 4

###### quality
This determines the quality of the triangles. It has 4 different options. Currently you have to manually assign the quality as it is defaults to 'High'. The options are:
- low
- med
- high (default)
- ultra

###### resize
This determines if the squares resize when the page is resized. This is off by default but you can turn it on by assigning 'true' for the value. The options are:
- true
- false (default)

###### triangleHeight
Triangle height is how you decide on the height of the triangle. They way it is calculated is 1/x of the height of the canvas, so if you passed in 16 the height of a triangles will range between 1/16th and 1/18th the canvas height (the upper range is always 2 more than the number passed in). The default is 6.

###### triangleWidth
Triangle width is how you decide on the width of the triangle. They way it is calculated is 1/x of the width of the canvas, so if you passed in 16 the width of a triangles will be 1/16th. The default is 6.

###### color
The color options lets you select the color of the randomly generated triangles. Currently you can select from the following options:
- blue <br/>
![blue](https://cloud.githubusercontent.com/assets/8935913/25468077/541a2240-2ad0-11e7-9d33-e9806489dfe7.png)
- brown <br/>
![brown](https://cloud.githubusercontent.com/assets/8935913/25468178/3b9dafce-2ad1-11e7-9edd-957478486a7f.png)
- gray <br/>
![gray](https://cloud.githubusercontent.com/assets/8935913/25468174/3b8e06a0-2ad1-11e7-84be-39e67c1f903f.png)
- green <br/>
![green](https://cloud.githubusercontent.com/assets/8935913/25468177/3b8eca18-2ad1-11e7-8512-cd1d7bd9d8e7.png)
- orange <br/>
![orange](https://cloud.githubusercontent.com/assets/8935913/25468175/3b8e400c-2ad1-11e7-8f5d-61843c19e275.png)
- pink <br/>
![pink](https://cloud.githubusercontent.com/assets/8935913/25468172/3b8c2a9c-2ad1-11e7-8631-9a680c7607a0.png)
- purple <br/>
![purple](https://cloud.githubusercontent.com/assets/8935913/25468173/3b8de8fa-2ad1-11e7-97d5-727878d2da46.png)
- red <br/>
![red](https://cloud.githubusercontent.com/assets/8935913/25468176/3b8e29b4-2ad1-11e7-99a7-68850d05ab15.png)
- white <br/>
![white](https://cloud.githubusercontent.com/assets/8935913/25468179/3b9eef7e-2ad1-11e7-97f5-52690e22c431.png)
- yellow <br/>
![yellow](https://cloud.githubusercontent.com/assets/8935913/25468180/3b9ef2b2-2ad1-11e7-8786-59da66ceb0be.png)

Those are the base options, you can customize the color more by passing in multiple colors with a '-' separated list, for example:
```HTML
<canvas id="canvas-id" color=red-green ></canvas> 
```
###### animation
There are currently 4 different animations that are built in to the library by default, the different options are:
- 1, a random movement effect <br />
![anim1](https://cloud.githubusercontent.com/assets/8935913/25506239/deea239c-2b62-11e7-8dcf-71e10452c282.gif)
- 2, a wave effect from right to left <br />
![anim2](https://cloud.githubusercontent.com/assets/8935913/25506238/dee6d840-2b62-11e7-8cdf-ab4320f36bf2.gif)
- 3, a wave effect with a color changing effect also <br/>
![anim3](https://cloud.githubusercontent.com/assets/8935913/25506232/ded44ebe-2b62-11e7-869b-945a311111cc.gif)
- 4, a pure color changing effect from right to left <br />
![anim4](https://cloud.githubusercontent.com/assets/8935913/25506234/dee2fd38-2b62-11e7-9bda-5ccfc36f9e2a.gif)
- 5, a wave with a fading color change <br />
![anim5](https://cloud.githubusercontent.com/assets/8935913/25506235/dee5b866-2b62-11e7-8c4c-b1f53f759628.gif)
- 6, a wave with a non-fading color change <br />
![anim6](https://cloud.githubusercontent.com/assets/8935913/25506237/dee5f9ca-2b62-11e7-9953-631feda7947c.gif)
    
###### animationColors
Animation colors are used when use select animation 3 & 4 as it is the color changing animation. The same colors are available from the 'color' list, and you can use multiple colors also.

###### animationSpeed
This is a option to let you select the animation speed for the different animations, all of the animations have a default speed but
you can override the default with this option. This option sets the interval speed in ms.


#### Development
Currently this product is still in development and should get more features as it moves along.

#### License
Copyright 2017 Mitchell Woodhouse Mckenzie

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

![bottom](https://cloud.githubusercontent.com/assets/8935913/25506236/dee5e570-2b62-11e7-9d72-987d82b918e1.png)
