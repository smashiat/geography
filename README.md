Structured experiments to test how geographic context (where an image appears to be taken) influences model interpretation and outputs.

## Overview

This project investigates whether and how AI vision models respond differently based on the geographic origin of an image. Experiments span image captioning, visual question answering, zero-shot classification, and sentiment analysis — all examined through a geographic lens.

## Motivation

Geographic bias in vision-language models is underexplored. Images from different continents may trigger different model behaviors: in word choice, sentiment, confidence, or classification, even when the depicted object category remains the same. This project provides a reproducible experimental scaffold for surfacing and quantifying those differences.

## Experiments

### Captions (`Captions.ipynb`)
Image captioning using [BLIP] (https://github.com/salesforce/BLIP). Generates natural language descriptions for images across geographic regions to examine whether caption content or tone varies by location context.

### Continent Classification (`ContinentClassification.ipynb`)
Tests whether vision models can identify which continent an image was taken in, probing implicit geographic knowledge encoded in model representations.

### Sentiment Analysis in Captions (`SentimentAnalysisinCaptions.ipynb`)
Analyzes negative connotative language in generated captions, broken down by continent. Investigates whether models use systematically more negative or positive language when describing images from different parts of the world.

### Visual Question Answering (`VQAipynb.ipynb`)
Uses VQA (Visual Question Answering) to probe how geographic context shapes model responses to structured questions about image content.

### Zero-Shot Classification (`zeroshot/`)
Applies zero-shot classification to geographically diverse images to examine category assignment patterns across regions using [CLIP] (https://openai.com/index/clip/).

### Bootstrapping Experiments (`stats/`)
Statistical bootstrapping framework for measuring variance and significance across geographic groups in model outputs.
