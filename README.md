# AI IMAGE CAPTIONING PROJECT

## OVERVIEW
This project implements an AI powered image captioning system using a pre-trained vision language model. The system takes an input image and generates a natural language description of its contents.

The goal of this project is to explore how modern generative AI models can be used to connect computer vision and natural language processing in a practical application.

## Problem Statement
Automatically generating captions for images is an important task in artificial intelligence, with applications in accessibility, image search, and content organization.

This project aims to build a system that will:
* Take an image as input
* Generate a descriptive caption
* Evaluates the quality of generated captions

## Approach
This project uses the BLIP (Bootstrapping Language Image Pretraining) model from Hugging Face.

* Model: 'Salesforce/blip-image-captioning-base'
* Framework: PyTorch
* Library: Hugging Face Transformers

The System:
1. Load a pre-trained BLIP model
2. Processes input images
3. Generates captions using the model
4. Evaluates the results using manual scoring

Beam search ('num_beams=5') is used to improve caption generation quality.

## Dataset
A small dataset of 15 images was used for testing.
The images were collected from:
- Unsplash

The dataset includes a variety of categories:
- Animals
- People
- Food
- Nature scenes
- Everyday objects

## Results
The model successfully generated captions for all input images.
Captions were evaluated based on:
* Accuracy
* Detail
* Clarity

Example output:
* “a woman and two children in a wagon picking apples from a tree”
* “a brown dog carrying a stick in the woods”
* “a white plate topped with meat and vegetables”

