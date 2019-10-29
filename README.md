# Email address image generator

This is a simple app that generates images containing text. It's intended initially to generate human readable emails, that cannot be easily crawled by robots, but can be used for any other purposes. 

## Installing

It is a Python 3 Flask application that requires Pillow and a font file. To install it, create a virtualenv and install the requirements, like below:

```bash
$ cd app
$ python3 -m venv .venv
$ source .venv/bin/activate
(.venv) $ pip install -r requirements.txt
```

## Running

To run the function, just initialize the flask app and query the address specified, providing the desired string as a parameter in the url. The response will be an image containing the string:

TODO: insert app output when running and curl command in a different terminal

## Deploying

Other than running locally, this app can be deployed as a Lambda/Cloud function in AWS or GCP. To do that, you need to have Terraform and run the following commands:

TODO: insert terraform deployment for both AWS and GCP

## Testing

TODO: Test

## Automating - CI/CD

This repo also contains the required config file for deploying it in a cloud environment in an automated manner, using CircleCI as a CI/CD environment. Having the CircleCI-GitHub link properly configured, every commit to the master branch in this repository will trigger the workflow and deploy a new version to the chosen cloud environment.
