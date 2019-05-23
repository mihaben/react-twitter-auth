[![NPM](https://nodei.co/npm/react-twitter-auth.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/react-twitter-auth/)

[![npm](https://img.shields.io/npm/dt/react-twitter-auth.svg)](https://img.shields.io/npm/dt/react-twitter-auth.svg)
[![Build Status](https://travis-ci.org/GenFirst/react-twitter-auth.svg?branch=master)](https://travis-ci.org/GenFirst/react-twitter-auth)
[![Code Climate](https://codeclimate.com/github/GenFirst/react-twitter-login/badges/gpa.svg)](https://codeclimate.com/github/GenFirst/react-twitter-login)
[![Coverage Status](https://coveralls.io/repos/github/GenFirst/react-twitter-auth/badge.svg?branch=master)](https://coveralls.io/github/GenFirst/react-twitter-auth?branch=master)
[![npm version](https://badge.fury.io/js/react-twitter-auth.svg)](https://badge.fury.io/js/react-twitter-auth)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

# React Twitter Authentication Component

> A React Twitter oAUth Sign-in / Log-in Component for React, implemented with Apollo

## Installation

`npm install mihaben/react-twitter-auth`

## Usage

```jsx harmony
<TwitterLogin
  onFailure={this.onFailed}
  onSuccess={this.onSuccess}
  requestTokenQuery={REQUEST_TOKEN_QUERY}
/>
```

Custom content that overrides default content:

```jsx harmony
<TwitterLogin
  onFailure={this.onFailed}
  onSuccess={this.onSuccess}
  requestTokenQuery={REQUEST_TOKEN_QUERY}
  showIcon={true}
>
  <b>Custom</b> Twitter <i>Login</i> content
</TwitterLogin>
```

## Options

|      params       |  value   |    default value     |                                  description                                   |
| :---------------: | :------: | :------------------: | :----------------------------------------------------------------------------: |
|        tag        |  string  |        button        | tag that should be used to create element that will be used as loging element  |
|       text        |  string  | Sign in with Twitter |                      text that will be shown in component                      |
| requestTokenQuery | function |                      |                            gql (graphql-tag) query                             |
|     onFailure     | function |                      |          function that will be called if user cannot be authenticated          |
|     onSuccess     | function |                      |        function that will be called with `{oauthToken, oauthVerifier}`         |
|     disabled      | boolean  |        false         |                               disable component                                |
|       style       |  object  |                      |                                  style object                                  |
|     className     |  string  |                      |                            class name for component                            |
|    dialogWidth    |  number  |         600          |                                  dialog width                                  |
|   dialogHeight    |  number  |         400          |                                 dialog height                                  |
|     showIcon      |   bool   |         true         |                         should default icon be visible                         |
|     children      |   node   |                      |     this props can be used in order to override default component content      |
|    forceLogin     |   bool   |        false         |         force user to authenticate with Twitter username and password          |
|    screenName     |  string  |                      | prefills the username input box of the OAuth login screen with the given value |

# License

react-twitter-auth is released under [MIT License](https://opensource.org/licenses/MIT).
