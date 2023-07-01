- 👋 Hi, I’m @ShecTor04
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ShecTor04/ShecTor04 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
def calculate_weight(density, thickness, width, length, shape):
    if shape == "лист":
        volume = thickness  width  length
    elif shape == "труба":
        volume = 3.14  (width / 2) * 2 * length
    elif shape == "круг":
        volume = 3.14  (width / 2) * 2 * thickness
    else:
        print("Неверная форма")
        return
    weight = density * volume
    return weight

density = float(input("Введите плотность металла: "))
thickness = float(input("Введите толщину металла: "))
width = float(input("Введите ширину металла: "))
length = float(input("Введите длину металла: "))
shape = input("Введите форму металла (лист, труба или круг): ")

weight = calculate_weight(density, thickness, width, length, shape)
print(f"Вес металла: {weight} кг")
