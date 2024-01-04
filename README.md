temperature_coefficient = 0.5
precipitation_coefficient = -0.2
wind_coefficient = 0.1

def weather_model_hardcoded():
    temperature = temperature_coefficient * 2**2
    precipitation = precipitation_coefficient * 2**2
    wind = wind_coefficient * 2**2

    return temperature, precipitation, wind

def weather_model_keyboard_input():
    latitude = float(input("Enter geographical latitude: "))
    date = input("Enter date (YYYY-MM-DD): ")

    temperature = temperature_coefficient * latitude**2
    precipitation = precipitation_coefficient * latitude**2
    wind = wind_coefficient * latitude**2

    return temperature, precipitation, wind
result_hardcoded = weather_model_hardcoded()
result_keyboard_input = weather_model_keyboard_input()

print("Hardcoded Result:", result_hardcoded)
print("Keyboard Input Result:", result_keyboard_input)
