# Use latest Python runtime as a parent image
FROM python:3

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install the required libraries
#RUN pip install numpy pandas sklearn seaborn jupyter
RUN pip install -r requirements.txt

# Make port 8888 available to the world outside this container
EXPOSE 8888

# Run jupyter when container launches
CMD ["jupyter", "notebook", "--ip='*'", "--port=8888", "--no-browser", "--allow-root"]

# Run the container with: docker run -p 8888:8888 <container-name>
