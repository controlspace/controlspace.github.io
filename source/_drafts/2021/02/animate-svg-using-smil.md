---
title: How to animate SVG using SMIL
date: 2021-02-07
tags: ['svg', 'web', 'animation']
author: Jyothi Prasad Buddha
description: Read on to find out how to animate SVG using SMIL
---

https://codepen.io/jbuddha/pen/yLVNbKg

```
<svg viewBox="0 0 800 800">
<g id="button-group">
  <rect id="button" x="200" y="10" width="100" height="25" fill="lightgreen" />
  <text id="button-text" x="250" y="22.5" text-anchor="middle" alignment-baseline="central">Start</text>
</g>
  
<line x1="125" y1="50" x2="70" y2="100" stroke="black" />  
<line x1="125" y1="50" x2="180" y2="100" stroke="black" />  
  
<line x1="70" y1="100" x2="25" y2="150" stroke="black" />  
<line x1="70" y1="100" x2="100" y2="150" stroke="black" />   
  
<line x1="180" y1="100" x2="150" y2="150" stroke="black" />  
<line x1="180" y1="100" x2="210" y2="150" stroke="black" />   
  
<line x1="100" y1="150" x2="80" y2="200" stroke="black" />  
<line x1="100" y1="150" x2="120" y2="200" stroke="black" /> 


<circle id="node-445" r="15" cx="125" cy="50" fill="orange" />
<text id="text-445" x="125" y="50" text-anchor="middle" alignment-baseline="central">445</text>
  
  
<circle id="node-23" r="15" cx="70" cy="100" fill="orange" />
<text id="text-23" x="70" y="100" text-anchor="middle" alignment-baseline="central">23</text>
  
<circle id="node-678" r="15" cx="180" cy="100" fill="orange" />
<text id="text-678" x="180" y="100" text-anchor="middle" alignment-baseline="central">678</text>
  
<circle id="node-12" r="15" cx="25" cy="150" fill="orange" />
<text id="text-12" x="25" y="150" text-anchor="middle" alignment-baseline="central">12</text>  

<circle id="node-46" r="15" cx="100" cy="150" fill="orange" />
<text id="text-46" x="100" y="150" text-anchor="middle" alignment-baseline="central">46</text> 
  
<circle id="node-461" r="15" cx="150" cy="150" fill="orange" />
<text id="text-461" x="150" y="150" text-anchor="middle" alignment-baseline="central">461</text>   
  
<circle id="node-789" r="15" cx="210" cy="150" fill="orange" />
<text id="text-789" x="210" y="150" text-anchor="middle" alignment-baseline="central">789</text>   
  
<circle id="node-30" r="15" cx="80" cy="200" fill="orange" />
<text id="text-30" x="80" y="200" text-anchor="middle" alignment-baseline="central">30</text> 
  
<circle id="node-89" r="15" cx="120" cy="200" fill="orange" />
<text id="text-89" x="120" y="200" text-anchor="middle" alignment-baseline="central">89</text> 
  
<circle r="15" cx="125" cy="50" fill="orange" />
<text x="125" y="50" text-anchor="middle" alignment-baseline="central">445</text>
  
<circle r="15" cx="70" cy="100" fill="orange" />
<text x="70" y="100" text-anchor="middle" alignment-baseline="central">23</text>
  
<circle r="15" cx="180" cy="100" fill="orange" />
<text x="180" y="100" text-anchor="middle" alignment-baseline="central">678</text>
  
<circle r="15" cx="25" cy="150" fill="orange" />
<text x="25" y="150" text-anchor="middle" alignment-baseline="central">12</text>  

<circle r="15" cx="100" cy="150" fill="orange" />
<text x="100" y="150" text-anchor="middle" alignment-baseline="central">46</text> 
  
<circle r="15" cx="150" cy="150" fill="orange" />
<text x="150" y="150" text-anchor="middle" alignment-baseline="central">461</text>   
  
<circle r="15" cx="210" cy="150" fill="orange" />
<text x="210" y="150" text-anchor="middle" alignment-baseline="central">789</text>   
  
<circle r="15" cx="80" cy="200" fill="orange" />
<text x="80" y="200" text-anchor="middle" alignment-baseline="central">30</text> 
  
<circle r="15" cx="120" cy="200" fill="orange" />
<text  x="120" y="200" text-anchor="middle" alignment-baseline="central">89</text> 


<animate 
    xlink:href="#button-group"
    attributeName="opacity"
    values="1;0.5;1"
    dur="0.25s"
    begin="click"
    fill="remove" 
    id="button-anim"/>  
  
<animate 
    xlink:href="#node-445"
    attributeName="cx"
    to="25" 
    dur="1.25s"
    begin="button-anim.begin + 0s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-445"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 0s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-445"
    attributeName="x"
    to="25" 
    dur="1.25s"
    begin="button-anim.begin + 0s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-445"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 0s"
    fill="freeze" 
    id="button-anim"/>  
  
<animate 
    xlink:href="#node-23"
    attributeName="cx"
    to="60" 
    dur="1.25s"
    begin="button-anim.begin + 1s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-23"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 1s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-23"
    attributeName="x"
    to="60" 
    dur="1.25s"
    begin="button-anim.begin + 1s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-23"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 1s"
    fill="freeze" 
    id="button-anim"/>  

<animate 
    xlink:href="#node-678"
    attributeName="cx"
    to="95" 
    dur="1.25s"
    begin="button-anim.begin + 2s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-678"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 2s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-678"
    attributeName="x"
    to="95" 
    dur="1.25s"
    begin="button-anim.begin + 2s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-678"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 2s"
    fill="freeze" 
    id="button-anim"/>  
  
<animate 
    xlink:href="#node-12"
    attributeName="cx"
    to="130" 
    dur="1.25s"
    begin="button-anim.begin + 3s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-12"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 3s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-12"
    attributeName="x"
    to="130" 
    dur="1.25s"
    begin="button-anim.begin + 3s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-12"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 3s"
    fill="freeze" 
    id="button-anim"/>      
  
<animate 
    xlink:href="#node-46"
    attributeName="cx"
    to="165" 
    dur="1.25s"
    begin="button-anim.begin + 4s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-46"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 4s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-46"
    attributeName="x"
    to="165" 
    dur="1.25s"
    begin="button-anim.begin + 4s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-46"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 4s"
    fill="freeze" 
    id="button-anim"/>      

  
<animate 
    xlink:href="#node-461"
    attributeName="cx"
    to="200" 
    dur="1.25s"
    begin="button-anim.begin + 5s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-461"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 5s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-461"
    attributeName="x"
    to="200" 
    dur="1.25s"
    begin="button-anim.begin + 5s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-461"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 5s"
    fill="freeze" 
    id="button-anim"/>  
  
<animate 
    xlink:href="#node-789"
    attributeName="cx"
    to="235" 
    dur="1.25s"
    begin="button-anim.begin + 6s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-789"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 6s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-789"
    attributeName="x"
    to="235" 
    dur="1.25s"
    begin="button-anim.begin + 6s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-789"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 6s"
    fill="freeze" 
    id="button-anim"/>      
  
<animate 
    xlink:href="#node-30"
    attributeName="cx"
    to="270" 
    dur="1.25s"
    begin="button-anim.begin + 7s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-30"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 7s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-30"
    attributeName="x"
    to="270" 
    dur="1.25s"
    begin="button-anim.begin + 7s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-30"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 7s"
    fill="freeze" 
    id="button-anim"/>     
  
  
<animate 
    xlink:href="#node-89"
    attributeName="cx"
    to="305" 
    dur="1.25s"
    begin="button-anim.begin + 8s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#node-89"
    attributeName="cy"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 8s"
    fill="freeze" 
    id="button-anim"/>  

  <animate 
    xlink:href="#text-89"
    attributeName="x"
    to="305" 
    dur="1.25s"
    begin="button-anim.begin + 8s"
    fill="freeze" 
    id="button-anim"/>
  
<animate 
    xlink:href="#text-89"
    attributeName="y"
    to="250" 
    dur="1.25s"
    begin="button-anim.begin + 8s"
    fill="freeze" 
    id="button-anim"/>     
  
</svg>
```


