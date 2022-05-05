---
layout: journal
category: journal
subtitle:
date: 2022-04-21
tags:
---

# Using Graphviz with the Exocore

*"Graphviz is open source graph visualization software for representing structural information as diagrams of abstract graphs and networks. Graphviz layout programs take descriptions of graphs in a simple text language, and make diagrams in useful formats, such as images and SVG for web pages; PDF or Postscript for inclusion in other documents; or display in an interactive graph browser. Graphviz has many useful features for concrete diagrams, such as options for colors, fonts, tabular node layouts, line styles, hyperlinks, and custom shapes."*

---

# A Demonstration of syntax for the use of the Graphviz parser plugin

{% graphviz %}
graph {
    bgcolor="black"
    node [shape=circle, style=filled fillcolor=black, color=orange, fontcolor=orange, labelfontcolor=orange];
    edge [color=orange, fontcolor=orange, labelfontcolor=orange];
    Don -- Himi
    Charlie -- Himi
    Lemaire -- Himi [label=a];
    Lemaire -- Fod 
    Charlie -- Lemaire [label=n];
    Fod -- Don
    Charlie -- Don
    Lemaire -- Estonia
    Estonia -- Leili
    Leili -- Lemaire [label=z];
    HAF [shape=cylinder];
    HAF -- Ilyena
    Ilyena -- Lemaire
    HAF -- 11 
    HAF -- 22 
    HAF -- "33?" 
    Surfy -- 11
    Surfy -- 33
    Surfy -- Estonia
    11 [shape=doublecircle];
    Himi [shape=rectangle]
    Fod [shape=square];
    Estonia [shape=doublecircle];
}
{% endgraphviz %}

{% graphviz %}
digraph structs {
    bgcolor="black"
    node [shape=record, style=filled fillcolor=black, color=orange, fontcolor=orange, labelfontcolor=orange];
    edge [color=orange, fontcolor=orange, labelfontcolor=orange];
    struct1 [label="<f0> HAF|<f1> Himi|<f2> Fod"];
    struct2 [label="<f0> Don|<f1> Ilyena"];
    struct3 [label="Estonia |{ b |{c|<here> d|e}| f}| g | Charlie"];
    struct1:f1 -> struct2:f0;
    struct1:f2 -> struct3:here;
}
{% endgraphviz %}