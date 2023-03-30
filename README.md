# OJO HTML Report Format

![image](https://user-images.githubusercontent.com/56839927/228921367-a3169b70-1eff-4ee2-9c23-9a7df7f8697c.png)

## How to install / use

When you sit down to start a new report, you can copy the template and all needed by navigating to your working directory and using the following terminal command:

```bash
# Be sure to navigate to the right place first with `cd my/working/directory`
quarto use template openjusticeok/ojo-report-template
```

This will install the extension and create an example qmd file that you can use as a starting place for your report / article / whatever.

## Using

*TODO*: Describe how to use your format.

## Format Options

The template includes the following configuration options in the yaml header:

* A `title`, `subtitle`, `logo`, and `description` to display in the banner at the top
* `author`, `date` (set to use the current date by default), 
* `abstract` and `abstract-title` can be used to create an executive summary, etc. before the body
* `number-sections` automatically numbers the section headers / TOC, `smooth-scroll` makes the scrolling behavior nicer, and `knitr: opts_chunk: fig.align: center` just sets the default behavior for figures / images in the body.

For a full list of available configuration options, see https://quarto.org/docs/reference/formats/html.html
