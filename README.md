![version](https://img.shields.io/static/v1?label=biological-crystallography-voice-in&message=0.4&color=brightcolor)
[![license: mit](https://img.shields.io/badge/license-mit-blue.svg)](https://opensource.org/licenses/mit)


# biological-crystallography-voice-in

## Introduction
This repo contains voice commands about biological crystallography for the automated speech recognition software Voice In Plus.
Voice In Plus is a plugin for Google Chrome and Microsoft Edge.
The commands include navigating the browser by voice to vital websites.
The snippets of LaTeX are recognized and rendered correctly by most markdown typesetting languages, including org-mode in Emacs and markdown cells in Jupyter and R Markdown notebooks and, of course, documents in Overleaf, the online LaTeX editor for academics.

https://github.com/MooersLab/biological-crystallography-voice-in/assets/15176203/c9e71fd7-e3f5-4f58-9b3d-c9dc3f87ab1e

## Examples of voice triggers and their results

\[ P_{xi}=\overline{U_{x}}+\sigma_{x}\frac{\sum^{Nu}_{k}D_{kx}\times 
    \left( \frac{S_{ki}-\overline{U_{k}}}{\sigma_{k}}\right)}{\sum^{Nu}_{k}D_{kx}} \]

  
| Voice trigger | Result|
| :------: | :----:|
|expand jac | Journal of Applied Crystallography|
|expand iucr | International Union of Crystallography|
|expression for sigmaA 2fo minus fc| $$2mF_{o} - DF_{c}$$ |
|expression for Wilson ratio | $$\left\langle I^2\right\rangle /\langle I\rangle^2$$ |
|insert equation for the structure factor|$$\mathbf{F}(\mathbf{S})=\sum_{j=1}^n f_j \exp \left[2 \pi i \mathbf{r}_j \cdot \mathbf{S}\right]$$|
|P212121  | $$P2_{1}2_{1}2_{1}$$  |
|insert space group number for P212121 | 19|


You may have to reload this page to get the equations rendered by **Mathjax**.
Likewise, when opening the biocryst.csv file in GitHub, you may have to reload the view to get the rendering by **Mathjax**.


## Usage
The utilization of these custom commands requires a subscription to Voice In Plus.
You can utilize the commands immediately after they have been uploaded.
I toggle Voice In on and off by using a keyboard shortcut.
I then dictate the command.
See the Voice In plug-in documentation to learn how to configure keyboard shortcuts.


## Installation
Each command is paired with the inserted text on a single line in a comma-separated value file, *biocryst.csv*.
Equations, code snippets, and so on that span multiple lines are placed inside double quotes.
You can upload these commands into your collection of custom commands using the **Bulk Add** button in Voice In Plus.

## Contents of the library biocryst.csv

- Names of all 230 space groups that can accommodate chiral molecules (i.e., proteins and nucleic acids)
- Space group numbers
- Software acronyms and their expansions
- Light source acronyms and their expansions
- Scientific society acronyms and their expansions
- Journal acronyms and their expansions
- Select equations formatted in LaTeX for in-line and display mode
- Select cctbx code snippets in Python
- URLs for software
- URLs for vendors


## Related repositories
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing).
You will want to include the library of contractions at a minimum to eliminate them from your formal prose.

You will likely want the [Jupyter markdown library](https://github.com/MooersLab/markdown-jupyter-voice-in) for writing prose in Markdown cells by voice command and the [Jupyter commands library](https://github.com/MooersLab/jupyter-voice-in) for running commands in code cells including line and cell magics.

## Slides from ACA 2024 meeting
See [ACA 2024 talk](https://github.com/MooersLab/ACA2024)

## Rules for developing voice commands

### Pick word combinations rarely used in ordinary prose
The basic rule for developing a voice command is to pick a word combination that is very unlikely to be used in one's prose.
This choice can avoid the accidental insertion of an unintended set of words.

### Pick word combinations that do not contain other commands
If you pick a word combination with a subset of words already assigned to another command, the commands will collide, and you will not get the intended effect.
It is better to pick a synonym for the new command than include the old one.

### Use verbs are prefixes
I use the verb "insert" before the name of the computer code or equation I want to insert.
I use the verb "expand" to expand acronyms.
I use the verb "list" to list sets of items.

### Test the commands
Like other forms of computer code, test the Voice In commands to ensure you get the intended effect.
The speed with which you vocalize a command has a significant impact.
You may have to verbalize the command quickly to avoid inserting just the first word rather than the entire command.

## Contributions are welcome
This project can benefit all biological crystallographers.
It should be a community project.
Make a pull request, post an issue, or send me an e-mail with additions in CSV format.

## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)

## Update history

|Version      | Changes                                                                                                                                    | Date                 |
|:-----------:|:------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|
| Version 0.3 |   Added update table, video, link to slides, and some commands.                                                                            | 2024 July 9          |
| Version 0.4 |   Added voice commands for centrosymmetric space groups.                                                                                   | 2024 July 17         |



  
