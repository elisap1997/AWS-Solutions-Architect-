# IAM

manages access of aws users and resources

## Core Components

iam identities - users, groups,and roles
  - users: end users who log into console or itneract with aws resource programmatically
  - groups: group up your users so they all share permission levels of the group (eg admin, dev, auditors)
  - roles: associate permissions and then assign to users or groups

policies - attached to iam identities, json documents, grant permissions for specific user/group/role to access services

users can belong to group, roles can be applied to groups to quickly add and remove permissions en-masse to users

inline policy - policy directly attached to user

roles can have many policies attached

various aws resources allow you to attach roles directly to them

## Types of Policies

managed policies
  - managed by aws
  - cannot edit
  - labeled w orange box
  
customer managed policies
  - created by customer
  - editable
  - no symbol beside them
  
inline policies
  - directly attached to user

## Policy Structure

Version - states policy language version

Statement - container for policy element, can have multiple

Sid - optional, way of labeling statements

Effect - set whether policy will allow or deny

Principal - account/user/role/federated user would like to allow or deny access

Action - list of actions policy allows or denies

Resource - resource to which action applies

Condition - optional, circumstancies which policy grants permission

## Password Policy

set minimum requirements of password, rotate passwords so users have to update password after x days

## Access Keys

allow users to interact with aws service programmatically via aws cli or sdk, only allowed two per user 

## Multi-Factor Authentication

can be turned on per user, but user has to turn it on bc admin cannot directly enforce, admin can create policy to require mfa to acces certain resources

## Follow Along

go to dashboard

take what security status says into account

have to set up mfa with compatible devices
