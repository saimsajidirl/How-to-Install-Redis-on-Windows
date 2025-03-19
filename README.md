# How to Install Redis on Windows

Since Redis is officially supported on Linux, the recommended method to install and run it on Windows is by using WSL (Windows Subsystem for Linux). Follow these steps to set it up:

## Step 1: Install WSL

Open PowerShell or Command Prompt as Administrator and run the following command to install WSL:

    wsl --install

This will install WSL

## Step 2: Restart Your Computer

Restart your computer to apply the changes properly.

## Step 3: Install ubuntu

To install Ubuntu, open PowerShell or Command Prompt as Administrator and execute:

       wsl --install Ubuntu


## Step 4: Install Redis in WSL

Once Ubuntu is installed, open the terminal by typing ubuntu in Command Prompt and then run these commands:

    sudo apt update
    
    sudo apt install redis-server

## Step 5: Start Redis Server

Start Redis with the following command:

    sudo service redis-server start

## Step 6: Verify Redis Installation

Test if Redis is running by connecting to it:


    redis-cli

You should see the Redis prompt (127.0.0.1:6379>).
