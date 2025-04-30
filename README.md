

### 📘 **Learning Rate Schedules Comparison – Project Summary**

We implemented and compared four different learning rate schedules using the following hyperparameters:

- Initial learning rate: `η₀ = lr₀ = 0.05`
- Number of epochs: `50`
- All learning rate functions were evaluated and plotted over the range `epoch = 5 to 50`.

#### 🔧 Implemented Learning Rate Schedules:

1. **Time-based Decay**  
   - Function: `lr_time_based_decay(epoch, lr0)`  
   - Plotted and applied within the 5–50 epoch range.

2. **Step Decay**  
   - Function: `lr_step_decay(epoch, lr0)`  
   - Plotted and applied within the 5–50 epoch range.

3. **Exponential Decay**  
   - Function: `lr_exp_decay(epoch, lr0)`  
   - Plotted and applied within the 5–50 epoch range.

---

### 🧠 **Model Architecture**

- A simple neural network with:
  - **One hidden layer**
  - **121 neurons**
  - **Activation function: ReLU**

---

### 🏁 **Training and Evaluation**

- The model was trained using each of the learning rate strategies.
- We compared **training and test accuracy** for each method.

---

### 📈 **Results & Analysis**

Based on the accuracy plots over 50 epochs:

1. **Exponential Decay** yielded the best results with fast convergence and highest test accuracy.
2. **Step Decay** came in second place, performing well with stable accuracy.
3. **Time-based Decay** was average and showed some fluctuations during training.
4. **Constant Learning Rate** performed the worst, which aligns with expectations — using a fixed learning rate across all epochs is less efficient than adapting it intelligently over time.

> **Conclusion:** Adaptive learning rate schedules (especially exponential decay) significantly improve model performance and generalization compared to a constant learning rate.

