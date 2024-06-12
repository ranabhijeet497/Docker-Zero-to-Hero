# Use the base image
FROM python:3.12-slim

# Set the working directory
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install dependencies
RUN apt-get update && \
    apt-get install -y python3-pip python3-venv pipx && \
    pipx install --python python3 /path/to/your/application

# Copy the application code
COPY . .

# Set the PATH to use pipx
ENV PATH="/root/.local/bin:$PATH"

# Set the default command
CMD ["your_application_command"]
