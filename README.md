# norminette for 42 schools, Xcode compatible

## Install:

requires python3.7

```shell
pip3 install -r requirements.txt
```


To install, simply run

```shell
python3 setup.py install
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
