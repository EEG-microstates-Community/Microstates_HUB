(markdown_syntax)=
# How to add content

Here are the  contribution guidelines

## Syntax

Here is a brief overview of syntax that can be use to populate this website.

Microstates HUB uses markdown, a simple and efficent syntay.
You can check the [markdown guide](https://www.markdownguide.org/basic-syntax/) to get the basics of it.

In addition, the website offers different extensions to create more specific content.
Additional features are listed below:

## Figures

``````restructuredtext
```{figure} ../images/cool.jpg
---
width: 60%
alt: My figure text
name: my_figure
---
And here is my figure caption.
```
``````

```{figure} ../images/cool.jpg
---
width: 60%
alt: My figure text
name: my_figure
---
And here is my figure caption.
```

You can use the `:name:` variable to link to figure:
``````restructuredtext
 {numref}`my_figure`
``````
link to the figure {numref}`my_figure`

## Mathematics

``````restructuredtext

```{math}
:label: my_label
w_{t+1} = (1 + r_{t+1}) s(w_t) + y_{t+1}
```

``````

```{math}
:label: my_label
w_{t+1} = (1 + r_{t+1}) s(w_t) + y_{t+1}
```

You can use the `:label:` variable to link to equation:
``````restructuredtext
 {eq}`my_label`
``````
link to the equation {eq}`my_label`

## Notes




### Margin

````{margin} **Notes in margins**
```{note}
A note in margin
```
````

Note in margin

``````restructuredtext

````{margin} **Notes in margins**
```{note}
A note in margin
```
````

``````


## References and bibliographies

### References

The extension `sphinxcontrib-bibtex` allows to manage the bibliography of this site.
To cite an article, add the reference in bibtex format to the `bibliography.bib` file and
refer to the citation using the bibtex keyword:

````{eval-rst}
.. tabs::

   .. tab:: Markdown (MyST)

      ..  code-block:: text


          {footcite}`michel2018`


   .. tab:: rST

      ..  code-block:: restructuredtext

          :footcite:`michel2018`
 
````

Will be rendered as {footcite}`michel2018`

### Bibliography

To insert a bibliography on the page use

````{eval-rst}
.. tabs::

   .. tab:: Markdown (MyST)

      ..  code-block:: text

         ```{footbibliography}
         ```

   .. tab:: rST

      ..  code-block:: restructuredtext

         .. footbibliography::
 
````


```{footbibliography}
```
Note that all references will also be listed in the website [](Bibliography).

## Tabbed content

Tabbed content can be added using `sphinx-tabs`:

``````restructuredtext

````{eval-rst}
.. tabs::

   .. tab:: MATLAB

      EEG microstate toolbox.

   .. tab:: PYTHON

      Pycrostates.

   .. tab:: CARTOOL

      Cartool.
````

``````



````{eval-rst}
.. tabs::

   .. tab:: MATLAB

      EEG microstate toolbox.

   .. tab:: PYTHON

      Pycrostates.

   .. tab:: CARTOOL

      Cartool.
````

## Custom

You can add HTML content directly in your `markdown` files:


``````html

<iframe style="border-radius:12px" src="https://open.spotify.com/embed/track/0VypHqSlFRWpshnWwzLe5K?utm_source=generator" width="100%" height="380" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

``````

<iframe style="border-radius:12px" src="https://open.spotify.com/embed/track/0VypHqSlFRWpshnWwzLe5K?utm_source=generator" width="100%" height="380" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

## Toggle content with buttons


The extension `sphinx_togglebutton` allows to add content in toggle frames.

``````restructuredtext

```{image} https://media.giphy.com/media/FaKV1cVKlVRxC/giphy.gif
:class: toggle
```

``````

```{image} https://media.giphy.com/media/FaKV1cVKlVRxC/giphy.gif
:class: toggle
```