---
title: Introduction to Linked (Open) Data
subtitle: Introduction to Linked Open Data
summary: A crash course on Linked Open Data (LOD). It introduces the fundamental concepts of data publishing and integration by using URIs, RDF triples, and ontologies.
date: 2023-12-20
math: false
image:
  placement: 2
  caption: '"Linked Open Data", deepai.org'
slides: introduction-lod-it
draft: true
---

text 

## Examples

`highlight`

```python
def hello_world(par):
  print("Hello world")
```

```markmap {height="200px"}
- Hugo Modules
  - wowchemy
  - blox-plugins-netlify
  - blox-plugins-netlify-cms
  - blox-plugins-reveal
```

```markmap
- Mindmaps
  - Links
    - [Wowchemy Docs](https://docs.hugoblox.com/)
    - [Discord Community](https://discord.gg/z8wNYzb)
    - [GitHub](https://github.com/HugoBlox/hugo-blox-builder)
  - Features
    - Markdown formatting
    - **inline** ~~text~~ *styles*
    - multiline
      text
    - `inline code`
    -
      ```js
      console.log('hello');
      console.log('code block');
      ```
    - Math: $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$
```

{{< chart data="line-chart" >}}

```mermaid
graph TD
A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

```mermaid
sequenceDiagram
Alice->>John: Hello John, how are you?
loop Healthcheck
    John->>John: Fight against hypochondria
end
Note right of John: Rational thoughts!
John-->>Alice: Great!
John->>Bob: How about you?
Bob-->>John: Jolly good!
```



```mermaid
gantt
section Section
Completed :done,    des1, 2014-01-06,2014-01-08
Active        :active,  des2, 2014-01-07, 3d
Parallel 1   :         des3, after des1, 1d
Parallel 2   :         des4, after des1, 1d
Parallel 3   :         des5, after des3, 1d
Parallel 4   :         des6, after des4, 1d
```

```mermaid
classDiagram
Class01 <|-- AveryLongClass : Cool
Class03 *-- Class04
Class05 o-- Class06
Class07 .. Class08
Class09 --> C2 : Where am i?
Class09 --* C3
Class09 --|> Class07
Class07 : equals()
Class07 : Object[] elementData
Class01 : size()
Class01 : int chimp
Class01 : int gorilla
Class08 <--> C2: Cool label
```

```mermaid
stateDiagram
[*] --> Still
Still --> [*]
Still --> Moving
Moving --> Still
Moving --> Crash
Crash --> [*]
```

- [x] Write math example
  - [x] Write diagram example
- [ ] Do something else

{{< table path="results.csv" header="true" caption="Table 1: My results" >}}

{{% callout note %}}
A Markdown aside is useful for displaying notices, hints, or definitions to your readers.
{{% /callout %}}

{{< spoiler text="Click to view the spoiler" >}} You found me! {{< /spoiler >}}

{{< icon name="terminal" pack="fas" >}} Terminal  
{{< icon name="python" pack="fab" >}} Python  
{{< icon name="r-project" pack="fab" >}} R

## Organize your notebooks
Place the notebooks that you would like to publish in a `notebooks` folder at the root of your website.

## Import the notebooks into your site
```bash
pipx install academic
academic import 'notebooks/**.ipynb' content/post/ --verbose
```

## References
- Jonathan Blaney, "Introduction to the Principles of Linked Open Data," Programming Historian 6 (2017), https://doi.org/10.46430/phen0068.
- Tom Heath and Christian Bizer (2011) Linked Data: Evolving the Web into a Global Data Space (1st edition). Synthesis Lectures on the Semantic Web: Theory and Technology, 1:1, 1-136. Morgan & Claypool.

### Did you find this page helpful? Consider sharing it 🙌
