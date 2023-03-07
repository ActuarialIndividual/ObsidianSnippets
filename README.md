# ObsidianSnippets
Different snippets and templates using templater for note-taking


## Essential Plugins

- Dataview
- Templater


## Guide

1. Copy the ztemplates folder into the vault. 
2. Configure the shortcuts for the **snippets (not template)** via the templater plugin if you would like.
3. That is all


## Example Run-through

On my [recent post](https://www.reddit.com/r/ObsidianMD/comments/11hzx3x/til_you_can_embed_dataview_in_callouts_to_make/?utm_source=share&utm_medium=web2x&context=3) I noticed a few people were quite interested in my note taking process so I thought I'd showcase my setup. I have included a github repo containing all the relevant templates and code snippets.

For background, I'm a 3rd year actuarial student so most of my notes are heavily math / finance oriented with plenty of definitions and formulas. My note taking philosophy essentially is "Super simple to use. Over-engineered beneath" so that I'm not memorising millions of shortcuts but still able to have complex functionality. This way I'm able to keep up with lecture pace while still having complex, multilayered notes.


### An Example: Compound Poisson Model

On the subject page, I hit `Cmd + L` to create a new lecture note called `2. Collective Risk Modelling`, with metadata autofilled. Let's say the lecturer begins by talking about the Compound Poisson Model. I press `Cmd + D` to create a new definition note with metadata, which is embedded into my lecture note via `![[Collective Risk Model#Definition]]`. Inside the definition note, I write the formula and variable definitions.

As the lecturer continues, I can add more information to my lecture note under another H1 header, such as "Properties." This ensures only the definition note is displayed in the final result.

The final result is [here](https://www.reddit.com/r/ObsidianMD/comments/11l0wko/uni_notetaking_process_ft_templater_and_dataview/?utm_source=share&utm_medium=web2x&context=3)


# Disclaimer

I'm not really the coding type so I'm sure anyone who codes in js will die inside looking at what I've written
