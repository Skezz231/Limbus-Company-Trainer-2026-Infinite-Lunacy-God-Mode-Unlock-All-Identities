# Limbus Company Trainer

Демонстрационный тренер для игры Limbus Company с современным ImGui интерфейсом.

![Limbus Company](https://img.shields.io/badge/Game-Limbus%20Company-blue)
![C++](https://img.shields.io/badge/Language-C%2B%2B17-green)
![ImGui](https://img.shields.io/badge/GUI-ImGui-orange)
![License](https://img.shields.io/badge/License-Educational-yellow)

## ⚠️ Disclaimer

Этот проект создан **исключительно в образовательных целях** для изучения:
- Создания GUI приложений с ImGui
- Работы с GLFW и OpenGL
- Архитектуры тренеров для игр
- Эмуляции игровой логики

**НЕ используйте** это для читерства в онлайн-играх. Это может привести к бану аккаунта.

## ✨ Возможности

### 🎮 Функциональность
- **Resources:** Infinite Lunacy, Unlock All, Infinite Materials, Infinite Stamina
- **Combat:** God Mode, Damage/Defense Multipliers, Infinite HP/SP/Sanity
- **Automation:** Auto Farm, Auto Battle, Story Skip, Speedhack
- **Misc:** Anti-Cheat Bypass (эмуляция), Max Level Sinners

### 🎨 Интерфейс
- Современный темный дизайн
- Полноэкранный режим без рамок
- Панель статистики в реальном времени
- Система уведомлений
- Блокировка функций до подключения к "игре"
- Плавные анимации и эффекты

### 💻 Технические особенности
- Эмуляция сканирования процесса игры
- Живая статистика (Lunacy, HP, Level и т.д.)
- Реалистичная обратная связь
- Без консольного окна (только GUI)

## 🚀 Установка и запуск

### Требования
- **CMake** 3.10+
- **C++17** компилятор (MSVC, GCC, Clang)
- **Git** для клонирования ImGui

### Windows

1. **Клонируйте репозиторий:**
```bash
git clone https://github.com/yourusername/limbus-company-trainer.git
cd limbus-company-trainer
```

2. **Скачайте ImGui:**
```bash
git clone https://github.com/ocornut/imgui.git
```

3. **Соберите проект:**
```bash
mkdir build
cd build
cmake ..
cmake --build . --config Release
```

4. **Запустите:**
```bash
.\Release\LimbusCompanyTrainer.exe
```

### Linux

1. **Установите зависимости:**
```bash
sudo apt-get install build-essential cmake libglfw3-dev libgl1-mesa-dev git
```

2. **Клонируйте и соберите:**
```bash
git clone https://github.com/yourusername/limbus-company-trainer.git
cd limbus-company-trainer
git clone https://github.com/ocornut/imgui.git
mkdir build && cd build
cmake ..
make
./LimbusCompanyTrainer
```

### macOS

1. **Установите зависимости:**
```bash
brew install cmake glfw
```

2. **Соберите проект:**
```bash
git clone https://github.com/yourusername/limbus-company-trainer.git
cd limbus-company-trainer
git clone https://github.com/ocornut/imgui.git
mkdir build && cd build
cmake ..
make
./LimbusCompanyTrainer
```

## 📁 Структура проекта

```
limbus-company-trainer/
├── src/
│   └── main.cpp          # Основной код приложения
├── imgui/                # ImGui библиотека (клонировать отдельно)
├── build/                # Директория сборки (создается автоматически)
├── CMakeLists.txt        # Конфигурация CMake
├── .gitignore           # Исключения Git
└── README.md            # Документация
```

## 🎯 Как это работает

1. **Запуск:** Приложение начинает "сканировать" процесс игры (эмуляция - 3 секунды)
2. **Подключение:** После "обнаружения" игры активируются все функции
3. **Взаимодействие:** Включайте/выключайте читы, меняйте множители
4. **Обратная связь:** Наблюдайте изменения в статистике и уведомления

## 🛠️ Технологии

- **C++17** - Основной язык
- **ImGui** - Графический интерфейс
- **GLFW** - Управление окнами
- **OpenGL 3.3** - Рендеринг
- **CMake** - Система сборки

## 📸 Скриншоты

(Добавьте скриншоты вашего приложения)

## 🤝 Вклад в проект

Pull requests приветствуются! Для серьезных изменений сначала откройте issue.

## 📝 Лицензия

Этот проект создан в образовательных целях. Используйте ответственно.

## ⭐ Если вам понравилось

Поставьте звезду этому репозиторию, если проект был полезен!

---

**Примечание:** Функции являются UI-эмуляциями и не модифицируют реальную игру.
