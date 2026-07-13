# SAIL Architect Lab

An interactive, edge-computed neural network constructor and real-time visualizer running entirely in the browser. 

This application allows users to provision fully connected dense neural networks, capture custom image datasets via a live webcam stream, manually override hidden layer node biases, and observe live backpropagation and weight optimization on a dynamic HTML5 Canvas.

## 🚀 Live Demo
Deploying to GitHub Pages. Click here to open the lab: `https://cirqlar-official.github.io/sail-architect-lab/`

## 🧠 Core Features
* **Edge-Computed Training:** Powered by `TensorFlow.js`, models compile and train natively on your device without server-side dependencies.
* **Live Topology Visualization:** An active HTML5 Canvas rendering loop calculates and maps network weights in real-time. Positive weights render in blue; negative weights render in red.
* **Dynamic Architecture Modification:** Scale hidden layer densities (up to 5 hidden layers) and swap activation functions (ReLU, Tanh, Sigmoid, Linear) on the fly.
* **Synthetic Bias Injection:** Interactive node clicking exposes a neuron's specific bias tensor, allowing for manual numeric mutation and forced re-injection back into the model weights mid-session.
* **Dataset Inspection & Pruning:** Features a visual data frame manager to audit, review, and prune captured training frames before compilation.

## 🛠️ Technical Specifications
* **Frontend:** Tailwind CSS, Lucide Icons, Google Fonts (Inter & JetBrains Mono)
* **ML Engine:** TensorFlow.js v4.15.0 (Sequential Dense Pipeline)
* **Input Vector:** 784 dimensions (28x28 normalized grayscale matrices extracted from live webcam buffers)
* **Optimization Paradigm:** Adam Optimizer with dynamically bound learning rates
* **Analytics:** Chart.js live crossentropy loss tracking

## 🔧 How to Run Locally
1. Clone this repository:
   ```bash
   git clone [https://github.com/](https://github.com/)cirqlar-official/sail-architect-lab.git