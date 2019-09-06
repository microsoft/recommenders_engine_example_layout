<img src="assets/reel_mock.png">

## Introduction 

Recommenders Engine Example Layout (REEL) is a cross-platform movie recommendation application that demonstrates the integration of example recommendation algorithms from Microsoft/Recommenders into an application workflow. The following sections will demonstrate how to locally build REEL. These sections will guide the reader into:
	
* Creating an ML model endpoint
* Setting up and populating [Azure SQL Database](https://docs.microsoft.com/en-us/azure/sql-database/)
* Setting up [Azure Search](https://docs.microsoft.com/en-us/azure/search/)
* Running the app's backend on Azure using [AKS](https://docs.microsoft.com/en-us/azure/aks/)
* Installing the [Xamarin.Forms](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/) app for the mobile client
	
Currently, REEL runs *Simple Algorithm for Recommendation (SAR)* and *LightGBM algorithms*. The application is built using [Xamarin.Forms](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/),
 so it is supported on **iOS**, **Android** and **[Windows Desktop](https://docs.microsoft.com/en-us/windows/uwp/get-started/universal-application-platform-guide)**. The algorithms are trained on the [MovieLens dataset](https://grouplens.org/datasets/movielens/).




## System Architecture
 
 <img src="assets/system_arch_diagram.png">


# Getting Started

At a high level, this project is composed of 3 main folders
* [backend](backend/README.md): where the Flask web service logic / deployment files are kept. This folder's README also contains instructions for setting up the backend and the database
* [data](data/DATABASE_README.md): where scripts for setting up the SQL database with the movielens dataset are kept
* [mobile](mobile/README.md): where the Xamarin.Forms cross platform application sits. This folder's README contains a high level tour of how the application is structured, as well as information about how to run the application

## Installation process

To get started running the mobile application, a few steps must be followed: 
1. Deploy a SAR model by running the SAR notebook
2. Deploy a LightGBM model by running the LightGBM notebook
3. Set up and deploy the backend to AKS
4. Set up and run the Xamarin.Forms application on your choice of Android, iOS, or UWP

# Demos

## Onboarding

<img src="assets/Onboarding1.gif" width="300px"> 
<img src="assets/Onboarding2.gif" width="300px">

## Browse

<img src="assets/Browse.gif" width="300px">

## Favorites

<img src="assets/Favorites.gif" width="300px">

## Settings

<img src="assets/Settings.gif" width="300px">

## Search

<img src="assets/Search.gif" width="300px">

## Show your support

Give a ⭐️ if this project helped you!

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.