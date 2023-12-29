# biological-crystallography-voice-in

## Introduction
This repo contains voice commands about biological crystallography for the speech recognition software Voice In Plus.
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
Use the **bulk add** button in Voice In Plus to upload these commands into your collection of custom commands.

## Contents of the library biocryst.csv

- Names of space groups that can accommodate chiral molecules (i.e., proteins and nucleic acids)
- Space group numbers for the space groups that can accommodate chiral molecules
- Acronyms in crystallography
- Light source acronyms and their expansions
- Scientific society acronyms and their expansions


## Related repos
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing)

## Rules for developing voice commands

### Pick word combinations rarely used in normal prose
The basic rule for developing a voice command is to pick a word combination that is very unlikely to be used in one's prose.
This choice can avoid the accidental insertion of an unintended set of words.
For example, using the voice command "to do" to insert an org-mode TODO is pretty pointless because this phrase is used frequently in my prose.
Instead, I came up with the command ''priority'' and then the associated alphanumeric code for the priority. 
It is pretty unlikely that I will say the command "priority A1" in my usual prose.

### Pick word combinations that do not contain other commands
If you pick a word combination with a subset of words already assigned to another command, the commands will collide, and you will not get the intended effect.
It is better to pick a synonym for the new command than include the old one.

### Use verbs are prefaces
I use the verb "insert" in front of the computer code that I want to insert.
I use the verb "expand" to expand a person's first name into their full name and to expand acronyms into their full term.

### Test the commands
Like other forms of computer code, test the Voice In commands to ensure you get the intended effect.
The speed with which you vocalize a command has a significant impact.
You may find that you have to verbalize the command at high speed to avoid inserting just the first word of the command rather than the entire command.

