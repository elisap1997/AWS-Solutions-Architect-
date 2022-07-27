# Cognito

Decentralized managed authentication

signup siginin integration for apps

social identity provider eg fb and google

Cognito User Pools
  - user directory
  - authentication to IpD to grant access to our app

Cognito Identity Pools
  - provides temporary credentials
  - for users to access aws services

Cognito Sync
  - syncs user data and preferences across all devices

## Web Identity Federation

Web Identity Federation
  - exchanges identity and security info
  - btwn identity provider (IdP) and an app

Identity Provider (IdP)
  - trusted provider of your user identity
  - allows you to authenticate access to other services
  - examples: FB, Amazon, Google, Twitter, Github, Linkedin

Types of Identity Providers
  - tech behind indeitty providers
  - e.g. security asserion markup language (SAML), Single Sign On (SSO), OpenID Connect (OIDC) OAuth  (used by Github, for web identity federation)
  
## User Pools

user directories used to manage actions for web and mobile apps such as signup/signin/account recovery/account confirmation

allows users to sign in directly to user pool or using web identity federation

uses aws congnito as identity broker between aws and identity provider

successful user authentication generates json web token (JWTs)

user pools can be thought of as account used to access the system (email address and password)

choose what attributes, password requirements

apply mfa

restrict whether users are allow to sign up on their own or need admin verification

analytics with pinpoint for user campaigns

trigger custom log via lambdas after actions such as user signup

## Identity Pools

provide temp aws credentials to access services eg s3 dynamodb

acutal mechaniasm authorizing access to aws resources

choose who to provide access to, use sdk to get temp credentials

## Sync

sync user data and preferences across devices w one line of code

push sync used to push updates and synchronize data

uses simple notification service (SNS) to send notifications to all user devices when data in the cloud changes
