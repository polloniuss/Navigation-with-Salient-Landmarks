# "Move towards the big black piano": how fine-grained features affect the goal of navigation

## Overview

Focused on improving salient landmark features within an end-to-end system, the approach aims to enhance human-like route descriptions.

## Methodology

1. **Noun Phrase Analysis:**
   - Classified salient features based on frequency from human descriptions.
   - Grouped categories using WordNet clustering methods.

2. **Image Processing with Faster-RCNN:**
   - Utilized Faster-RCNN model on Matterport3D project images.
   - Selected attributes and objects based on confidence score and overlapping area.
   - Applied clustering techniques to classify selected features.

3. **Textual and Visual Description Alignment:**
   - Computed pairs of the highest cosine score between textual and visual descriptions.

4. **LSTM Encoder Decoder Model Fine-Tuning:**
   - Fine-tuned features of an LSTM encoder-decoder model with attention on specific attributes and objects.

## Experimentation

- Applied the methodology on the Room-to-Room dataset from the Matterport3D project for navigation through pictures of rooms in houses.
