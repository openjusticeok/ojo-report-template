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

## Examples

Here is an example of a customized version of the template: 

![image](https://user-images.githubusercontent.com/56839927/228943717-cd888a12-b0f0-4929-9b3e-0dca44834157.png)

Here's how I made it:

1) I navigated to the directory I wanted the report in (in this case it was `Github/diversion-hub/inst/reports/metrics-report/`) in the terminal.
2) I ran `quarto use template openjusticeok/ojo-report-template`, which cloned the template repo and generated a `.qmd` file, plus all the necessary extensions / styling (most of which will be in `/_extensions/`). If you just open and run the resulting `.qmd` file, you should see the generic template version of the OJO report. 
3) I customized the template by editing the `yaml` at the top of the `.qmd` file (for exmaple, I set `title-block-banner` to match DHub's green color, and `logo` to the DHub logo instead of the OJO one). I also wanted to change a few more specific things, so I edited the SCSS variables at the top of `/_extensions/openjusticeok/ojo-report-template/custom.scss` so I could change the title / subtitle text colors individually. Once you've cloned the template with `quarto use template openjusticeok/ojo-report-template`, you can go nuts and change anything you want!
