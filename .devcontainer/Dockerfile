# Use official Python image
FROM mcr.microsoft.com/devcontainers/python:3.12

# Install Jupyter and collaboration extension
RUN pip install --upgrade pip \
    && pip install notebook jupyter_collaboration

# Set the working directory
WORKDIR /workspace

# Expose Jupyter Notebook port
EXPOSE 8888

# Start Jupyter Notebook on container start
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
