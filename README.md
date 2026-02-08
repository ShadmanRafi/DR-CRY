# DR-CRY: Dashcam Road-Crack Recognition Y-network
Robust Crack Detection via CNN-Transformers and Large-Scale Pretraining

A Hybrid Encoder-Decoder architecture. The backbone utilizes a pre-trained ResNet-34 to extract high-frequency texture features (asphalt grain), while a Transformer Bottleneck applies self-attention to capture long-range dependencies, essential for connecting disjointed crack segments. 
In the model architecture, Branch A (Top) performs segmentation using skip connections. Branch B (Bottom) performs anomaly reconstruction to flag unknown defects. 
To handle class imbalance and focus on thin boundaries, we utilize the Geometry-Aware Guided Loss (GAGL) which weights edge pixels higher than background pixels. This ensures the model prioritizes structural integrity over simple background classification.

