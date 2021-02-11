# -Python-Project-13
#13 Calculating user BMI

userweight = input("What\'s your weight in kilogram?\n")
print(f"Got it! {userweight}Kg")
userheight = input("What\'s your height in metters?\n")
print(f"Got it! {userheight}")

BMI = round(int(userweight) / float(userheight) ** 2, 2)

print(f"BMI = {BMI}")
if BMI < 18.5:
    print(f"You\'re underweight. ({BMI} < 18.5)")
elif float(BMI) < 25.0:
    print(f"You\'ve a normal weight. (18.5 > {BMI} < 25.0)")
elif float(BMI) < 30.0:
    print(f"You\'re overweight. (25.0 > {BMI} < 30.0)")
elif float(BMI) < 35.0:
    print(f"You\'re obese. (30.0 > {BMI} < 35.0)")
else:
    print(f"You\'re clinically obese ({BMI} > 35.0")
