# Downloading a lot of PDFs

Sometimes you'll have a big list of PDFs that you want to download. Maybe you'll eventually run them through Tika or tesseract or something, but for now: we need to download them!

## Downloading a list of files

The best way to download a list of files is using `wget`. You can install `wget` on OS X with `brew install wget`, and on Windows I think [this is the best option](https://www.jcchouinard.com/wget/#Download_Wget_on_Windows).

After it's installed, make sure you have a file formatted with **one complete URL on each line**, like below.

```
https://www.example.com/file-1.pdf
https://www.example.com/file-2.pdf
https://www.example.com/file-3.pdf
```

Then you can use the `wget` command to download each one of the files.

```
wget -i urls.txt
```

## Creating a list of files from a dataframe

Maybe you have a dataframe where one of the columns is your URL.

|name|code|url|
|---|---|---|
|ABC|123|https://www.example.com/file-1.pdf|
|XYZ|456|https://www.example.com/file-2.pdf|
|LMN|789|https://www.example.com/file-3.pdf|

How do you export the `url` column into a list of URLs? You just need to tell `to_csv` to only save the column you're interested in, and not to write any header or index information.

```python
df.to_csv("urls.txt", columns=['url'], header=False, index=False)
```

Now you're all set to use `wget -i urls.txt`!