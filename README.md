![version](https://img.shields.io/static/v1?label=biological-crystallography-voice-in&message=0.1&color=brightcolor)
[![license: mit](https://img.shields.io/badge/license-mit-blue.svg)](https://opensource.org/licenses/mit)


# biological-crystallography-voice-in

## Introduction
This repo contains voice commands about biological crystallography for the automated speech recognition software Voice In Plus.
Voice In plus is a Google Chrome extension.
It only works in Google Chrome at this time.
The utilization of these custom commands requires a subscription to Voice In Plus.
These commands can be used in the text area of most websites opened in Google Chrome.
They can be used during dictation of manuscripts about protein and nucleic acid crystal structures and crystallography.
The commands include the symbols for all of the space groups that can accommodate chiral molecules like the biological molecules.
The symbols are represented as LaTeX math.
These short snippets of the LaTeX are recognized and rendered correctly by most markdown type setting languages including org-mode.

## Usage
After the commands have been uploaded, you can utilize them immediately.
I toggle Voice In on and off by using a keyboard shortcut.
I then dictate the command.
See the documentation for the Voice In plug-in to learn how to configure keyboard shortcuts.

## Installation
Each command is paired with the inserted text on a single line in of a comma separated value file (biocryst.csv).
Equations, code snippets, and so on that span multiple lines are placed inside of double quotes.
Use the **Bulk Add** button in Voice In Plus to upload these commands into your collection of custom commands.

## Contents of the library biocryst.csv

- Names of space groups that can accommodate chiral molecules (i.e., proteins and nucleic acids)
- Space group numbers for the space groups that can accommodate chiral molecules
- Software acronyms and their expansions
- Light source acronyms and their expansions
- Scientific society acronyms and their expansions
- Journal acronyms and their expansions
- Key equations
- Urls for software


## Related repos
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing).
At a minimum, you will want to include the library of contractions so that these can be eliminated from your formal prose.

## Rules for developing voice commands

### Pick word combinations rarely used in normal prose
The basic rule for developing a voice command is to pick a word combination that is very unlikely to be used in one's prose.
This choice can avoid the accidental insertion of an unintended set of words.

### Pick word combinations that do not contain other commands
If you pick a word combination with a subset of words already assigned to another command, the commands will collide, and you will not get the intended effect.
It is better to pick a synonym for the new command than include the old one.

### Use verbs are prefaces
I use the verb "insert" in front of the name for the computer code or equation that I want to insert.
I use the verb "expand" to expand acronyms.
I use the verb "list" to list sets of causes.

### Test the commands
Like other forms of computer code, test the Voice In commands to ensure you get the intended effect.
The speed with which you vocalize a command has a significant impact.
You may find that you have to verbalize the command at high speed to avoid inserting just the first word of the command rather than the entire command.

## Contributions are welcome
This project can benefit all biological crystallographers.
It should be a community project.
Make a pull request, post a issue, or send me e-mail with additions in csv format.

