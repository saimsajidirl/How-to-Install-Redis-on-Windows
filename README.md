# How-to-Install-Redis-on-Windows


Redis is officially supported on Linux, so using WSL is the recommended way to install and run Redis on Windows. Here's how to do it:

Step 1: Install WSL

Open PowerShell/cmd as Administrator and run the following command to install WSL:

    wsl --install

This will install WSL and the default Linux distribution (typically Ubuntu).

Step 2: Restart your Laptop

Restart your laptop so the settings gets saved

Step 3: Install ubuntu

Open PowerShell/cmd as Administrator use this command to install ubuntu:

       ubuntu

This will install ubuntu 

Step 4: Install Redis in WSL

Once ubuntu is installed, open the Ubuntu terminal from the Start menu and run the following commands to update the package list and install Redis:
open cmd and type 'ubuntu' to run ubuntu then type these

    sudo apt update
    
    sudo apt install redis-server

Step 5: Start Redis Server

Start Redis with the following command:

    sudo service redis-server start

Step 6: Verify Redis Installation

Test if Redis is running by connecting to it:


    redis-cli

You should see the Redis prompt (127.0.0.1:6379>).
