
```markdown
# SpotDL

SpotDL is a command-line tool for downloading songs from Spotify using various input methods. It utilizes the `spotdl` Python package.

## Installation

To install SpotDL, use the following pip command:

```sh
pip install spotdl
```

## Usage

SpotDL provides flexible options for downloading songs from Spotify.

### Download by Command Line

To download songs using the command line, you can use the following syntax:

```sh
spotdl [options] [urls]
```

Replace `[urls]` with the Spotify URLs of the songs you want to download.

**Example:**
```sh
spotdl https://open.spotify.com/track/your_track_id
```

### Download by Python Module

You can also use SpotDL as a Python module:

```sh
python -m spotdl [urls]
```

### Advanced Options

You can use various options to customize the download process:

- `--format` or `-f`: Specify the desired output format (e.g., mp3, flac, m4a).
- `--output` or `-o`: Specify the output folder and file naming template.

**Example:**
```sh
spotdl --format mp3 --output /Folder/Subfolder/{title}.mp3 songlink
```

## Examples

### Download a Single Song

To download a single song, use the Spotify URL of the song as an argument:

```sh
spotdl https://open.spotify.com/track/your_track_id
```

### Download Multiple Songs

To download multiple songs, provide multiple Spotify URLs as arguments:

```sh
spotdl https://open.spotify.com/track/track_id1 https://open.spotify.com/track/track_id2
```

### Download with Custom Format and Output

To download a song with a custom format and specify the output folder structure, use the `--format` and `--output` options:

```sh
spotdl --format mp3 --output /Music/{artist}/{title}.mp3 https://open.spotify.com/track/your_track_id
```


