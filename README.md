# udacity-project-1
My first project for the Udacity Data Scientist Nanodegree program.

## Summary
When asked to work on a dataset for my Data Scientist Nanodegree program from Udacity, I chose to work with the StackOverflow 2017 survey data we used in the class. As discussed in more detail in the project notebook here and on my [Medium post](https://medium.com/@reed.anzalone/is-coding-the-great-equalizer-1b1b3ad5b62f), I took a deep dive into whether code development education could be a democratizing force, by looking in detail at how developer salary interacts with education and other factors.

I reorganized the `FormalEducation` and `HighestEducationParents` columns from the dataset to reduce the number of groups and make them easier to visualize. In doing so, I found that salary generally increased as a function of the respondent's education and their parents' education.

I also split the data set into responses from developed and developing countries and looked at whether we could draw any conclusions about whether coding allows people to break generational barriers better or worse in the developed world than in the developing world.

Finally, I looked at whether there are other factors that could contribute more to success than education alone. 

### Noteworthy Things

When normalizing data, I subtracted the mean and divided by the standard deviation. In different circumstances, though, I used different means and different standard deviations, so it's important to note that not all of the plots are comparable amongst each other in terms of absolute value. 

### Future Work

For this specific project, there are a couple of functions (`group_plot` and `single_group_plot`) that sort of do the same thing. I was having a hard time making `group_plot` work for using `groupby` with a single column, so I just made another function to make it work. Going back, I'd put in some more effort to make it `group_plot` work right in the first place.

Also, obviously, the questions I posed on Medium are pretty high and mighty and are not answered entirely by this dataset -- or really probably any single dataset. There's lots more work to be done there.

## Files
- Project1.ipynb, a Jupyter Notebook containing the code used to analyze the data and generate plots.

*Note: I did not include the survey results or survey schema files here because I was having trouble uploading them onto GitHub. See the dependencies section below for where I obtained the data.*

## Dependencies
- Standard Conda libraries (pandas, numpy, matplotlib)
- [StackOverflow 2017 survey results](https://www.kaggle.com/stackoverflow/so-survey-2017)

## Acknowledgements
Thanks to 

