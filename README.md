# espresso-cucumber-sandbox

Example setup of User Acceptance Tests for Andorid.

Main tools used are Cucumber for building test scenarios, and Espresso for instrumentation.

## usage

clone it to your local repository

```git clone git@github.com:paddyzab/espresso-cucumber-sandbox.git```

navigate to repo

```cd espresso-cucumber-sandbox```

run the tests

```gradle connectedAndroidTestUatsDebug```

## scripts
Or use one of two convinience scprits provided in /scripts folder.
I am using [gdub](https://github.com/dougborg/gdub) for convinience. 
If you do not want to use it modify scripts to start wit gradle instead of gw.

## tags
Setup supports filtering based on tags.

### tags
Tags are arbitrary gouping tool, which allows you to attach tests to keyword. 
For convinience, for example you may want to group tests for performance testing, synchronisation or other
more sensitive groups.
Annotate the such test with ```@tag``` and you're good to go.
To run grouped tests use one of convinence scripts and pass as a parameter tag you want to run with:
```./uat-tag performance``` or directly from gradle ```gradle connectedAndroidTestUatsDebug performance```



