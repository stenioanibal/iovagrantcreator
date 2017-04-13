# IOVagrant Creator

Create a complete project structure using Vagrant, VVV and Zsh running `wpinit` command!

This command build a basic structure to init or clone one Wordpress Project to your Vagrant machine using VVV, including:

- **Automatically** create nginx .conf files
- **Automatically** define hosts in vvv-config.yml file
- Clone wordpress-default folder
- Option to delete and create blank wp-content folder
- Option to run Vagrant Provision on complete steps
- Option to change default host created
- Option to edit default wp-config.php file or create new with **Database Information**
- Option to change default table prefix in wp-config

### Clone this

To clone this project, follow this steps sequence:

1 - Run this command:

```
curl https://raw.githubusercontent.com/stenioanibal/iovagrantcreator/master/iovagrantf > ~/.iovagrantf --silent
```

2 - Paste this code into your `.zshrc`, present in `~` folder

```
cd ~
sudo vim .zshrc
```

```
# IOVagrant Creator
IOVDIRECTORY=~/.iovagrantf
source $IOVDIRECTORY
```

After, run `wpinit` command and use these features! 

### Options

```
-h: Show help infos
-cvd: Change Vagrant Directory
```

### Important Infos

- Enter the path of the vagrant from the root. Ex: `/Users/JohnDoe/Vagrant/wordpress/`
- Never ever enter `www` folder to Vagrant Directory!
