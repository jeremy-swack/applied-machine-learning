# Informal Response 1 (2/5/2021)

[Back to Home Page](https://jeremy-swack.github.io/applied-machine-learning/)

## Difference between Traditional Programming and Machine Learning

According to Laurence Maroney, the main difference between traditional programming and machine learning is that in traditional programming, the programmer creates the rules that result in answers, while in machine learning, a model of some kind is created that creates rules for existing answers and data. A machine learning model, like a neural network, takes in data and infers a relationship based on how the data is labeled. 

## Testing Maroney's Script

The first time I created the neural network and predicted what the value 7 would produce, I got 22.000916. However, when I created the model again with the same parameters, I got 21.998657. Although these values are extremely close, they are not the same because the loss value of both neural networks was not zero. Because of this, there is slight variation in the two outputs. It is possible that raising the number of epochs could reduce the difference, but the difference between the two values will likely never be zero.

## Neural Network with Housing Prices from Mathews County, VA

After creating the neural network, I used it to predict values for the different 2, 3, 4, and 5 bedroom houses I had and named the corresponding array "yhat". Then, I took the difference between the actual and predicted values to find if the model thought the price for each house was either too low or too high. According to the model, the best deal was on the house on Holly Point Rd with a difference of about 134k in favor of the buyer, and the worst deal was on the house on Church St with a difference of about 98k in favor of the seller. 
