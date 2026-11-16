# Project Resources

Everything we use or are considering. To add something, put one line under the right heading:

```
- [Name](link): what it's for
```

## Datasets
- [PlantVillage](https://github.com/spMohanty/PlantVillage-Dataset): disease classification, lab-style photos (risk of overfitting)
- [PlantDoc](https://github.com/pratikkayal/PlantDoc-Dataset): disease classification, field photos
- [Cassava Leaf Disease](https://www.kaggle.com/c/cassava-leaf-disease-classification): disease classification, field photos

## Models: Classifier
- [SigLIP](https://huggingface.co/google/siglip-base-patch16-224): image encoder that can be shared with the VLM
- [DeiT](https://github.com/facebookresearch/deit): small ViT
- [MobileViT](https://huggingface.co/apple/mobilevit-small): mobile-friendly ViT

## Models: Image Description (VLM)
- [SmolVLM](https://huggingface.co/HuggingFaceTB/SmolVLM-500M-Instruct): tiny on-device VLM (256M / 500M / 2.2B)
- [Gemma 3n](https://ai.google.dev/gemma/docs/gemma-3n): on-device multimodal, runs via MediaPipe / LiteRT
- [Qwen2.5-VL-3B](https://huggingface.co/Qwen/Qwen2.5-VL-3B-Instruct): strong detail descriptions (check licence)
- [Moondream](https://github.com/vikhyat/moondream): small captioning / VQA model
- [PaliGemma 2](https://huggingface.co/google/paligemma2-3b-pt-224): built for fine-tuning on captioning
- [Florence-2](https://huggingface.co/microsoft/Florence-2-base): lightweight captioning only

## Training
- [Hugging Face TRL](https://github.com/huggingface/trl): VLM fine-tuning
- [Hugging Face PEFT](https://github.com/huggingface/peft): LoRA adapters
- [Unsloth](https://github.com/unslothai/unsloth): faster LoRA fine-tuning

## On-Device Runtimes
- [LiteRT (formerly TFLite)](https://ai.google.dev/edge/litert): classifier on device
- [MediaPipe LLM Inference](https://ai.google.dev/edge/mediapipe/solutions/genai/llm_inference): Gemma 3n on device
- [llama.cpp](https://github.com/ggml-org/llama.cpp): GGUF VLMs on device
- [ONNX Runtime GenAI](https://github.com/microsoft/onnxruntime-genai): alternative runtime
- [ExecuTorch](https://github.com/pytorch/executorch): alternative runtime (PyTorch)

## Treatment Protocols (Layer 2)
- [UC IPM](https://ipm.ucanr.edu/): curated pest and disease management guides
- [PlantwisePlus Knowledge Bank](https://plantwiseplusknowledgebank.org/): crop disease factsheets

## Literature APIs (Layer 3)
- [PubMed E-utilities](https://www.ncbi.nlm.nih.gov/books/NBK25501/): fetch abstracts
- [Europe PMC REST API](https://europepmc.org/RestfulWebService): fetch abstracts

## Papers
- [On Calibration of Modern Neural Networks (Guo et al., 2017)](https://arxiv.org/abs/1706.04599): temperature scaling

## Other
