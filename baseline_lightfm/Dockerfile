# Стартовое изображение  
FROM python:3.9-bookworm 
  
# Установка необходимых библиотек
## для нормальной установки lightfm
RUN python -m pip install --upgrade pip setuptools wheel
RUN python -m pip install --no-use-pep517 lightfm
RUN pip install tqdm catboost numpy pandas scikit-learn lightfm
  
# Установка JupyterLab  
RUN pip install jupyterlab  
  
# # Установка рабочей директории  
WORKDIR /app  
  
# Настройка запуска JupyterLab  
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8888", "--allow-root", "--no-browser"]
