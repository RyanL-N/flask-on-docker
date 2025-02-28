# Use the official Python image
FROM python:3.12

# Set the working directory
WORKDIR /usr/src/app

# Install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /usr/src/app/requirements.txt
RUN pip install -r requirements.txt

# Copy application files
COPY . /usr/src/app/

# Run the application
CMD ["python", "manage.py", "run", "-h", "0.0.0.0", "--port=5000"]

