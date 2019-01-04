# mac-provisioning-scripts

```
export USER_FULL_NAME=

brew update
brew cask install intellij-idea webstorm docker spectacle spotify visual-studio-code
brew install git jq

git config --global user.name “$USER_FULL_NAME”

git config --global user.email “$USER@klarna.com”

./add-git-aliases

# TODO: dockerize that specific project's build
brew install node@8
echo 'export PATH="/usr/local/opt/node@8/bin:$PATH"' >> ~/.bash_profile
export PATH="/usr/local/opt/node@8/bin:$PATH”
brew install yarn
```
