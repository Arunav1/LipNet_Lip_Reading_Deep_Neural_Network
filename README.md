# LipNet_Lip_Reading_Deep_Neural_Network
This project is focused on developing an AI-powered lip reading system that processes video frames of a speaker and predicts the spoken words. The system leverages Deep Learning techniques combining 3D-CNNs (Convolutional Neural Networks) and BiLSTMs (Bidirectional Long Short-Term Memory networks) to extract and interpret visual speech patterns.
Key Features & Workflow:

    Dataset Processing:

        Prepares video frames as input, ensuring they are correctly shaped and batched.

        Converts labels to a format suitable for sequence learning using Connectionist Temporal Classification (CTC) Loss.

    Deep Learning Model:

        3D-CNN Layers: Extracts spatial and temporal features from video sequences.

        Time-Distributed Layers: Flattens the feature maps while preserving sequential information.

        BiLSTM Layers: Captures temporal dependencies in both forward and backward directions for accurate sequence prediction.

        CTC Loss Function: Enables the model to learn variable-length word sequences without requiring strict alignment.

    Training & Optimization:

        Implements learning rate scheduling for efficient convergence.

        Uses model checkpoints to save the best model weights.

        Includes a custom callback to evaluate real-time predictions at the end of each epoch.

    Prediction & Evaluation:

        The trained model takes video input and predicts spoken words by decoding the learned patterns.

        Predictions are compared against ground-truth transcriptions to measure accuracy.

Applications:

    Speech-to-Text for the Hearing Impaired

    Silent Communication Systems

    Enhanced Video Subtitle Generation

    Security & Surveillance (Silent Speech Recognition)

