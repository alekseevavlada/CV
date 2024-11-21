# Data Science (CV)

## Описание Проекта

Цель данного проекта заключается в сравнительном анализе изображений упаковок двух препаратов: **Clarinase 14 Repetabs** и **Claritine 20 Tablets**. Основная задача — определить степень схожести упаковок и выявить между ними различия.

## Требования

- Python 3.7+
- Библиотеки, указанные в `requirements.txt`

## Используемые Методы

- **Обработка Изображений**: Использование библиотеки OpenCV для предобработки изображений.
- **Метрики Сходства**: Применение Индекса Структурного Сходства (SSIM) из библиотеки `scikit-image` для оценки степени схожести.
- **Визуализация Различий**: Выделение различий на изображениях с помощью контуров и визуализация результатов.
- **Анализ Результатов**: Сравнительная таблица и графики для представления степени схожести.

## Результаты

- Таблица со степенью схожести всех изображений с эталонным.
- График, отображающий степень схожести для каждого изображения.
- Визуализация различий между выбранными упаковками.

# Отчет по Сравнительному Анализу Изображений Упаковок

## Методология

### 1. Сопоставление Упаковок

Были выбраны два конкретных изображения для первичного сравнения:
- **Clarinase 14 Repetabs**: `iphone xs max (47).JPG`
- **Claritine 20 Tablets**: `iphone xs max 358.JPG`

### 2. Преобразование Изображений

Все изображения были приведены к единому формату:
- Приведение к одинаковому размеру (800x800 пикселей).
- Преобразование к цветовой схеме RGB.

### 3. Определение Степени Схожести

Использовался **Индекс Структурного Сходства (SSIM)** для оценки степени схожести между изображениями. SSIM позволяет учитывать восприятие человеческим зрением и оценивать структурные изменения между изображениями.

### 4. Выделение Различий

Различия между упаковками были визуализированы путем выделения контуров участков с наибольшими отличиями.

## Результаты

### Степень Схожести

- Исходные упаковки из папок **Clarinase 14 Repetabs** и **Claritine 20 Tablets** имеют степень схожести **64.18%** по метрике SSIM.

### Выделенные Различия

![output](https://github.com/user-attachments/assets/87e6efaa-bccd-4cc8-b1fa-0c2682f3e0c5)

На визуализации различий были обнаружены следующие отличия:

- Различия в цветовой гамме фона.
- Отличия в расположении логотипов и текста.
- Различие в свето-тени, которое повлекло кривые контуры при сопоставлении.
