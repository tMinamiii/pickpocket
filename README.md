# Pick

 Pick is able to search sites in your Pocket and open browser.

[![Image from Gyazo](https://i.gyazo.com/993a78fd1fc4828ada433a79514f3e35.gif)](https://gyazo.com/993a78fd1fc4828ada433a79514f3e35)

## Installation

``` sh
go get -u github.com/tMinamiii/pick
```

### WSL

You need wsl-open. and add PATH to powershell.exe

``` sh
npm i -g wsl-open
export PATH=/mnt/c/Windows/System32/WindowsPowerShell/v1.0/:$PATH
```

## Usage

### Create Pocket Cosumer Key

Access https://getpocket.com/developer/apps/ and **CREATE AN APPLICATION**

1. input `Application Name`(e.g. pick)
2. Check Permission `Retrieve`
3. Check Platform `Desktop (other)`
4. Check `I accept the Terms of Service`
5. Push **CREATE APPLICATION**, then generate consumer key.

### Auth Pocket

``` sh
pick keygen <Pocket Consumer Key>
```

Generate authorization token file in `$HOME/.config/pick/key.json`.

### Run Pick

``` sh
pick
```

## Motivation

 Pocket is one of very useful service, however we keep storing favorite
or read later site.  We often only add site and never visit it. Pick helps
search titles ( and contets if you are premium user ) in your Pocket sites and
open browser directly.
