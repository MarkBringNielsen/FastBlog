# Getting binder to work with fast.ai
These are my tips that helped me get it up and running. Firstly, I need to state that I mostly just followed [this](https://github.com/butchland/fastai-binder-app-template) guide by Butch Landingin. I did however meet a couple of minor hickups and that is what I'm going to explain how to fix. Secondly, I did these things on Paperspace so I cannot speak to how my tips work on Colab. So here are my tips:

When you come across the part where you set up git on paperspace meaning this part:
 * `git config --global user.name "<Your name>"`
 * `git config --global user.email "<email@address>"`
 
I absolutely recommend just doing that right away.

When you get to installing git-lfs just follow the instructions for Ubuntu/Debian except that you do not have sudo rights on paperspace so just leave the sudo out of the commands.

Next in step 7 before running the git commands change to the directory of your git repo:
```
%cd <your-copy-of-fastai-binder-app-template>
```

And lastly when setting up the binder remember to get these two things right.
- Set the path to an URL path at the dropdown next to "Launch"
- Have that path be /voila/render/your-notebook.ipynb


![](https://raw.githubusercontent.com/markbringnielsen/binder_test/master/images/binder.PNG)
