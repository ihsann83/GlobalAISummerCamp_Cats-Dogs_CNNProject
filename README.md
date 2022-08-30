# GlobalAISummerCamp_Cats-Dogs_CNNProject

Data Set: https://www.microsoft.com/en-us/download/details.aspx?id=54765

I got the images and splitted them into train, validation and test data.

Then, I checked the sizes of the images and resize them as (128,128,3)

I rescaled them.

# Image Manipulation

I used ImageDataGenerator to get more data in order to make a better prediction, because deep learning needs more data.

# Creating the Model

Then I created my model with the generated data.

I used Conv2D with relu as activation function, 64 filters,

Maxpooling with pool size (2,2), 

Dropout (0.5)

Also I used compile with;

loss = binary_crossentropy

optimiser = adam

metrics = accuracy

# Early Stopping

I used early stopping with monitor = val_loss

# Model Training

I trained model with 10 epochs

# Evaluating The Model

I got the loss, accuracy, val_accuracy and val_loss scores. Also I visualised those scores.

With those scores, I got the pred probalisities. I used them in order to get the confusion matrix and classification report.






