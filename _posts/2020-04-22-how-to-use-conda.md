---
layout: post
title: How to install and use conda
category: python
---

## What is Anaconda and Conda?

Anaconda is a free and open-source distribution of the Python and R which offers simple package management and deployment solutions.

The packages versions are managed my a system called **conda**. To use this package management features only, we can use the bootstrap version of Anaconda called **Miniconda**

## Download

**Step 1:**
Go to anaconda site: https://www.anaconda.com/distribution/

Click Download

![Download](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_download.png)

**Step 2:**
Next, choose your Python version. The most updated and stable version is as of 04/22/2020 is Python 3.7. (The higher the version number the later of the version)

![Download Python](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_python_download.png)

**Step 3:** 
Select the location to store the file.

![Save File](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_save_python_download.png)

Now, you have download Anaconda successfully!

## Install Anaconda

**Run Installation file**
Go to the folder that you just select. Once the download is completed, run the .exe file. An installation window will pop-up

Click Next to move the next step: 

![Installation window](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_1.png)

Click I Agree to agree with the terms and conditions

![Agree Terms and Conditions](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_2.png)

**Choose installation type**

By default, anaconda will install on the current user. You can choose all users to install Anaconda on all users in this computer. For example: if my computer have 2 users: harry and hoang (You can see list of users at: C:\Users), Anaconda will be install at C:\\Users\harry\Anaconda and C:\\Users\hoang\Anaconda  

In general, it is likely that you only need it to install for one user,so don't worry too much about this step and select Next.

![Choose installation type](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_3.png)

**Choose installation location**

By default, the destination folder will be at: C:\\Users\your-user-name\anaconda

![Choose installation location](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_4.png)

**Configure advanced installation options**

There are two options to considers:

1. Add Anaconda3 to my PATH environment

This option allows you to call anaconda from cmd directly. For example: you can open cmd and type conda scripts: `conda install pandas` However, it might cause unwanted problems that would need to uninstall and reinstall Anaconda.

2. Register Anconda3 as my default Python 3.7

This allow other applications (PyCharm. Visual Studio) use Python 3.7 installed by Anaconda. If you don't choose this option, you can always set up Python path later for each application.

![Choose Advance Options](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_5.png)

Now, you can click "install" and start using Anaconda!

![Installing](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_6.png)

## Install Package
To install package, you can find the name of the package here:https://docs.anaconda.com/anaconda/packages/pkg-docs/. Or, the easiest way that I often use is search Google: conda install package-name. By doing this, even if you don't remember the package name correctly, Google will likely suggest you the correct package

Step 1: Open Anaconda Prompt

Step 2: Type the following command:

`conda install package-name`

For example: Install package called **numpy**

`conda install numpy`

![Install Numpy Package](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_install_package.png)

By default, anaconda will install the lastest version of the package. To install a specific version

`conda install package-name=version`

For example:

`conda install numpy=1.16.4`


*Note: this tutorial requires you to have connection to Internet. 

**Anaconda Interface**
