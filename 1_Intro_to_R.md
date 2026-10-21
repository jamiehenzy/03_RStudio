## Get started with swirl ##

Swirl is a program run within R (or RStudio) that introduces you to R features and commands.

### Get set up for the tutorial ###
Request an RStudio session from Explorer, using the OOD interface. Tip: set the time to 2h instead of the default 1h.

Once you've connected to the RStudio server, work in the console window. 

Install swirl:
```
install.packages("swirl")
```
and load the library, with instructions to save a log of your work during (use this command before every session of swirl):
```
library(swirl)
swirl_options(swirl_logging = TRUE)
```
Begin the session by typing:
```
swirl()
```

Follow the prompts and select "R Programming" for the course. Work through the 15 lessons. If you do not complete all lessons in one session, just be sure to include the "swirl_options" command above each time you load the library.

When you are finished with all 15 lessons (even if you've done them in different sessions), find the data and zip it:
```
user_dir <- file.path(find.package("swirl"), "user_data")
zip("swirl_logs.zip", list.files(user_dir, recursive = TRUE, full.names = TRUE)
```
The zipped file can be pushed to your Github account when you submit your module work.
