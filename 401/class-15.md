# Spring Security Architecture

## Authentication and Access Control

Application security boils down to two more or less independent problems: authentication and authorization 

## Authentication

The main strategy interface for authentication is : 
>public interface AuthenticationManager {

 > Authentication authenticate(Authentication authentication)
  >  throws AuthenticationException;
> }


An AuthenticationManager can do one of 3 things in its authenticate() method:

1. Return null

2. Throw an AuthenticationException

3. Return an Authentication

## Customizing Authentication Managers

Spring Security provides some configuration helpers like : AuthenticationManagerBuilder

## Authorization or Access Control

AccessDecisionManager : 

> boolean supports(ConfigAttribute attribute);

> boolean supports(Class<?> clazz);

> int vote(Authentication authentication, S object,
   >     Collection<ConfigAttribute> attributes);

   ## Web Security

   Spring Security based on Servlet Filters

   ## Creating and Customizing Filter Chains

   You can switch it off completely by setting security.basic.enabled=false 

   ## Request Matching for Dispatch and Authorization

   Once the decision is made to apply a particular filter chain, no others are applied.

   ## Combining Application Security Rules with Actuator Rules

   