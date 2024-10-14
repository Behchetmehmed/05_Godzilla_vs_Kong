budget = float(input())
number_of_extras = int(input())
price_for_clothes = float(input())

decor_of_the_film = budget * 0.10
total_price_of_clothes = number_of_extras * price_for_clothes

if number_of_extras > 150:
    total_price_of_clothes = total_price_of_clothes * 0.90

everything = total_price_of_clothes + decor_of_the_film

if everything >= budget:
    money_needed = everything - budget
    print("Not enough money!")
    print(f'Wingard needs {money_needed:.2f} leva more.')
elif everything < budget:
    money_left = budget - everything
    print("Action!")
    print(f'Wingard starts filming with {money_left:.2f} leva left.')
