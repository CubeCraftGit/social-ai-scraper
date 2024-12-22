All files will be uploaded for the user to give examples and add thier own implementations if interested.

# Twitter Scraper implementation for Ordigent

- see: https://gist.github.com/ordigent/7262442ba5e5e1a1c4ef945bca20ae38 for more information

## Contributing

We welcome contributions to this project. If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## Acknowledgments

We would like to thank OrdiSwap for partnership, implementation information, partnership and funding to make this project happen.

#Scraper

Pipeline for generating AI character files and training datasets by scraping public figures' online presence across Twitter and blogs.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Copy the `.env.example` into a `.env` file:
   ```properties
   # (Required) Twitter Authentication
   TWITTER_USERNAME=     # your twitter username
   TWITTER_PASSWORD=     # your twitter password

## Usage

### Twitter Collection
```bash
npm run twitter -- username
```
Example: `npm run twitter -- pmarca`

### Blog Collection
```bash
npm run blog
```

### Finetune
```bash
npm run finetune
```

### Finetune (with test)
```bash
npm run finetune:test
```
Example: `npm run generate-virtuals -- pmarca 2024-11-29`
Example without date: `npm run generate-virtuals -- pmarca`

The generated character file will be in the `pipeline/[username]/[date]/character/character.json` directory.
The generated tweet dataset file will be in `pipeline/[username]/[date]/raw/tweets.json`.
