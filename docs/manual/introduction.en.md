---
title: Introduction
order: 0
redirect_from:
  - /en/docs/manual
---

<img src='https://user-images.githubusercontent.com/6113694/45008751-ea465300-b036-11e8-8e2a-166cbb338ce2.png' width='750' height='250' />

[![](https://img.shields.io/travis/antvis/g6.svg)](https://travis-ci.org/antvis/g6)
![](https://img.shields.io/badge/language-javascript-red.svg)
![](https://img.shields.io/badge/license-MIT-000000.svg)
[![npm package](https://img.shields.io/npm/v/@antv/g6.svg)](https://www.npmjs.com/package/@antv/g6)
[![NPM downloads](http://img.shields.io/npm/dm/@antv/g6.svg)](https://npmjs.org/package/@antv/g6)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/antvis/g6.svg)](http://isitmaintained.com/project/antvis/g6 "Percentage of issues still open")

[中文简介](/zh/docs/manual/introduction/)


## What is G6
[G6](https://github.com/antvis/g6) is a graph visualization engine, which provides a set of basic mechanisms, including rendering, layout, analysis, interaction, animation, and other auxiliary tools. G6 aims to simplify the complex relationships, and help people to obtain the insight of relational data.

![68747470733a2f2f67772e616c697061796f626a656374732e636f6d2f7a6f732f726d73706f7274616c2f485178596775696e464f4d49587247514f4142592e676966.gif](https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*ObTOSKnlQb4AAAAAAAAAAABkARQnAQ)

Developers are able to build graph visualization **analysis** applications or graph visualization **modeling** applications easily.

<img src="https://user-images.githubusercontent.com/6113694/44995293-02858600-afd5-11e8-840c-349e4730d63d.gif" height=150><img src="https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*I9OdTbXJIi0AAAAAAAAAAABkARQnAQ" height=150><img src="https://user-images.githubusercontent.com/6113694/44995332-2ba61680-afd5-11e8-8cab-db0e9d08ceb7.gif" height=150>

<img src="https://gw.alipayobjects.com/zos/rmsportal/HQxYguinFOMIXrGQOABY.gif" height=150><img src="https://gw.alipayobjects.com/zos/rmsportal/nAugyFgrbrUWPmDIDiQm.gif" height=150><img src="https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*xoufSYcjK2AAAAAAAAAAAABkARQnAQ" height=150>

## Features
- Abundant Built-in Items: Nodes and edges with free configurations;
- Steerable Interactions: More than 10 basic interaction behaviors ;
- Powerful Layouts: More than 10 layout algorithms;
- Convenient Components: Outstanding abilities and performance;
- Friendly User Experience: Complete documents for different levels of requirements. TypeScript supported.

G6 concentrates on the principle of 'good by default'. In addition, the custom mechanism of the item, interation behavior, and layout satisfies the customization requirements.

<img src='https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*Y0c6S7cxjVkAAAAAAAAAAABkARQnAQ' width=800 height=200 />

<img src='https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*Eh7yQ5ddu7MAAAAAAAAAAABkARQnAQ' width=400 height=500/>

## Installation

```bash
$ npm install @antv/g6
```

## Usage

<img src='https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*srtDT5slbN8AAAAAAAAAAABkARQnAQ' width=400>

```javascript
  // The source data
  const data = {
    // The array of nodes
    nodes: [{
      id: 'node1',
      x: 100,
      y: 200
    },{
      id: 'node2',
      x: 300,
      y: 200
    }],
    // The array of edges
    edges: [
      // An edge links from node1 to node2
      {
        source: 'node1',
        target: 'node2'
      }
    ]
  };
  
  // Instantiate the Graph
  const graph = new G6.Graph({
    container: 'mountNode', // The container id or HTML node of the graph canvas.
    // The width and the height of graph canvas
    width: 800,
    height: 500
  });
  // Load the data
  graph.data(data);
  // Render the graph
  graph.render();
```

[![Edit compassionate-lalande-5lxm7](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/compassionate-lalande-5lxm7?fontsize=14&hidenavigation=1&theme=dark)

For more information about the usage, please refer to [Getting Started](https://antv-g6.gitee.io/en/docs/manual/getting-started).

## Documents
- [Tutorial](/en/docs/manual/tutorial/preface)
- [Key Concepts](/en/docs/manual/middle/keyConcept)
- [Advanced Guides](/en/docs/manual/advanced/shape-and-properties)
- [API Reference](/en/docs/api/Graph)


## Links
Some implementations combined with front-end libraries from the third party:

- [Flow visualization editor powered by G6 and React](https://github.com/guozhaolong/wfd) - [Workflow Designer](https://github.com/guozhaolong/wfd)；
- [Visualization editor powered by G6 and Vue](https://github.com/caoyu48/vue-g6-editor)；
- [Visualization and graphics editor powered by G6 and Vue](https://github.com/OXOYO/X-Flowchart-Vue) - [A visual graph editor based on G6 and Vue](https://github.com/OXOYO/X-Flowchart-Vue)。


## G6 Communication Group
Users are welcome to join the **G6 Communication Group** (It is a DingTalk group). We are also welcome the github issues.

<img src='https://gw.alipayobjects.com/mdn/rms_f8c6a0/afts/img/A*dsXsSpgynmUAAAAAAAAAAABkARQnAQ' width=400>


## How to Contribute

Please let us know what you are you going to help. Do check out [issues](https://github.com/antvis/g6/issues) for bug reports or suggestions first.

To become a contributor, please follow our [contributing guide](https://github.com/antvis/g6/blob/master/CONTRIBUTING.md).

## License

[MIT license](./LICENSE).

