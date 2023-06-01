# OpenAI-Rick-and-Morty-ChatBot

 Python script that demonstrates a conversation between two characters, Rick and Morty, using dialogue from the TV show "Rick and Morty." The script utilizes the pandas library to read a CSV file containing a dataset of Rick and Morty script lines.

First, the necessary imports are made, including importing pandas as pd and setting up the OpenAI API key. Then, the script reads the CSV file using pd.read_csv() and stores it in the variable df. The dataframe is then printed, displaying the contents of the dataset.

Next, a function named "model" is defined, which takes a prompt as input and uses OpenAI's Completion API to generate a response based on the prompt. The function returns the generated response text.

After that, a conversation between Rick and Morty is constructed using a for loop that iterates through the rows of the dataframe. If the name in a row is either "Morty" or "Rick," their corresponding dialogue line is appended to the text variable. The loop breaks after reaching the 100th row.

The prompt for the conversation is set to the constructed text. Then, a while loop begins, prompting the user (representing Morty) to input their dialogue. Morty's input is appended to the prompt, followed by "Rick:" to indicate Rick's turn. The model function is called with the prompt, and the generated response is printed as Rick's dialogue. If the user inputs "bye," the loop terminates, and Rick delivers a closing message.

The conversation provided in the example showcases an exchange between Morty and Rick, where Morty suggests going on an adventure, offers to clean Rick's spaceship, discusses picking a planet, and suggests listening to country music and bringing Jessica along. Rick rejects some of Morty's suggestions, leading to a humorous and dynamic dialogue.
