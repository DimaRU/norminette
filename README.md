# norminette for 42 schools, Xcode compatible

## Install:

Requires python3.7+ (3.7, 3.8, 3.9)

### Directly inside your global commands

Install using pip.
```shell
python3 -m pip install --upgrade pip setuptools
python3 -m pip install norminette
```

To upgrade an existing install, use
```shell
python3 -m pip install --upgrade norminette
```

### Inside a virtual environment

Using a virtual environment will avoid version conflicts with already globally installed packages.

```shell
python3 -m venv venv
source venv/bin/activate
pip install norminette
```

## Usage

```
norminette
```
Runs on the current folder and any subfolder

```
norminette filename.[c/h]
```
Runs on the given filename(s)

```
norminette --xcode
```
Xcode compatible output

```
norminette --xcode --lenient
```
Xcode compatible output and downrgade errors to warnings

```
norminette -d
```
Prevents stopping on various blocking errors

```
norminette -dd
```
Outputs all the debug logging

## Docker usage

```
docker build -t norminette .
cd ~/42/ft_printf
docker run -v $PWD:/code norminette /code
```
