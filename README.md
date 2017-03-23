This repository stores a working resume, written in markdown. Combining this
with css files for styling, it can be translated into html format using
`pandoc` with the following command:

`pandoc --standalone -c css/style.css -c css/fonts.css --from markdown --to html -o resume.html resume.md`

I then make a printable pdf document from this with `wkhtmltopdf` using

`wkhtmltopdf -L 1mm -R 1mm -T 1mm -B 1mm --page-size Letter resume.html resume.pdf`
