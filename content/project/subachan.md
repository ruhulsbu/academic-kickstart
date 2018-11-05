+++
# Date this page was created.
date = "2012-01-01"

# Project title.
title = "Subachan: Bengali Text to Speech Synthesis Software."

# Project summary to display on homepage.
summary = "This software provide text to speech services to the user of Mongol Dip. Funded by Ministry of Science and ICT, Bangladesh."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = ""

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["NLP", "Speech Synthesis", "HCI"]

# Optional external URL for project (replaces project detail page).
external_link = "https://ieeexplore.ieee.org/abstract/document/5700757"
url_project = "https://ieeexplore.ieee.org/abstract/document/5700757"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
# [header]
# image = "updated_pipeline.jpg"
# caption = "My caption :smile:"

+++

Subachan can convert Bengali words to corresponding speech. In doing these tasks, we had to develop a bunch of algorithms for the Bengali language processing. We have developed an algorithm for text normalization implementing the expansion rules based on the grammar of Bengali language. We can detect standard and non-standard words and can resolve abbreviation, as well as we can identify phrase by this algorithm. We have also developed an algorithm for phonetic analysis that converts a Bengali sentence to its phonetics using customized grapheme to phoneme rules developed based on our research on Bengali language. We have also developed a small lexicon which removes the O-karanto problem in Bengali language in some cases. Hence correctness of the Bengali pronunciation is increased. Our approach for diphone reduction makes the system smaller and faster without losing optimal intelligibility and naturalness of the generated speech. We have followed a completely new approach for handling the joint letters in which the developed algorithm transforms a joint letters to the concatenation of diphones, fade in and fade out effect of starting and ending diphones and silence to maintain the artificial stress and pitch.
 
We did not use any kind of transliteration like another Bengali text to speech synthesis software Kotha that use the third party tools Festival, a multi lingual text to speech synthesis system. Again, Our system, Subachan takes around 45 ms to generate a 10 second utterance where as Festival takes 2 seconds to generate a 10 second utterance which is too long. The most important difference is that we have used only 527 diphones as oppose to the 4355 diphones of Kotha. Since most of the speech generation is done algorithmically we could decrease the total number of word-specific information of lexicon in our system. With some exceptions, Subachan can work in any situation and produce better performances. Demonstrated implementation of Subachan produces emotionless speech close to natural language like a news presenter.