 Usages:
   thumbsup [required] [options]
   thumbsup --config config.json


Required:
  --input   [string] [required]
  --output  [string] [required]

Output options:
  --thumb-size            [number] [default: 120]
  --large-size            [number] [default: 1000]
  --photo-quality         [number] [default: 90]
  --download-photos       [choices: "large", "copy", "symlink", "link"] [default: "large"]
  --download-videos       [choices: "large", "copy", "symlink", "link"] [default: "large"]
  --download-link-prefix  [string]
  --cleanup               [boolean] [default: false]
  --concurrency           [number] [default: 4]
  --gm-args               [array]
  --watermark             [string]
  --watermark-position     [choices: "Repeat", "Center", "NorthWest", "North", "NorthEast", "West", "East", "SouthWest", "South", "SouthEast"]

Album options:
  --albums-from            [array] [default: ["%path"]]
  --sort-albums-by         [choices: "title", "start-date", "end-date"] [default: "start-date"]
  --sort-albums-direction  [choices: "asc", "desc"] [default: "asc"]
  --sort-media-by          [choices: "filename", "date"] [default: "date"]
  --sort-media-direction   [choices: "asc", "desc"] [default: "asc"]

Website options:
  --index                 [default: "index.html"]
  --albums-output-folder  (default: website root)  [default: "."]
  --theme                 [choices: "classic", "cards", "mosaic"] [default: "classic"]
  --theme-path            [string]
  --theme-style           [string]
  --title                 [default: "Photo album"]
  --footer                [default: null]
  --google-analytics      [string]

Deprecated:
  --original-photos     Copy and allow download of full-size photos  [boolean] [default: false]
  --original-videos     Copy and allow download of full-size videos  [boolean] [default: false]
  --albums-date-format  How albums are named in <date> mode [moment.js pattern]  [default: "YYYY-MM"]
  --css                 Path to a custom provided CSS/LESS file for styling  [string]

Options:
  --version      Show version number  [boolean]
  --help         Show help  [boolean]
  --config       JSON config file (one key per argument)  [string]
  --log          Print a detailed text log  [choices: null, "info", "debug", "trace"] [default: null]
  --usage-stats  Enable anonymous usage statistics  [boolean] [default: true]
  --dry-run      Update the index, but don't create the media files / website  [boolean] [default: false]


 The optional JSON config should contain a single object with one key
 per argument, not including the leading "--". For example:
 { "sort-albums-by": "start-date" }
