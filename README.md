# Simple chatbot ML project
```python
responses = {
    "hi": "Yes my lord!!!",
    "how are you": "I'm doing well , thank you.",
    "bye": "see ya later !", 
    "do you like games": "no i am your puppet ☻♦☻",
    "default": "My IQ is not so high to process that my lord!."
}

print("Hello! I'm jinny your SHUBCHINTAK chatbot. Type 'bye' to exit.")


while True:
    user_input = input("You: ").lower()

    response = responses.get(user_input, responses['default'])

    print("Chatbot:", response)

    if user_input == 'bye':
        break

```

# responses = {
# "hi": "Hello!",
# "how are you?": "I'm doing well, thank you.",
# "bye": "Goodbye!",
# "default": "I'm not sure how to respond to that."
# }
## Explanation:-

This part of the code initializes a Python dictionary named responses.

It contains key-value pairs where the keys are strings representing user inputs, and the values are corresponding responses that the chatbot will give for those inputs.

For example, if the user inputs "hi," the chatbot responds with "Hello!" which is based on dictionary.

print("Hello! I'm chatbot. Type 'bye' to exit.")

# while True:
# user_input = input("You: ").lower()

## This starts an infinite while loop that continues until explicitly broken.

Within the loop, it prompts the user with input("You: ") to enter their message, converts it to lowercase using .lower(), and stores it in the user_input variable.

# response = responses.get(user_input, responses['default'])
Check if user input is in the predefined responses, otherwise use the default response

## Explaination
""responses.get(user_input, responses['default'])"" is a method call on the responses dictionary.

user_input is the key that the code attempts to retrieve from the dictionary.

If the user_input key exists in the responses dictionary, responses.get() returns the corresponding value associated with that key.

However, if the user_input key does not exist in the dictionary, the get() method returns the value specified as the second argument (responses['default'] in this case). This serves as a fallback or default response.

For instance:

If the user inputs "hi," user_input becomes "hi," and the code looks for this key in the responses dictionary. It finds a match, so it returns the value associated with "hi," which is "Hello!".

If the user inputs something not in the dictionary, like "What's your favorite color?" the code does not find a match for this input in the dictionary. In such cases, it returns the default response, which is "I'm not sure how to respond to that."

This method allows the chatbot to handle user inputs by providing predefined responses for specific inputs while defaulting to a general response when the input is not explicitly defined in the dictionary.
