# Ebbinghaus / Müller-Lyer Size-Matching Task (Online)

A standalone, single-file HTML/JavaScript implementation of an Ebbinghaus and
Müller-Lyer illusion size-matching task, built for unsupervised online
administration (e.g. linked from a Qualtrics survey). No server, account, or
installation required — participants just open the page in a browser.

## What it does

Participants adjust the size of one object (a circle, a line, or a star
during practice) to match a reference object, using the up/down arrow keys
and space to confirm. Trials are presented with and without the
Ebbinghaus/Müller-Lyer context stimuli, across both illusion types, in a
counterbalanced order. The page includes:

- A simple on-screen calibration step (matching a standard ID/credit card
  against a resizable rectangle) so stimuli render at a consistent physical
  size across different screens.
- Autosave/resume handling in case a participant's browser closes
  mid-session.
- A CSV of trial-level data that downloads automatically at the end.

## Usage

Intended to be hosted (e.g. via GitHub Pages) and linked from a survey
platform; a participant ID can be passed in via a `?pid=` URL parameter.
Opening the file directly also works for local testing, though some browsers
restrict local storage for `file://` pages.

A password-gated preview mode exists for researcher testing (a short version
of the task); see inline code comments for details.

## Limitations

Stimuli are sized to a consistent *physical* size across screens (via the
on-screen calibration step), not true per-participant visual angle, which
would require estimating each participant's viewing distance.

## Attribution

This task is adapted for online/browser administration from an original
PsychoPy experiment:

> Developed at Karolinska Institutet by Lowe Wilsson, with input from Tessa
> M. van Leeuwen (Radboud University).
> Original repository: https://github.com/AnonZebra/ebbinghaus-mullerlyer-psychopy

Based on:

> Burghoorn, F., Dingemanse, M., van Lier, R., & van Leeuwen, T. M. (2020).
> The Relation Between Autistic Traits, the Degree of Synaesthesia, and
> Local/Global Visual Perception. *Journal of Autism and Developmental
> Disorders, 50*(1), 12–29. https://doi.org/10.1007/s10803-019-04222-7

## License / usage terms

Following the terms of the original project: free to use and modify for
non-commercial purposes (research included) with attribution. If you publish
work based on this project, please cite the Burghoorn et al. article above
and link to the original PsychoPy repository.
