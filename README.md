# Edge-Efficient Knowledge-Distilled Hybrid Vision–Model System for Plant Disease Detection

This project presents an edge-efficient hybrid Vision–Language framework for intelligent plant disease diagnosis and smart farming guidance. A lightweight MobileNetV2 student model, trained via knowledge distillation from a high-capacity teacher network, performs low-FLOPs leaf image classification. The distilled architecture enables accurate disease prediction while maintaining computational efficiency suitable for edge and resource-constrained environments.

The predicted disease label and confidence score are integrated with a locally hosted large language model using Ollama, forming a hybrid CNN–LLM pipeline. This reasoning layer generates structured agricultural advisory reports, including disease summaries, causes, treatment recommendations (organic and chemical), prevention strategies, and severity assessment.

By combining efficient computer vision with contextual language reasoning, this system extends traditional plant disease classifiers into intelligent decision-support tools for practical, explainable, and scalable smart farming applications.

## Architecture

![Architecture Diagram](CV_architecture.png)

## Repository Structure

- **KD distillation model + Ollama implementation.ipynb**: The core implementation notebook containing the Knowledge Distillation training process and the integration pipeline with the Ollama LLM for generating reports.
- **ollama_helper.py**: A utility script to handle interactions with the local Ollama instance, sending the classification results and retrieving structured agricultural advice.
- **Comparison of 6 TL models.ipynb**: A comparative study of various Transfer Learning models to benchmark performance.
- **Two MobileNetV2 Students (Ensemble).ipynb**: Experiments with an ensemble of MobileNetV2 student models for improved accuracy.

## **Contributors**

<table>
  <tr>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/Jopan?s=300" width="100" alt="Jopan" /><br/>
      <a href="https://github.com/Jopan"><b>Joseph Binu George</b></a>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/SajeevSenthil?s=300" width="100" alt="Sajeev Senthil" /><br/>
      <a href="https://github.com/SajeevSenthil"><b>Sajeev Senthil</b></a>
    </td>
        <td align="center">
      <img src="https://avatars.githubusercontent.com/hari23228?s=300" width="100" alt="Hari Varthan" /><br/>
      <a href="https://github.com/hari23228"><b>Hari Varthan</b></a>
    </td>
    <td align="center">
      <img src="https://avatars.githubusercontent.com/FightKlub?s=300" width="100" alt="DJR" /><br/>
      <a href="https://github.com/FightKlub"><b>Dennis Jerome Richard </b></a>
    </td>
  </tr>
</table>
