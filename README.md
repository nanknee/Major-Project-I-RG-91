# Major-Project-I-RG-91

Crop-disease and crop-stress detection has become one of the most heavily explored problems in 
agricultural AI, but the overwhelming majority of student and academic projects reduce it to a single 
task: classifying leaf images from the PlantVillage dataset. While this benchmark is convenient, it is also 
saturated. Dozens of published models already report high accuracy on it and it does not reflect how 
stress actually develops in a real field. Leaf-image classifiers only detect disease after visible symptoms 
such as lesions or discoloration have already appeared, by which point yield loss may be unavoidable 
and the underlying cause (pathogen, water stress, nutrient deficiency, or heat stress) is often impossible 
to distinguish from the image alone. Real field conditions involve multiple interacting stress factors 
fluctuating soil moisture, temperature extremes, humidity, and weather events that single-modality, 
image-only pipelines simply cannot capture, leaving a significant gap between academic benchmarks 
and practically useful, field-deployable systems. 
This project addresses that gap by fusing three complementary data modalities: aerial/drone and satellite 
imagery, ground-based IoT sensor time-series (soil moisture, temperature, humidity), and weather API 
data into a single multimodal model that predicts crop stress type and severity before visible symptoms 
emerge. Imagery captures spatial patterns of canopy health, while sensor time-series and weather data 
capture the temporal and environmental drivers of stress that precede visible symptoms. By combining a 
CNN/ViT-based visual encoder with an LSTM/Temporal-CNN sensor encoder through a fusion 
transformer or cross-attention layer, the system can correlate what a field looks like with what 
conditions caused it to look that way, enabling an early-warning alert rather than a post-hoc diagnosis. 
This multimodal fusion approach is still a genuine research gap in agricultural AI, and it directly targets 
a practical need: giving farmers actionable, early alerts instead of a late confirmation of damage that has 
already occurred. 
