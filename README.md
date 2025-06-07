# How to Install Redis on Windows by Saim

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

## Step 4: Run Ubuntu and Create an Account

Once Ubuntu is installed, open the terminal and then run this command:

    wsl
    
This command will launch Ubuntu, prompting you to create a UNIX user account. Once the account is set up, Ubuntu will start running in the terminal.

## Step 5: Install Redis in WSL

After creating your UNIX account, run the following commands one by one:

    sudo apt update
    
    sudo apt install redis-server

## Step 6: Start Redis Server

Start Redis with the following command:

    sudo service redis-server start

## Step 7: Verify Redis Installation

Test if Redis is running by connecting to it:


    redis-cli

You should see the Redis prompt (127.0.0.1:6379>).
