# wsrc-melon
A Melon Web Source for Mp3tag.
<br><br>

# What it does
Parses album information from [Melon](https://melon.com) using the [Web Source Framework](https://help.mp3tag.de/main_online.html) provided by Mp3tag.

# Installation
Ensure that [Mp3tag](https://www.mp3tag.de/en/) is installed.

Copy the .src files into the sources folder located in:<br>
> %AppData%\Roaming\Mp3tag\data\sources

# Usage
Navigate to Tag Sources > Melon.
<br>
For Melon Lyrics, it's recommended to parse with Melon.src first to obtain the song ID for an easier lookup.

# Parsed Tags _(10/12/2020)_
The following tags are retrieved from the source:
<br>

| Name              | Tag               | Notes
| ----------------- | ----------------- | -----------------
| Album Artist      | %ALBUMARTIST%     | 
| Artist            | %ARTIST%          | 
| Copyright         | %COPYRIGHT%       | 
| Cover             |                   | The album artwork.
| Genre             | %GENRE%           |
| Melon Artist ID   | %MELONARTISTID%   | The unique artist identifier for each track.
| Melon Song ID     | %MELONSONGID%     | The unique song identifier for each track. Can be used with Melon Lyrics.
| Publisher         | %PUBLISHER%       | 
| Track #           | %TRACK%           | 
| Year              | %YEAR%            | Parsed in the format YYYY.MM.DD

<br>
Multiple tag values are delimited by a comma.
