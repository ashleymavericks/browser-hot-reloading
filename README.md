<div align="center">
<h1 align="center">Browser hot-reloading in FastAPI using arel</h1><br>
<img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"/><br><br>

 Implementaion of lightweight browser hot-reloading for Python ASGI web apps frameworks like FastAPI using [arel](https://github.com/florimondmanca/arel)
</div><br>

## What is arel?
arel can be used to implement development-only hot-reload for non-Python files that are not read from disk on each request. This may include HTML templates, GraphQL schemas, cached rendered Markdown content, etc.

## How does arel work?
arel watches changes over a set of files. When a file changes, arel notifies the browser (using WebSocket), and an injected client script triggers a page reload. You can register your own reload hooks for any extra server-side operations, such as reloading cached content or re-initializing other server-side resources.

## Installation guide
1. Install dependencies
```bash
pipenv install
```
or 
```bash
pip install -r requirements.txt
```
2. Set environment variable in your shell instance
```bash
export DEBUG=True
```
3. Verify it using
```bash
echo $DEBUG
```
4. Test this implementation, and further include it in your projects for a better development experience with Python ASGI web frameworks

## LICENSE
This project is licensed under the MIT license