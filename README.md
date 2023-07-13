# AnimeOnegai Downloader NX

AnimeOnegai Downloader NX is capable of downloading videos from the *AnimeOnegai* streaming service.

## Legal Warning

This application is not endorsed by or affiliated with *AnimeOnegai*. This application enables you to download videos for offline viewing which may be forbidden by law in your country. The usage of this application may also cause a violation of the *Terms of Service* between you and the stream provider. This tool is not responsible for your actions; please make an informed decision before using this application.

## Prerequisites

* Mp4Decrypt >= 1.6.0.0 (https://www.bento4.com/documentation/mp4decrypt/)
* RE.exe (N_m3u8DL-RE) >= 2.0.0 (https://github.com/nilaoda/N_m3u8DL-RE/)
* ffmpeg >= 6.0.0 (https://www.videohelp.com/software/ffmpeg)
* MKVToolNix >= 78.0.0 (https://www.videohelp.com/software/MKVToolNix)

### Paths Configuration

By default this application uses the following paths to programs (main executables):
* `./mkvmerge.exe`
* `./ffmpeg.exe`
* `./re.exe`
* `./mp4decrypt.exe`

To change these paths you need to edit `bin-path.yml` in `./config/` directory.

## CLI Options

### Authentication

Open config.json and add your email and password.

### Get Show ID

* `--search <s>` sets the show title for search

### Download Video

* `-s <i> ` sets the language you want to download [es , ja]. 
* `-url` enter the url of the movie or series (if available)
* `-movie` This option will let the script know that you are trying to get a movie

### Utility

* `-h`, `--help` show all options

## CLI Examples

* `ao --search "cat"`
* `ao -s es -url https://www.animeonegai.com/es/details/Nrl72yko71qOjTpnw ` 
* `ao -url https://www.animeonegai.com/es/details/PxzELBoJxQjYrU3nQ -movie` 
