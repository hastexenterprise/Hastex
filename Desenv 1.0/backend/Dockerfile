# Usar uma imagem oficial do Python como base
FROM python:3.12.6

# Definir o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiar o arquivo de requisitos e instalar as dependências
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Copiar o restante do código para o contêiner
COPY . /app/

# Expor a porta que o Django usará
EXPOSE 8000

# Comando para iniciar a aplicação
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "C:\Users\joaop\Documents\SaaS\Desenv 1.0\backend\wsgi.py"]