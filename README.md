# GenAI to Explain CNN

Deep Learning research project exploring CNN interpretability and bias through generative AI and semantic analysis.

## 📋 Overview

This project investigates how ResNet-50 truly "sees" images by combining Stable Diffusion 3.5 for controlled image generation with Core WordNet for semantic consistency. The main goal is to understand whether the network relies on genuine object recognition or contextual shortcuts learned during training.

## 🎯 Key Findings

- Deeper layers effectively distinguish semantic concepts
- The network shows significant dependency on visual context
- Measurable bias: bees need flowers, frogs need lily pads, guitars need stages

## 📁 Project Structure

### Notebooks
- `DL_PROJECT.ipynb` - Main analysis pipeline
- `DL_PROJECT_100IMGS.ipynb` - Extended validation with 100 images

### Documentation
- `DL_Project_ENG.pdf` - Full white paper (English)
- `DL_Project_ITA.pdf` - Full white paper (Italian)

### Data Files
- `neuron_analysis.json` - Neuron activation analysis
- `prompt_synset_mapping.json` - Prompt to synset mappings
- `quantitative_metrics.json` - Separability scores and metrics
- `synset_layer_analysis.json` - Layer-wise synset analysis

## 🛠️ Methodology

1. Select classes from Core WordNet and Salient ImageNet
2. Generate images with Stable Diffusion 3.5 using three prompt types:
   - Object-only (isolated objects)
   - Context-only (environments without objects)
   - Mixed (objects in natural contexts)
3. Extract ResNet-50 activations using forward hooks
4. Measure bias by comparing classification confidence across prompt types

## 🚀 Technologies

- Stable Diffusion 3.5 Large
- ResNet-50
- Core WordNet
- Salient ImageNet

## 📊 Results

While ResNet-50 shows strong semantic understanding, it exhibits significant bias toward contextual cues, revealing the challenges in CNN interpretability and the need for more robust training approaches.

## 🎓 Academic Achievement

Developed for a Deep Learning course - achieved the highest grade.

## 📄 License

Available for academic and research purposes.

---

For detailed methodology and results, see the white papers in the repository.
