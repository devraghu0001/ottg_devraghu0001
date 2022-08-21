# Obey The Testing Goat - 21st August 2022


# Branch first.. Basic Git commands

How to Clone? (get a fresh repository in local box)
```
git clone git@github.com:kanchiraghuraman/ottg.git
```

How to branch?

```
git checkout -b users/ini/20220821_prerequisites
```

Save changes
```
git add -A
git commit -am "Some context message"
```

Send changes to repository
```
git push --set-upstream origin users/ini/20220821_prerequisites
```


# Lesson 00: Prerequisites

Install python

mkdir /src/learning/YYYYMM

```
mkdir /src/learning/202208

mkdir /src/learning/202208/ottg

cd /src/learning/202208/ottg

git init

code .
```

# Setup python virtual environment

Ensure you are in the correct folder/directory.
Create Virtual Environment with name **venv**
```
python -m venv venv
```
Activate Virtual Environment
```
.\venv\Scripts\Activate.ps1
```
Note: if you see error text in red with message like Unauthorized access. You will have to follow this additional steps to allow running powershell scripts.

Error Message: .\venv\Scripts\Activate.ps1 : File C:\src\learning\202208\venv\Scripts\Activate.ps1 cannot be loaded because running scripts is disabled on this system. For more information, see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170.

```
<!-- Get-ExecutionPolicy -->
<!-- Get-ExecutionPolicy -List -->
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Deactivate Virtual Environment
```
<!-- .\venv\Scripts\deactivate.bat -->
deactivate

```