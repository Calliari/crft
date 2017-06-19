### Instructions to create a repo from git CLI from terminal

#### Create a folder in you machine and cd into it

```
mkdir crft && cd crft # create a repository from the terminal and cd into it
```
#### Create at leat a file call README in you machine

```
echo "# This is the README file" > README.md
```

#### (1) First step - generate the link between local and remote  
```
curl -u 'calliari' https://api.github.com/user/repos -d '{"name":"crft"}'
```
Terminal will ask the details for credentials from git

#### (2) Second step - …or create a new repository on the command line

```
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/Calliari/crft.git
git push -u origin master

```

Done, check your github, a new repo is created
