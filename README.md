import random

def monitor_temperature(lower_limit, upper_limit):

    temperature = random.uniform(-10, 50)
    print(f"Current Temperature: {temperature:.2f}°C")
    

    if temperature < lower_limit:
        print("Alert! Temperature is too low!")
    elif temperature > upper_limit:
        print("Alert! Temperature is too high!")
    else:
        print(" Temperature is within the safe range.")


lower_limit = float(input("Enter lower temperature limit: "))
upper_limit = float(input("Enter upper temperature limit: "))


monitor_temperature(lower_limit, upper_limit)
