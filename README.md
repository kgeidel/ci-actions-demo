## MSDS434 Module 10: Github CI actions demonstration

An experiment to test CI/CD principles using Github actions.

I am in section 55 (Winter '25.) This is my week 10 demonstration. <br>
Please visit my <img src="https://kstatic.googleusercontent.com/files/d57b24106c34c7e50ef3d98423b94ddaf35ad2da73a9b9d4d12f52dbb9dd4c08c2957f6255ab8690d5ef0b32cff8287e09577d05e479d263e872160c4c9e8363" height="20" width="20">[Google Drive Folder](https://drive.google.com/drive/folders/1so_fM2HcdTYzCYSuwtdbxBeXtx1CPN8J?usp=sharing) for the weekly demonstration videos.

### Replication

```shell
# Fork the repo (you wont be able to push to my repo w/o a pull request) 
# Once you have your own repo SSH url replace mine below.
# Clone your fork and enter the repo
git clone git@github.com:kgeidel/ci-actions-demo.git && cd ci-actions-demo

# Make sure the script is executable
chmod u+x some_script.sh

# Run the script as is...
./some_script.sh

# Now make some changes to the script...
# For example, append an echo command:
echo "echo SOME TEXT THAT WILL BE RECOGNIZED AS NEW" >> some_script.sh

# re-run the script to confirm the changes are present
./some_script.sh

# Push the changes to trigger the CI action
git commit -m "Changes that should trigger CI"
git push

```

### Troubleshooting

* Did you fork the example repo? Or are you trying to push to mine?
* Are you on a system with bash or similar shell?
* Did you need to escape a character in your added echo command?
* Try editing the shell script in an editor if you are picking up unescaped characters using the append by redirect (`>>`).
* Is your git configured for pushing/pulling? Credentials in place?

### Testing CI/CD pipeline


