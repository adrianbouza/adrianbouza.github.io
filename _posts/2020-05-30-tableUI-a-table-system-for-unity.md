---
layout: post
title:  "TableUI Unity asset"
date:   2020-05-30
excerpt: "A simple UI element that allows you to create a table in Unity"
image: "/images/tableUI_main.jpg"
---

<p>In this post I'll be talking about a little project that I've recently made in Unity. It is a new UI component that allows you to create a simple table with some simple options for configuration. This project was born because I was in the need of a table UI for another project that I am developing. And looking in the asset store for solutions I noticed that there are no free assets that could help me. There were some paid solutions that could help me but I decided to make a simple asset and also learn about making a custom inspector in Unity. </p> 

<p>In the result product I managed to create a table with very few configuration options but that I hope to be improving over time. As of today you can dinamically change the number of rows and columns, customize a header, the borders, colors and style. </p>

<span class="image fit"><img src="{{ "/images/TableUI.jpg" | absolute_url }}" alt="" /></span>


<p>Of course there are some features that it lacks and could be interesting to implement, and that I intend to do. The main drawback is that you can't change the column width individually, meaning that all columns must have the same width, also all the cells are text, meaning that right now you cant put a button or a checkbox in a cell. Also you can't nest different levels of headers.  </p>

<p>The way the component is made is quite simple. It reuses the default Unity UI elements like panels and text componets and combines them in such a way that a table structure is made. You can see all the code if you download the package.</p>

[Click Here to download the project documentation][1]

[1]:{{ site.url }}/downloads/SimpleTableUIDocumentation.pdf


<!--
<ul>
    <li>UILineRenderer.cs: This script is based on the code provided by eh <a href="https://bitbucket.org/UnityUIExtensions/unity-ui-extensions/src/master/">UnityUIExtensions</a> repository, which holds a lot of useful scripts for enhancing your UI. In this case the script allows to draw lines inside a Cavnas gameobject. I edited the script to fit the needs of my project. I needed it for the drawing of the borders of the table.</li>
    <li>TableUI.cs: This script holds all the info regarding the table, such as the number of rows, columns, colors, ... It also holds the logic for creating all the structure of the table and placing each item where it belongs.</li>
    <li>TableUI_Menu.cs: This script simply defines the way you instantiate a new table. In this case I made it so you can create a table the same way you create every UI element, from the create>UI menu. It also holds the logic for creating a new Canvas and EventSystem in case you don't have one.</li>
    <li>TableUI_Editor.cs : This script is made to create the custom inspector for the component, it is located in the Editor folder.</li>
</ul>
-->