![version](https://img.shields.io/static/v1?label=biological-crystallography-voice-in&message=0.2&color=brightcolor)
[![license: mit](https://img.shields.io/badge/license-mit-blue.svg)](https://opensource.org/licenses/mit)


# biological-crystallography-voice-in

## Introduction
This repo contains voice commands about biological crystallography for the automated speech recognition software Voice In Plus.
Voice In Plus is a plugin for Google Chrome and Microsoft Edge.
These short snippets of LaTeX are recognized and rendered correctly by most markdown typesetting languages including org-mode in Emacs and markdown cells in Jupyter and R Markdown notebooks.

## Examples of voice triggers and their results

<center>
| Voice trigger | Result|
| :------: | :----:|
|expand jac | Journal of Applied Crystallography|
|expand iucr | International Union of Crystallography|
|expression for sigmaA 2fo minus fc| $$2mF_{o} - DF_{c}$$ |
|expression for Wilson ratio | $$\left\langle I^2\right\rangle /\langle I\rangle^2$$ |
|insert equation for the structure factor|$$\mathbf{F}(\mathbf{S})=\sum_{j=1}^n f_j \exp \left[2 \pi i \mathbf{r}_j \cdot \mathbf{S}\right]$$|
|P212121  | $$P2_{1}2_{1}2_{1}$$  |
|insert space group number for P212121 | 19|
</center>
You may have to reload this page to get the equations rendered by **Mathjax**.

## Usage
The utilization of these custom commands requires a subscription to Voice In Plus.
You can utilize the commands immediately after they have been uploaded.
I toggle Voice In on and off by using a keyboard shortcut.
I then dictate the command.
See the Voice In plug-in documentation to learn how to configure keyboard shortcuts.


## Installation
Each command is paired with the inserted text on a single line in a comma-separated value file (biocryst.csv).
Equations, code snippets, and so on that span multiple lines are placed inside double quotes.
You can upload these commands into your collection of custom commands using the **Bulk Add** button in Voice In Plus.

## Contents of the library biocryst.csv

- Names of space groups that can accommodate chiral molecules (i.e., proteins and nucleic acids)
- Space group numbers for the space groups that can accommodate chiral molecules
- Software acronyms and their expansions
- Light source acronyms and their expansions
- Scientific society acronyms and their expansions
- Journal acronyms and their expansions
- Key equations
- URLs for software


## Related repositories
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing).
You will want to include the library of contractions at a minimum so that you can eliminate them from your formal prose.

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
You may have to verbalize the command at high speed to avoid inserting just the first word rather than the entire command.

## Contributions are welcome
This project can benefit all biological crystallographers.
It should be a community project.
Make a pull request, post an issue, or send me an e-mail with additions in CSV format.

## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)
