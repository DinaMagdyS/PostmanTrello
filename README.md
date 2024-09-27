# Trello API Testing with Postman
![TrelloAPIRun](https://github.com/user-attachments/assets/6e193d10-f4e6-4acd-8cfc-91322222158f)

![NewmanHTMLExtraReport](https://github.com/user-attachments/assets/bc7a9fd1-fa39-418b-a836-a9b7b3103d35)




This repository contains Postman collections and environment variables for testing the [Trello API](https://developer.atlassian.com/cloud/trello/rest/).

## Introduction

This project demonstrates API testing using Postman for the Trello API. The tests cover common use cases such as creating, updating, and deleting boards, lists, and cards in Trello. It includes a Postman collection for different Trello API endpoints and an environment for storing variables like API keys.

## Technologies Used
<img src="https://user-images.githubusercontent.com/25181517/192109061-e138ca71-337c-4019-8d42-4792fdaa7128.png" title="POSTMAN" alt="POSTMAN" width="40" height="40" style="max-width: 100%;">


  
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/d5cb6f8e77a7f5a092c20719323115c658b1260da976663f11d698ca66514c64/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e65776d616e2d436f6d6d616e645f4c696e652d627269676874677265656e"><img src="https://camo.githubusercontent.com/d5cb6f8e77a7f5a092c20719323115c658b1260da976663f11d698ca66514c64/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e65776d616e2d436f6d6d616e645f4c696e652d627269676874677265656e" alt="Newman" data-canonical-src="https://img.shields.io/badge/Newman-Command_Line-brightgreen" style="max-width: 100%;"></a>

- Postman
- Newman


## Project Structure

- **/collections/**: Contains the Postman collection files that define the API requests and contains the test scripts.
- **/environment/**: Contains the Postman environment file for managing API keys and Trello-specific variables.

## Requirements

- [Postman](https://www.postman.com/) You can use the Postman desktop app or the Postman web UI.
- Regardless of whether you choose the desktop app or the web UI, you can use all of the collection’s requests and your changes are synchronized between the two environments so you can easily switch between them at any time.
- A Trello account and an API key/secret, which can be obtained from the [Trello Developer Portal](https://trello.com/app-key).
- Newman: You can install Newman using Node.js. Make sure you have Node.js installed, and then run the following command:
  ```bash
   npm install -g newman

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/DinaMagdyS/PostmanTrello.git
2. Install the project dependencies:
Install newman-reporter-htmlextra: 
npm install -g newman-reporter-htmlextra


## Usage
  ### Running Tests in Postman
  1. After importing the collection and environment, you can run the requests individually to interact with the Trello API.
  2. You can also run the entire collection using the Postman Collection Runner to execute all API tests at once.
  3. Use the Postman console to debug and inspect responses from the Trello API.
 
  ### Running Tests via Command Line using Newman
  You can also run the tests via the command line using Newman. Use the following command to run a specific test suite, specifying the environment: 
  ```bash
newman run "TrelloAPIs Run.postman_collection.json" -e Trello_Env.postman_environment.json -r htmlextra
