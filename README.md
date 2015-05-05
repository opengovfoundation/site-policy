# site-policy

Website policy documents as originally used in [Madison](https://mymadison.io) by [The OpenGov Foundation](http://opengovfoundation.org/).  All of these documents are being released with open licenses, meaning they're **absolutely free to use**.  This will allow any person or organization - **for profit or not for profit** - to copy, edit, rewrite, and distribute them at no cost!  They are [Creative Commons CC0 Licensed](https://creativecommons.org/publicdomain/zero/1.0/), dedicating them to the public domain.

## Disclaimer
This was created based on United States law, and if you're not in the US the policies here might not be legal wherever you are.

We are not lawyers, and cannot give you legal advice or tell you what is best for your organization.  You should have an actual lawyer review these documents before you use them in the first place.  If you have any questions, ask a lawyer.

We cannot be held responsible for any legal trouble that these documents get you into.  You're using them of your own accord.  We're providing them as-is with no warranty.  Seriously, please don't sue us.

## Available Files

The following files are available in a variety of formats - use the links below to download them directly.

Document | | | | |
--- | --- | --- | --- | --- |
Privacy Policy | [Markdown](https://rawgit.com/opengovfoundation/site-policy/master/markdown/privacy-policy.md) | [HTML](https://rawgit.com/opengovfoundation/site-policy/master/html/privacy-policy.html) | [PDF](https://rawgit.com/opengovfoundation/site-policy/master/pdf/privacy-policy.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/site-policy/master/docx/privacy-policy.docx)
Terms of Service | [Markdown](https://rawgit.com/opengovfoundation/site-policy/master/markdown/terms.md) | [HTML](https://rawgit.com/opengovfoundation/site-policy/master/html/terms.html) | [PDF](https://rawgit.com/opengovfoundation/site-policy/master/pdf/terms.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/site-policy/master/docx/terms.docx)
Copyright | [Markdown](https://rawgit.com/opengovfoundation/site-policy/master/markdown/copyright.md) | [HTML](https://rawgit.com/opengovfoundation/site-policy/master/html/copyright.html) | [PDF](https://rawgit.com/opengovfoundation/site-policy/master/pdf/copyright.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/site-policy/master/docx/copyright.docx)

## Contributing

We welcome suggested edits to these documents!

We use Markdown as the primary format for these files, so you'll need to know a little before you begin. Don't worry - it's easy!  [Here's a quick guide.](https://guides.github.com/features/mastering-markdown/) If you've used a wiki, reddit, etc. it should be easy to pick up.  *Note that we _cannot_ accept changes directly made to other formats, only Markdown.*

If you don't want to learn Markdown and still want to contribute, feel free to [open an issue on this repo](./issues), or just [send us an email](mailto:sayhello@opengovfoundation.org).

### The Easy Way ###
You can edit the files directly using the links below, no account or GitHub experience needed!

*Coming Soon!*

### The Advanced Way ###
If you are familiar with GitHub, please fork the repo and send a pull request.

We use [pandoc](http://pandoc.org/) to generate the many formats we display.  If you don't have pandoc installed, that's ok!  Just send us a pull request with the updated markdown files.

If you have pandoc installed with pdfLaTeX, you can run the following command from the repository root to generate these files:

    for myfile in $( ls ./markdown ); do echo Converting $myfile; for fmt in html docx pdf; do filetrim=${myfile%???}; pandoc -o "./"$fmt"/"$filetrim"."$fmt -f markdown "./markdown/"$myfile; done ; done

