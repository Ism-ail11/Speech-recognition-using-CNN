# Speech-recognition-using-CNN
In this project, I developed a speech recognition system using Convolutional Neural Networks (CNN) in conjunction with Mel Frequency Cepstral Coefficients (MFCC) to accurately transcribe spoken words or phrases into written text. The goal of the project was to leverage the power of deep learning and CNN architectures, along with the frequency-based MFCC features, to enhance the accuracy and robustness of the speech recognition system.

The first step in the project involved preprocessing the audio data. I applied the MFCC technique to convert the raw audio waveform into a suitable format for input to the CNN model. The MFCC algorithm extracted relevant frequency-based features from the audio signal, mimicking the human auditory system's sensitivity to different frequency ranges. This involved dividing the audio signal into small frames, applying a Fourier Transform to obtain the power spectrum, mapping it onto the Mel scale, and finally computing the logarithm of the resulting Mel filterbank energies.

Next, I designed and implemented a CNN model specifically tailored for speech recognition tasks, taking into account the MFCC features as input. The architecture of the CNN consisted of convolutional layers followed by pooling layers to extract relevant temporal and spectral features from the MFCC frames. I also incorporated additional layers such as dropout and batch normalization to improve the model's generalization and prevent overfitting. Finally, I connected the output of the CNN to a fully connected layer with a softmax activation function to classify the input audio into different speech classes or transcription labels.

To train the CNN model, I utilized a large dataset of labeled speech samples. I split the dataset into training and validation sets to evaluate the model's performance during training and prevent overfitting. I employed optimization algorithms such as stochastic gradient descent (SGD) or Adam to minimize the categorical cross-entropy loss function and update the model's parameters.

Once the CNN model with MFCC was trained, I evaluated its performance on a separate test dataset, measuring metrics such as accuracy, precision, and recall. I also performed additional evaluations using real-world speech recordings to assess the system's robustness and generalization capabilities.

Finally, I integrated the trained CNN model with MFCC into a practical speech recognition application. The application accepted audio inputs, processed them using the pre-trained CNN model with MFCC, and generated the corresponding transcriptions or text outputs. I also implemented post-processing techniques such as language modeling or decoding algorithms to further enhance the accuracy and fluency of the transcriptions.

Through this project, I aimed to showcase the effectiveness of combining CNN architectures with MFCC features for speech recognition tasks. The utilization of MFCC provided a frequency-based representation that captured important characteristics of the audio signal, while the CNN model leveraged its ability to learn hierarchical features from large-scale datasets, resulting in improved accuracy and robustness in transcribing spoken words into written text.
le lien de telechargement de dataset : http://download.tensorflow.org/data/speech_commands_v0.01.tar.gz
