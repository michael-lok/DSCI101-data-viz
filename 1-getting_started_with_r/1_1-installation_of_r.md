## 1.1 Installation of R
Let's get started by preparing our device for use in the R language.

* Download the Interactive Development Enviroment (IDE) [RStudio](https://www.rstudio.com/products/rstudio/download/#download).
* Open RStudio via your Launchpad
  * I'd recommend keeping it in your dock, or at least remember you can easily open it up by pressing `Cmd + Space` and typing **RStudio**.
* At this point, you should see a screen similar to the one below. A few things to know about the RStudio IDE: It is a user interface (UI) that allows you to write new R code, view your existing environment (variables/objects you've saved for retrieval), navigate through your directory structure, and perform commands in your Terminal (we won't go over this in this course, but helpful to know).
* **Environment** The place where your defined R objects in the current session can be tracked. You'll learn later in this chapter that you can have a variable represent some value; the environment lets you keep track of what these variables are.
* **Files** This pane will show you the directory structure, starting at your user's Home directory. If you take a look at the screenshot, I've already navigated to the `DSCI101-data-viz` location on my computer. You'll want to do this each time you start an R session in this course.
* **Console** This is the pane that allows you to write/execute R commands, as well as see the output of particular functions.
* **Source** This currently isn't seen in the screenshot, but once you open up a file, a new pane will populate the top-left quadrant of your IDE. This is where we'll spend most of our time interacting and writing code.

![](/images/1-rstudio-start.png)

The beauty of RStudio (and many other IDEs) is that you can stay on one window and have access to everything you'll need for coding/analyzing in R (`R` in itself is simply a language, but RStduio provides the environment in which users can perform development, hence the term IDE).

### Setting Working Directory
When coding, your computer needs to have a point of reference of where it is executing commands. This is important when you are retrieving particular files. Imagine going to a friend's house and asking where you can get a hair dryer, and your friend resonds, "Just grab it from the top shelf". You'll know to look at *a* top shelf, but *which* top shelf? Is it the one in the living room? The one in your friend's parents' restroom?

Similarly, your computer needs to know definitively where you are performing your work. This reference point is generally called the **working directory**, and we can set it to the location of this project on your computer. If you look at the screenshot, you'll notice that I've stored this project in the `Home/projects/` directory. **To set you working directory:**

* Use the `Files` pane and navigate to your `DSCI101-data-viz` location. Your `Files` pane should look similar to mine, where the filepath is `Home>{additional subdirectories>DSCI101-data-viz`.
* Click `More > Set As Working Directory`. You should notice that a command is executed in your `Console` that set the working directory to this project.

![](/images/1-setwd.png)


If you want to check that you're in the right working directory, let's write our first R command! In your `Console`, go to the next available line and type in the following command:

```r
getwd()
```

![](/images/getwd.png)

We're all set to start coding! Let's move on to the next section.