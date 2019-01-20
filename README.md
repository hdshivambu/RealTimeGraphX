# RealTimeGraphX
RealTimeGraphX is a data type agnostic, high performance plotting library for WPF, UWP and soon, Xamarin Forms.

The library core components are built using .Net Standard which makes it portable to a range of platforms.

Typical use case is, scientific measurements applications which requires real-time display with large data volumes.

RealTimeGraphX has a number of built-in data point types (axis) like Double, Float, Int32 and TimeSpan, but you can easily implement any kind of custom data type by inheriting and implementing the mathematical logic for that type.

<br/>
<hr/>
<br/>

The solution contains demo projects for WPF and UWP.

*Single Series*

![alt tag](https://github.com/royben/RealTimeGraphX/blob/master/Preview/single.png)

*Multi Series*
 
![alt tag](https://github.com/royben/RealTimeGraphX/blob/master/Preview/multi.PNG)
  
*Gradient Fill*
 
![alt tag](https://github.com/royben/RealTimeGraphX/blob/master/Preview/gradient.png)

<br/>
<hr/>
<br/>
 
The follwing diagrams demonstrates the connections between graph components and how they are implemented on each platform.

*Model*

![alt tag](https://github.com/royben/RealTimeGraphX/blob/master/Preview/schema.png)

The graph controller binds to a renderer and a surface. Data points are pushed to the controller, the controller uses the renderer in orderer to prepare and arrange the points for visual display. Finally, the controller directs the renderer to draw the points on the specific surface.

<h3>WPF Stack Implementation<h3>

![alt tag](https://github.com/royben/RealTimeGraphX/blob/master/Preview/stack.png)
