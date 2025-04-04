
# ORPO in Pytorch from scratch implementation

Trained OPT-330M model using ORPO in Pytorch for Instruction Following

## ModelArgs Hyperparameters

| Parameter    | Value    | Description                                                                 
|--------------|----------|-----------------------------------------------------------------------------|
| `batch_size` | 2        | The number of samples processed before the model is updated.                |
| `max_lr`     | 8e-6     | Maximum learning rate.                                                      |
| `device`     | 'cuda:0' | The device to run the model on (e.g., 'cuda:0' for GPU).                    |
| `betas`      | 0.95,0.99| Beta values                                                                 |           
| `weight_decay`| 0.1     | Weight decay values for the optimizer                                       |


### Datasets

[UltraFeedback](https://huggingface.co/datasets/argilla/ultrafeedback-binarized-preferences-cleaned)

### Frameworks:
**Pytorch**


### Epochs/Steps
Iterations (train) = 3k

Val iterations = every 20


### Losses

Train loss - 1.70 

Val loss - 1.98
(at 2.5k steps)

### Loss Curves

![Train and Val loss curves](img/curves.jpg)



