# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

## 0.7.12 - 2022-02-03
- add `parseTwitterToMarkdown` and `createTwitterURL` to `@subsocial/utils`, for support parsing Twitter posts to Markdown and creating Twitter saved content provided by [Post4ever](https://post4ever.app)

## 0.7.10 - 2022-12-03
We have done really huge update of our SDK. Get feedback of our early

### Added
- definitions for Subsocial Parachain Node
- new methods for IPFS instance:
  - saveContentToIpfs
  - pinContent
  - unpinContent
- support custom headers for IPFS node:
  - setWriteHeaders
  - setPinHeaders
- add high level getter for:
  - `api.base` - get base no-serialized data from blockchain and IPFS
  - `api.blockchain` - get no-serialized data only from blockchain
  - `api.ipfs` - get IPFS instance
  - `api.substrateApi` - get ApiPromise instance
- add methods to `blockchain` instance for getting data from roles storages from blockchain:
  - getAccountsWithAnyRoleInSpace
  - getSpaceIdsWithRolesByAccount
  - getSpacePermissionsByAccount
- add method to `blockchain` instance for getting counter of storage:
  - postsCountBySpaceId
  - sharesCountByPostId
  - repliesCountByPostId
  - accountFollowersCountByAccountId
  - accountsFollowedCountByAccount
- add `filters` arg for `find(Space|Post)Structs` methods in Subsocial API
- add methods to `SubsocialApi`:
  - findSpaces
  - findPosts
  - findProfileSpaces
