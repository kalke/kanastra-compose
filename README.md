# Kanastra Project Environment Setup

This README provides a comprehensive guide to setting up the Kanastra project environment on your local machine. This setup includes a MySQL database, the `kanastra-debt-api`, and the `kanastra-debt-page` components.

## Prerequisites

Before proceeding, ensure you have the following installed on your system:

- Docker
- Git

## Step 1: Create a Projects Directory

The first step is to create a dedicated `Projects` directory in your home directory. This will be used to store the project repositories. You can create this directory using the following command:

```bash
mkdir -p ~/Projects
```

## Step 2: Clone the Project Repositories

With the Projects directory in place, navigate to it and clone the repositories for both the API and the front-end page:

```bash
cd ~/Projects
```

```bash
git clone https://github.com/kalke/kanastra-debt-api.git
```

and

```bash
git clone https://github.com/kalke/kanastra-debt-page.git
```

## Step 3: Run the Docker Compose File

Once you have cloned the repositories, please move kanastra-compose to Projects too with:

```bash
sudo mv your-kanastra-compose-path/ ~/Projects
```

Then you ready to run the docker compose it self, and setup the components with:

```bash
docker compose -f kanastra-compose.yml up -d
```

## Step 4: Verify the Environment Setup

After starting the services, you can verify that they are running correctly:

```bash
docker ps
```

## Step 5: Accessing the Services

Once the services are up, you should be able to access:

The API: <http://localhost:8000/docs#/>

The Front-end Page: NAO SEI AINDA