### Instructions to create a repo from git CLI using terminal

#### Create a folder in you machine and cd into it

```
mkdir crft && cd crft # create a repository from the terminal and cd into it
```
#### Create at least a file call "README.md" in your machine

```
echo "# This is the README file" > README.md
```
#### Create a file .gitignore
```
cat >> .gitignore <<EOL

# Ignore the configuration files


# Ignore other files

*.DS_Store

EOL
```

#### (1) First step - generate the link between local and remote repos
```
curl -u 'calliari' https://api.github.com/user/repos -d '{"name":"crft"}'
```
Terminal will ask the details for credentials from git, type your github password

#### (2) Second step - …or create a new repository on the command line

```
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/Calliari/crft.git
git push -u origin master

```

Done, check your Github repositories, a new repo is created with the name "crft" under profile name
