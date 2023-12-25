# biological-crystallography-voice-in
Voice commands about biological crystallography for the speech recognition software Voice In

## Introduction
Biological crystallography related voice commands for the browser-based Voice In.
The utilization of these custom commands requires a subscription to Voice In Plus.

## Usage
After the commands have been uploaded, you can utilize them straight away.
Simply activate Voice In by using a keyboard shortcut and dictate the command.

## Installation
The commands are mapped to the text that is actually inserted.
Each command is paired with the inserted text on a single line in of a comma separated value file.
Use the bulk ad button in Voice In Plus to upload these commands into your collecton of custom commands.

## Contents

- 65 biological space groups
- acronymns in crystallography
- light source acronyms and their expansions
- scientific society acronyms and their expansions

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

