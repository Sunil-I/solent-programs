# Installing Maven
This is a short introduction on how to install Maven either on your personal machine or at a university machine should they not have it installed!

### Personal Machine
We have more freedom here since we have Admin rights, you will want to move the maven folder to `Program Files`. Once you have done, so you will want to make an environment variable in `PATH` to include the location of maven's bin folder e.g `C:\Program Files\maven\bin`

```
1) git clone --branch maven https://github.com/Sunil-I/solent-programs maven
2) Move maven to C:\Program Files\
3) Set up an enviroment variable in PATH to include C:\Program Files\maven\bin
```

### University Machine
Since we do not have admin rights we can't actually modify environment variables permanently or install maven to other C drive folders. So we will instead install maven in your own folder and set a temporary environment variable for it. Cloning the correct branch of this repo should give you all the tools to make this work easily.
```
1) git clone --branch maven https://github.com/Sunil-I/solent-programs maven
2) Test if maven is installed in the right place by running: %USERPROFILE%\maven\bin\mvn -version
3) Either run the bat file or run this command: set PATH=%PATH%;%USERPROFILE%\maven\bin
4) Test if this worked by running: mvn -version
```
**Note**: You should repeat steps 3 if you open a new command terminal since this only works for the same session! 

### Like using UNIX commands?
I am personally a fan of using UNIX commands over the normal windows command, since we have git installed we can technically use the bash commands outside the bash shell.
```
set PATH=%PATH%;C:\Program Files\Git\usr\bin
```