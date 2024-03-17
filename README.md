#Love-Calculator coding

#referrence variable
true_love = 'truelove'

while True:
  count = 0
  message = input("Would you like to check your love percentage? (Y/N): ")
  if message == "Y" or message == "y":
    her_name = input("Enter her full name with a space: ")
    his_name = input("Enter his full name with a space: ")
    their_name = her_name.lower() + his_name.lower()
    for letter in their_name:
      if letter in true_love:
        count += 1
      else:
        continue
    print(f"{her_name.title()} and {his_name.title()}'s love count is {count}")
    continue
  elif message == "N" or message == "n":
    break
  else:
    print('Invalid input! Please press "Y/N" to continue')
