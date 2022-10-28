(contributing)=
# Contributing

Microstates HUB accepts all kinds of contributions. Contributions can be about content:
- adding pages, text, figures
- edits 
- correction
or on the technical aspect:
- new website functionality (support for videos..)
- Web page layout (layout, css)

The best way to start contributing is by [opening an issue](https://github.com/EEG-microstates-Community/Microstates_HUB/issues)
on GitHub to discuss ideas for changes or enhancements

## Content contribution

 [Fork the this Repository](https://github.com/EEG-microstates-Community/Microstates_HUB/fork) on Github.

- Clone your forked repository locally.

- [OPTIONAL] create a new branch on which you will add your changes.

- Add/Edit markdown (.md) files.

- [Open a pull request](https://github.com/EEG-microstates-Community/Microstates_HUB/compare)


A detailed guide on markdown syntax use to generate the website can be found [here](markdown_syntax).

## Technical contribution

To be able to build the website localy

- [Fork the this Repository](https://github.com/EEG-microstates-Community/Microstates_HUB/fork) on Github.

- Clone your forked repository locally.

- [OPTIONAL] create a new branch on which you will add your changes.

- [OPTIONAL] create a new environment, for example with Anaconda:

    ```console
    conda create -n ms_hub python=3.9
    ```

    then activate your environment:

    ```console
    conda activate -n ms_hub
    ```

- Navigate to the repository's root folder

- Install pycrostates in editable mode with all optional dependencies:

    ```console
    pip install -r requirements.txt
    ```

- You should be able to build the website using the ```make`` command:

```console
make html
```

- You can use ``` make clean``` to clean the current build.


- [Open a pull request](https://github.com/EEG-microstates-Community/Microstates_HUB/compare)