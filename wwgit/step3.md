In this step you need github account and repository, let create it first okay. Btw you have 2 option for auth git. First, using https - this needed authentication after push command. Second, using ssh - not needed auth after push. In this tutorial using https.

## Task
1. Make sure you have created repository in github. Exxample, i have remote repository in https://github.com/andrimuhyidin/katacoda
2. Connecting to repository with `git remote add https://github.com/andrimuhyidin/katacoda-tutorial`{{execute}} Please change the address according to what you have.
3. When the file has been committed, just push to your remote repository with `git push origin master`{{execute}}, But it seems to be an error, because actually you have to be full to synchronize, you can force push with `git push -f origin master`{{execute}}. You need to auth with username & password github.
4. Have done, good job.