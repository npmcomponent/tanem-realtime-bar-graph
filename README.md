*This repository is a mirror of the [component](http://component.io) module [tanem/realtime-bar-graph](http://github.com/tanem/realtime-bar-graph). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/tanem-realtime-bar-graph`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# realtime-bar-graph

A bar graph that displays information in real time using canvas.

[![browser support](https://ci.testling.com/tanem/realtime-bar-graph.png)](https://ci.testling.com/tanem/realtime-bar-graph)

## Live Demo

[Check out the live demo on CodePen](http://codepen.io/tanem/pen/zkanq), which uses the stand-alone files.

## Installation

Ensure [component(1)](http://component.io) is installed, then:

```sh
$ component install tanem/realtime-bar-graph
```

## Stand-alone

This library may be used stand-alone without the component tool. To build the stand-alone files, ensure [UglifyJS2](https://github.com/mishoo/UglifyJS2) is installed, then: 

```sh
$ make standalone
```

Then add ./standalone/realtime-bar-graph.css and ./standalone/realtime-bar-graph.js to your application and reference the `RealtimeBarGraph` global.

## Unit Tests

To run the unit tests, ensure [testling](https://github.com/substack/testling) is installed. Then:

```sh
$ make test
```

## API

### new RealtimeBarGraph

Initialize a new `RealtimeBarGraph`.

### RealtimeBarGraph#barSpacing(barSpacing:Number)

Set the bar spacing.

```js
realtimeBarGraph.barSpacing(3)
```

### RealtimeBarGraph#barWidth(barWidth:Number)

Set the bar width.

```js
realtimeBarGraph.barSpacing(5)
```

### RealtimeBarGraph#gutter(gutter:Number)

Set the gutter.

```js
realtimeBarGraph.gutter(50)
```

### RealtimeBarGraph#width(width:Number)

Set the width.

```js
realtimeBarGraph.width(600)
```

### RealtimeBarGraph#height(height:Number)

Set the height.

```js
realtimeBarGraph.height(300)
```

### RealtimeBarGraph#backgroundBarColour(backgroundBarColour:String)

Set the background bar colour.

```js
realtimeBarGraph.backgroundBarColour('#dedede')
```

### RealtimeBarGraph#historyBarColour(historyBarColour:String)

Set the history bar colour.

```js
realtimeBarGraph.historyBarColour('#ababab')
```

### RealtimeBarGraph#axesFont(axesFont:String)

Set the axes font.

```js
realtimeBarGraph.axesFont('14px sans-serif')
```

### RealtimeBarGraph#frameRate(frameRate:Number)

Set the frame rate (fps).

```js
realtimeBarGraph.frameRate(30)
```

### RealtimeBarGraph#addHit

Add a hit to the graph.

```js
realtimeBarGraph.addHit()
```

### RealtimeBarGraph#start

Start the graph animation.

```js
realtimeBarGraph.start()
```

## License

The MIT License (MIT)

Copyright (c) 2014 Tane Morgan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.