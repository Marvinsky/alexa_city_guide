
Steps to create enviroment development

1.- Create Environment

    > sam init --runtime python3.6 --dependency-manager pip --name Alexa-City-Guide

2.- Install dependencies

    > Select environment created by the manager packages you want
    > CD city/
        > run pip install -r requirements.txt


2.- Update template.yaml
    
    > set CodeUri: city_guide/
    > set Handler: app.lambda_handler
    > set Runtime: python3.7
    > set Role: arn:aws:iam::XXXXXX

3.- how to get SkillId alexa?
    
    * Go to Alexa developer console and Click view Skill ID. 
    amzn1.ask.skill.9524a157-da01-4d73-abe8-60f2a70e30c6

4.- Update steps-deploy commands

5.- Go to https://developer.amazon.com/alexa/console -> Endpoint :
    
    > Select AWS Lambda ARN: Set default Region
    
    > Obtain Default Region:
        > Go to https://console.aws.amazon.com/lambda
        
        > Copy ARN
        
6.- Test the skill:  Alexa open city guide