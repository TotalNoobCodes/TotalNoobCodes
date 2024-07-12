- 👋 Hi, I’m @TotalNoobCodes
- 👀 I’m interested in coding
- 🌱 I’m currently learning javascript
- 💞️ I’m looking to collaborate on github
- 📫 How to reach me alexidtechmit@gmail.com
- 😄 Pronouns: he/him
- ⚡ Fun fact: my fav movie is highlander


while True:
  print("\nMenu:")
  print("1. Register new user")
  print("2. Login")
  print("3. Exit")
  choice = input("Enter your choice (1/2/3): ")

  if choice == '1':
      username = input("Enter new username: ")
      password = input("Enter password: ")
      

  elif choice == '2':  
    username_2 = input("what is your username?")
    password_2 = input("what is your password?")
    if username_2 == username:
      if password_2 == password:
        from iso639 import languages
        from googletrans import LANGUAGES, Translator


        # Function to translate a sentence
        def translate_sentence(sentence, dest_language='es'):
            translator = Translator()
            translation = translator.translate(sentence, dest=dest_language)
            return translation.text

        # Main program
        if __name__ == "__main__":
            print("Welcome to the Sentence Translator!")
            while True:
                user_input = input("Enter a sentence to translate (enter 'exit' to quit):\n ")

                if user_input.lower() == 'exit':
                    print("Exiting the program...")
                    break

                dest_language = input("Enter the destination language code (e.g., 'es' for Spanish). \n Type 'lookup' here if you don't know your language code. \n(if your language that you want it translated to is in simplified chinese then the code is zh-CN, not zh.):\n ")
                if dest_language.lower() == 'lookup':
                  user_input_language = input("type in the language that you want to find out your language code here: ")
                  def language_name_to_code(language_name):
                    language_code = None
                    for lang in languages:
                        if lang.name.lower() == language_name.lower():
                            language_code = lang.alpha2
                            break
                    return language_code
                  if __name__ == "__main__":
                    language_name = input("Enter a language name: ")
                    language_code = language_name_to_code(language_name)

                    if language_code:
                        print(f"The 2-letter code for '{language_name}' is '{language_code}'.")
                    else:
                        print(f"Language '{language_name}' not found or not supported.")
                else:
                  try:
                    translated_sentence = translate_sentence(user_input, dest_language)
                    print(f"Translated sentence: {translated_sentence}")
                  except Exception as e:
                    print(f"Translation error: {e}")

      

  elif choice == '3':
      print("Exiting...")
      break

  else:
      print("Invalid choice. Please enter 1, 2, or 3.")
<!---
TotalNoobCodes/TotalNoobCodes is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
