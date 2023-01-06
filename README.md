## Maven Build and Release Action

This github action is fairly simple, create a .github directory and then a workflows directory inside of that, then put the YAML file from here inside of it. You will need to change a few things depending on your preference. 

```yaml
file:
```

You need to set this to target/<whatever the name of the jar is when you build it locally, make sure to put the .jar at the end!

```yaml
asset_name:
```
You need to set this to whatever you want the released jar file to be called. Also dont forget to put the .jar at the end of it.

```yaml
tag:
```
You need to get this to whatever tag you want to use. If you just want to use the master tag put ${{ github.ref }}

```yaml
overwrite:
```
This boolean determines whether the current release should be overridden with the updated jar instead of publishing a whole new release. If set to false it will create a new release each time


Thats basically it, if you have any questions just like, hmu lol
