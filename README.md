# GH Pages

In order to make it work, gh-pages must be enabled, go to settings, click on "pages section" and once in pages section, look for *Branch* then leave it as the immage below.

![step-1](https://user-images.githubusercontent.com/47251170/184499600-5367203b-64b3-42b2-83c3-36b5298e2ed1.png)

![step-2](https://user-images.githubusercontent.com/47251170/184499603-58357774-7146-461f-aac0-32037d521f38.png)

![step-3](https://user-images.githubusercontent.com/47251170/184499605-702dba86-e9e4-4734-b3c8-f99e1b2c7953.png)

<br><br>


# GitBook

## Dependencies

[gitbook-cli](https://www.npmjs.com/package/gitbook-cli)

<br>

## How to install it?

```
$ npm install -g gitbook-cli
```

<br>

## Steps to test and modify it

1. Clone the project

2. Once in the project folder there will be 2 languages folders, *en* and *es*, each one with a **README.md** (*it will be the first page the user will see after choosing the language*) file.<br>
Also there will be other .md files, those are the pages that will be shown in the website. If Want to add a new chapter, a new .md file must be created, finally for it to appear on the site it must be added to **SUMMARY.md**

3. The new changes can be tested using the following command `$ npm gitbook build` followed by `$ npm gitbook serve`

4. If eveything is ok, the changes can be pushed to the remote repository using the following commands:


```
$ cp -R _book/* .
$ git clean -fx _book
$ git add .
$ git commit -m "commit"
$ git push origin main
```