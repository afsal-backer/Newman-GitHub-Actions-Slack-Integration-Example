# API Test Automation with Newman, GitHub Actions, and Slack Integration
This repository contains the setup for a simple yet effective API test automation framework using Newman, GitHub Actions, and Slack. It demonstrates how to implement a CI/CD pipeline for running Postman collections and reporting results directly to a Slack channel.

## Overview
The project is based on the concept detailed in Afsal Backer's Medium article (https://afsalbacker.medium.com/a-simple-api-test-automation-setup-using-newman-github-actions-and-slack-f70cfa15efe3). 
It provides a straightforward way to automate API testing using Newman (a command-line collection runner for Postman), integrates with GitHub Actions for continuous testing, and sends test reports to a designated Slack channel.

## Features

Newman: Utilizes Newman for running Postman collections.
GitHub Actions: Implements GitHub Actions for automated test execution upon code pushes or pull requests.
Slack Integration: Sends test reports directly to Slack, allowing for immediate feedback and collaborative troubleshooting.


# Getting Started

## Prerequisites
A GitHub account.
A Slack workspace and channel for reporting.
Postman for creating and exporting API tests.

## Setup

Clone the Repository
cd into your repo 

### Postman Collection

Create your API tests in Postman and export the collection as a JSON file.
Place the exported collection in the repository.

### Slack Webhook
Create an Incoming Webhook in your Slack workspace.
Store the webhook URL as a secret in your GitHub repository settings.
GitHub Actions Workflow

The .github/workflows/main.yml file contains the GitHub Actions workflow.
Customize this file as needed to suit your testing strategy.

### Running Tests
Tests will be automatically executed on pushes or pull requests made to the repository.
Test results will be sent to the configured Slack channel.

