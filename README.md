# mac-provisioning-scripts

```
export USER_FULL_NAME=
export USER_EMAIL=

brew update
brew bundle install

git config --global user.name "$USER_FULL_NAME"
git config --global user.email "$USER_EMAIL"

./add-git-aliases

echo 'export PATH="/usr/local/opt/node@8/bin:$PATH"' >> ~/.bash_profile
echo '[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion' >> ~/.bash_profile


echo >> ~/.bash_profile '
if [ -f "/usr/local/opt/bash-git-prompt/share/gitprompt.sh" ]; then
  __GIT_PROMPT_DIR="/usr/local/opt/bash-git-prompt/share"
  source "/usr/local/opt/bash-git-prompt/share/gitprompt.sh"
fi
'

```
