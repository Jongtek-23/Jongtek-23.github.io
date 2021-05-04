## Welcome to GitHub Pages

### NAMP
Basic scan to know wich ports are open
```
nmap -p- --open -T5 -v -n <IP> -oG allPorts
```

If the scan is slow, we launch this:
```
nmap -p- -sS --min-rate 5000 -vvv -n -Pn <IP> -oG allPorts
```

To grep ports from allPorts
`cat allPorts | grep -oP '\d{1,5}/open' | awk '{print $1}' FS="/" | xargs | tr ' ' ','`

To copy on the clipboard 
`xclip -sel clip`


You can use the [editor on GitHub](https://github.com/Jongtek-23/Jongtek-23.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Jongtek-23/Jongtek-23.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
