# SVG CDN for NPM Documentation

NPM does not support rendering flowcharts or diagrams (like Mermaid) natively. 

This repository provides a jsDelivr CDN storage to host SVG images of flowcharts for NPM documentation, allowing them to be displayed properly on npmjs.com.

## How it works

Since npmjs.com strips out interactive diagrams, we pre-render them as SVG files, upload them to this repository, and load them via the jsDelivr CDN.

For example:
```markdown
![Flowchart](https://cdn.jsdelivr.net/gh/webc-fs/-@main/your-diagram.svg)
```

## Projects

Below are the projects within our organization using this CDN:

### [webc-site/math](https://github.com/webc-site/math)

A lightweight TeX-to-MathML compiler for Markdown formula rendering.

Workflow flowchart rendered using this CDN:

![Math compiler workflow](https://cdn.jsdelivr.net/gh/webc-fs/-@main/math.svg)
