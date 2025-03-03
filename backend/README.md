# PDF Manager Backend

This is the backend service for the PDF Manager application. It is built using FastAPI and provides endpoints for uploading, merging, and managing PDF files.

## Setup

### Install and Run using Docker

1. Build the Docker image:

   ```sh
   docker build -t pdf-manager-backend .
   ```

2. Run the Docker container:

   ```sh
   docker run -p 8000:8000 pdf-manager-backend
   ```

### Manualy Install and Run the Backend

### Prerequisites

- Python 3.11
- Conda

1. Create a virtual environment:

   ```sh
   python3 -m venv venv
   ```

2. Activate the virtual environment:

   ```sh
   source venv/bin/activate
   ```

3. Install the required dependencies:

   ```sh
   pip install -r requirements.txt
   ```

4. Install Poppler utils if missing (required for PDF processing):

   ```sh
   conda install -c conda-forge poppler
   ```

5. From the /App directory, start the server with:

   ```sh
   uvicorn main:app --reload
   ```

## Endpoints

- Checkout the docs at http://localhost:8000/docs
