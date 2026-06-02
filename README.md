# Image-Forgery-Detection

Digital image manipulation has become increasingly sophisticated, making the detection of 
tampered or forged images a critical challenge in digital forensics, security, and media 
authentication. Traditional pixel-level and handcrafted feature-based methods often fail against 
modern editing techniques that subtly alter statistical traces within images. To address this, the 
present work proposes a deep learning–based forgery detection framework that integrates Spatial 
Rich Model (SRM) high-pass residual filters, a custom Initial Trace Extractor, and a specialized 
ManNet classification architecture designed to learn manipulation-aware patterns with improved 
precision. 

The system is trained and evaluated on multiple benchmark datasets, including CASIA 2.0, 
IMD2020, and the Columbia Splicing dataset, covering manipulation types such as splicing, 
copy-move, and region removal. The pipeline begins with the extraction of noise residuals using 
SRM convolution kernels, which suppress semantic content while amplifying manipulation 
traces. These residuals are fused with features extracted from the Initial Trace Extractor, resulting 
in a rich multi-level representation of both structural and statistical forensic cues that are often 
invisible in RGB space. The fused features are then processed by the ManNet classifier, a 
lightweight convolutional neural network optimized for binary manipulation detection and 
designed for computational efficiency. 

Experimental results demonstrate that the proposed model effectively captures subtle 
inconsistencies introduced during tampering, achieving improved accuracy, F1-score, and 
robustness when compared to baseline CNN architectures relying solely on pixel-domain 
information. Furthermore, the integration of noise-aware residual learning significantly enhances 
sensitivity to low-intensity forgeries and improves generalization across diverse manipulation 
techniques. These findings highlight the potential of SRM-guided CNN architectures for 
real-world scenarios such as media verification, forensic investigations, integrity assurance, and 
AI-safety applications, providing a promising direction for future research in digital image 
forensics. 
