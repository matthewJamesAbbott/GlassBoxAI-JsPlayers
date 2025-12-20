# GlassBoxAI-JsPlayers

Lightweight client-side inference players for GlassBoxAI machine learning models.

## Overview

**GlassBoxAI-JsPlayers** enables running inference for neural network models, decision forests, and graph neural networks directly in the browser or any JavaScript runtime, with no need for server compute. Trained models can be loaded in JSON format and played in web environments (such as React or Next.js), putting fast, privacy-preserving machine learning directly into the hands of students, hobbyists, or professionals.

This project is a critical part of the GlassBoxAI ecosystem, providing simple JavaScript "players" that can load and run models exported from other GlassBoxAI libraries—including both CUDA (GPU) accelerated and pure JavaScript (CPU) implementations.

## Purpose

- **Deploy trained models client-side:** Inference happens in-browser or on user's device—no server compute needed.
- **Connect training and playing:** Models trained with GlassBoxAI CUDA libraries (for speed and professional workflows) or JavaScript libraries (for education and accessibility) are saved in a standard JSON format. GlassBoxAI-JsPlayers loads this format for inference and deployment.
- **Empower learning and exploration:** Lower the barrier for students, educators, and enthusiasts to play with machine learning models without specialized hardware.

## Model Compatibility

Models must be exported in the shared JSON format used by all GlassBoxAI and Javascript-Facade* libraries. Supported models include:

- Multi-Layer Perceptrons (MLP)
- Convolutional Neural Networks (CNN)
- Recurrent Neural Networks (RNN)
- Graph Neural Networks (GNN)
- Random Forests

## List of Players

This repository includes the following lightweight, client-side players:

- **MLP Player** – for loading and running Multi-Layer Perceptron models.
- **CNN Player** – for Convolutional Neural Networks.
- **RNN Player** – for Recurrent Neural Networks.
- **GNN Player** – for Graph Neural Networks.
- **Random Forest Player** – for Random Forest models.

## Related Projects

### CUDA-based (GPU, high-speed, professional use)

- [GlassBoxAI-GNN](https://github.com/matthewJamesAbbott/GlassBoxAI-GNN)
- [GlassBoxAI-RNN](https://github.com/matthewJamesAbbott/GlassBoxAI-RNN)
- [GlassBoxAI-MLP](https://github.com/matthewJamesAbbott/GlassBoxAI-MLP)
- [GlassBoxAI-CNN](https://github.com/matthewJamesAbbott/GlassBoxAI-CNN)
- [GlassBoxAI-RandomForest](https://github.com/matthewJamesAbbott/GlassBoxAI-RandomForest)

### JavaScript-based (Education, easy access for students and hobbyists)

- [Javascript-MLP](https://github.com/matthewJamesAbbott/Javascript-MLP)
- [Javascript-CNN](https://github.com/matthewJamesAbbott/Javascript-CNN)
- [Javascript-RNN](https://github.com/matthewJamesAbbott/Javascript-RNN)
- [Javascript-GNN](https://github.com/matthewJamesAbbott/Javascript-GNN)
- [Javascript-RandomForest](https://github.com/matthewJamesAbbott/Javascript-RandomForest)

## Features

- **No GPU required:** Run inference on any device, anywhere, anytime.
- **Lightweight and Pure HTML/JavaScript:** No need for npm or external dependencies.
- **Standardized model loading:** Interoperate seamlessly with GlassBoxAI and Facade* libraries.
- **Privacy and speed:** Real-time client-side inference means no data leaves the user's device.

## Use Case Examples

1. **Train on CUDA, deploy in browser:**
   - Train complex models using CUDA GlassBoxAI libraries for speed.
   - Export the trained model to JSON.
   - Use GlassBoxAI-JsPlayers to let users interact or test model predictions within web apps, with no backend compute required.

2. **Learn and teach with JavaScript:**
   - Use *Facade* or JavaScript ML libraries to help students understand and build neural networks.
   - Export models and run inference entirely in-browser, ideal for workshops, classrooms, or interactive documentation.

3. **Flexible, facaded exploration:**
   - Facade versions (e.g. Javascript-FacadeRNN) make experimenting easier and more accessible for troubleshooting or teaching.

## Getting Started

Clone the repo:
```bash
git clone https://github.com/matthewJamesAbbott/GlassBoxAI-JsPlayers.git
```

Include the player you need in your HTML page as a script, then load your model and run inference:

```html
<script src="jsplayer-mlp.js"></script>
<script>
  // Example usage
  const modelJson = /* your JSON model */;
  const result = MLPPlayer.infer(modelJson, [/* input data */]);
  console.log('Inference result:', result);
</script>
```

## Resources


## License

MIT

---

*Created by [Matthew Abbott](https://github.com/matthewJamesAbbott) – Australia*  
