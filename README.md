# ToneLibrary
The ToneLibrary is a collection of tone models for GuitarML plugins. These files are json format. Feel free to contribute your own models, either by emailing to smartguitarml@gmail.com, or by creating a pull request.

The models are linked for download on the [GuitarML Website](https://guitarml.com/)

## Compatibility
The model files are compatible with GuitarML plugins, including:
- [Proteus](https://github.com/GuitarML/Proteus)
- [NeuralPi](https://github.com/GuitarML/NeuralPi)
- [SmartAmpPro](https://github.com/GuitarML/SmartAmpPro)
- [SmartPedal](https://github.com/GuitarML/SmartGuitarPedal)
- [SmartAmp](https://github.com/GuitarML/SmartGuitarAmp)

Note: Each plugin uses a different neural net architecture, and these are not cross-compatible. Only use the models intended for a specific plugin.

## Model Training
Model training is accomplished using the following tools:
- Proteus:    [Automated-GuitarAmpModelling](https://github.com/Alec-Wright/Automated-GuitarAmpModelling)
- NeuralPi:    [Automated-GuitarAmpModelling](https://github.com/Alec-Wright/Automated-GuitarAmpModelling)
- SmartAmpPro: [SmartAmpPro plugin or Colab script](https://github.com/GuitarML/SmartAmpPro)
- SmartPedal/SmartAmp:    [PedalNetRT](https://github.com/GuitarML/PedalNetRT)

## Model Layer Info
- Proteus     (stateful LSTM -> Dense)
- NeuralPi    (stateful LSTM -> Dense)
- SmartAmpPro (Conv1D -> Conv1D -> stateless LSTM -> Dense)
- SmartPedal/SmartAmp    (WaveNet)
