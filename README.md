# Text Generation Using SimpleRNN

This project demonstrates text generation using a Simple Recurrent Neural Network (SimpleRNN) implemented with TensorFlow and Keras. The dataset used is a text file (`Book.txt`), which is processed and used to train the RNN model to generate new text sequences.

## Project Structure

The project follows these steps:

1. **Data Preparation**:
    - Read the raw text from `Book.txt` and convert it to lowercase.
    - Clean the text by removing unwanted characters.
    - Create a character-to-integer mapping and prepare input sequences for the RNN model.

2. **Model Building and Training**:
    - Define a Sequential model with SimpleRNN layers.
    - Compile the model with categorical crossentropy loss and Adam optimizer.
    - Train the model on the prepared data, saving checkpoints during training.

3. **Text Generation**:
    - Load the trained model weights.
    - Generate new text sequences using a random seed from the dataset.
    - Convert the generated integer sequences back to characters to form the generated text.


## Conclusion

This project showcases how to build a SimpleRNN model for text generation using TensorFlow and Keras. I did this project just for practice. The model is trained on a text dataset, and new text sequences are generated based on the trained model. I did only 20 epochs with a batch size of 64 due to GPU requirements. I suggest for better accuracy use batch size as 1 and epoch equal to or greater than 100 as for my case til 20th epoch the loss was decreasing.

