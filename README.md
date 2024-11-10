# atom-hack-24
Анализ документации от поставщиков на уровень соответствия требованиям для оперативного принятия решений

## Установка
Решение запускалось в Yandex DataSphere в среде с GPU V100 и CUDA 11.8

Используется библиотека [unsloth](https://github.com/unslothai/unsloth), про установку которой можно прочитать в репозитории

* [install](install.ipynb) — установка дополнительных библиотек, исправление бага и скачивание модели с Hugging Face

* [requirements](requirements.txt) — список всех зависимостей

## Обучение

* [prompts](prompts.py) — файл с шаблонами промптов и инструкциями

* [make-dataset](make-dataset.ipynb) — подготовка датасета для обучения

* [train-model](train-model.ipynb) — обучение (меньше 6 минут) и сохранение весов

## Тестирование

* [Mistral-finetuned](https://drive.google.com/file/d/1YC_G6Pj5V8iHoxvZphJ1jjyV_lNDi2mU/view?usp=sharing) — ссылка на веса

* [FULL_LAUNCH](FULL_LAUNCH.ipynb) — полный запуск решения на тестовом датасете, произведен замер средней скорости обработки на один файл (17с)
