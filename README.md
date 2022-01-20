### Oregon state students need gpu resources to run code ###
srun -p gpu --gres=gpu:1 --pty bash

##Some basic setup not important for running the code##

mkdir GraphExplainability    #this is the name of your directory \
cd /GraphExplainability \
git init \
touch readME.md   #this is to create an initial file to push \
git commit -m "created readme" \\

git remote add origin git@github.com:YOUR_USERNAME/myDirName.git \
curl -u USERNAME:PASSWORD https://api.github.com/user/repos -d '{"name":"myDirName"}' #this will create the repo in github. \
git push -u origin master