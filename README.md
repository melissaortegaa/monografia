# Redes neuronales convolucionales para la detección de Salmonella *spp.* en aves de corral
## Convolutional Neural Networks for the Detection of Salmonella spp. in Poultry

#### Especialización en Analítica y Ciencia de datos - Analytics & Data Science
#### Universidad de Antioquia (2024)

Early detection of Salmonella spp. in poultry is crucial for improving the productivity of poultry companies in the country, as it not only reduces the mortality in their farms and maintains the profitability and reputation of the companies, but also guarantees the production of safe food for the population. However, the response capacity and cost of traditional methods limits the microbiological performance of these companies.

In this project, different architectures of Convolutional Neural Networks (CNN) were evaluated for the detection of salmonella spp. in images of poultry feces. A set of 5029 images taken in Africa between 2020 and 2021 was used, and they were classified as "Healthy" or "Salmonella." After data cleaning and preprocessing, it was found that the implementation of the L2 regularizer and a Dropout layer (0.5) in combination with the Adam optimizer (lr = 0.0001) are the optimal starting parameters for the transfer learning technique in the pre-trained VGG16 and ResNet50v2 models.

The results showed that both models outperformed the baseline model in terms of accuracy and recall, with VGG16 achieving a precision of 98.42% and ResNet50v2 of 93.67%. In conclusion, the effectiveness of computer vision and deep learning techniques for the detection of Salmonella spp. was demonstrated, which provides a solid foundation for future research with images taken in Colombia.


### Estándares de desarrollo
- Usar ramas diferentes para cada issue
- Usar la guía de estilos de [Python de Google](https://google.github.io/styleguide/pyguide.html)
- Mantener los commits cortos y con descripción
