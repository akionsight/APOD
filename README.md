# APOD
Get and easily parse the APOD (Astronomy Picture Of The Day) from the NASA open API

## Dependency Installation
for Windows:- `pip install -r requiremnts.txt`

for MacOs:- `pip3 install -r requirements.txt`

Also get a Nasa api key by clicking here [here](https://api.nasa.gov/#signUp).
## How to use (Do Not skip)
1. import the file
```python
from APOD import nasa_apod
```
2. Now call the `get_data` function and pass the `nasa api key` as the argument. Note api_key is a string. The data returned will be a Dictionary. Now you can parse the dictionary too

```python 
data = nasa_apod.get_data(<your_api_key>)
```
### get_date

the `get_date` function takes the dictionary we got above and returns the date.

```python
date = nasa_apod.get_date(data)
```
### get_explaination
the `get_explaination` function takes the dictionary we got above and returns the explaintion.

```python
date = nasa_apod.get_explaination(data)
```
### get_hdurl
the `get_hdurl` function takes the dictionary we got above and returns the High Definition url of the image.

```python
date = nasa_apod.get_hdurl(data)
```
### get_title
the `get_title` function takes the dictionary we got above and returns the title of the image.

```python
date = nasa_apod.get_title(data)
```
### get_url
the `get_url` function takes the dictionary we got above and returns the Standard definition url of the image.

```python
date = nasa_apod.get_hdurl(data)
```
### get_media_type
the `get_media_type` function takes the dictionary we got above and returns the media type the file (might be a video of a image).

```python
date = nasa_apod.get_hdurl(data)
```

## Other functions
there are also other functions that might help you in situations

### download_image
the `download_image` finction takes the url (hdurl or url) and the date from the function `get_date` and downloads the image in the current directory and with the file name of the date. the image downloaded is in the .jpg format
```python
nasa_apod.download_image(url, date)
```

### convert_image
sometimes the image we downloaded above might not be in the right format (.jpg) so you may call `convert_image` function to convert the image into .png. takes the `image` parameter which is the filepath.
```python 
nasa_apod.convert_image(image)
```

for any other queries contact me on GitHub or my email.
please let me know if you built something with it, I would be very happy 😊
