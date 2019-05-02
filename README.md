# tapas.io WebComic downloader
Unofficial downloader for webcomics on Tapas.io with automatic resume, written in PHP.

Saved images get filenames like "mainCounter-episode# episodeTitle.ext"


## Prerequisites:
The only requirement is a compatible working php interpreter.
I'm using `php-7.1.8-Win32-VC14-x64.zip`.
let me know if it works on other OSs.

## Usage:
1. Get episode number to start from.
 * Go to the comic you want to download (usually the first page).
 * Copy the integer from the current URL.
 * Examples: `https://tapas.io/episode/255222`  ->  `255222`
2. Start the download.
 * Usage of `tapas.io_downloader.php`:
 ```
 tapas.io_downloader.php -e <EP#> -p <path>
 ```
 * Windows example:
 ```
 C:\php\php.exe tapas.io_downloader.php -e 255222 -p D:\WebComics\Erma
 ```
 * The script will create the folder(s) if neccessary and store/save all images/objects of the comic in it.
 * If the folder already exists, it will resume downloading with/after the last saved episode.
