https://www.youtube.com/watch?v=kwtHOkf7Jdg
(6:50 in)
Install adapter in 'exploring-typesense' project path
$ pnpm add typesense-instantsearch-adapter


Copy books to project path

Initialize the data
populate import.js

% Run script
$ node import.js



Run the app with pnpm
$ pnpm start


Remember to uncompress books.jsonl.gz file
$ gzip -d books.jsonl.gz







<!-- View csv and json -->
brew install saulpw/vd/visidata
vd books.jsonl.gz