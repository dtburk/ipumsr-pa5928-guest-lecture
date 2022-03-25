[Start at ipums.org, and make sure you are not logged in.]

If we start at ipums.org, we see all the IPUMS data collections. For this 
example, we'll create an IPUMS USA extract, so the first step is to click into 
the IPUMS USA website.

[Click into IPUMS USA website.]

From the IPUMS USA homepage, we can click the "Get Data" button to start 
building our extract.

[Click "Get Data" button.]

The main tasks in building an extract are choosing samples and variables. You 
can do this in any order, but it often makes sense to choose samples first so 
that you can see what variables are available for the samples you're interested 
in. So I'll click the "Select Samples" button here.

[Click "SELECT SAMPLES" button.]

In our examples later in the presentation, we analyze access to a phone line by
geography and education, so let's create an extract we could use for that
analysis. I'll select the 2019 ACS as my most recent year [unclick "Default
sample for each year", and check box for 2019 ACS], because the 2020 ACS has
comparability issues related to the pandemic, as is noted by this tooltip here
[hover over the 2020 ACS info icon], then I'll grab a sample from the beginning
of each decade going back to 1960.

[Check boxes for 2010 ACS, 2000 5%, 1990 5% state, 1980 5% state, 1970 1% state
fm1, and 1960 1%; then click "SUBMIT SAMPLE SELECTIONS" button.]

Next, let's grab a household geography variable, which we'll find under the 
"Household" menu in the "Geographic" category.

[Navigate to Household > Geographic.]

Here we see a wide range of geographic variables and the availability of those
variables across our selected samples. An "X" indicates that the variable is
available for the sample; the blue "i" icon indicates that the variable is
available in a different sample from the same year; and a tiny dot indicates
that the variable is not available for any samples in that year.

First let's select the STATEFIP variable, which will tell us which state each 
household resides in, by clicking the plus sign to the left of the variable 
name.

[Click the plus sign to add STATEFIP to cart.]

We also want to select a lower level geography variable to map. Unfortunately,
the boundaries of some of these geographic units change over time, and since we
want to be able to map phone availability over time in with consistent
geographic units, we want to use a harmonized geographic variable like CONSPUMA
down here. We can see that CONSPUMA is available for 1980 through 2010. Let's
click on CONSPUMA to see more information about it.

[Click on CONSPUMA.]

From the description, we can see that CONSPUMA, which stands for "consistent
public use microdata areas," identifies the most detailed areas that can be
consistently delineated from 1980 to 2011. The description also includes a link 
to the separate page where you can download shape files with the boundaries 
corresponding to these units.

[Hover over the "CONSPUMA Geographic Tools page" towards the bottom of the 
description.]

Along the top of the CONSPUMA variable page, there is a lot more information 
about this variable organized into tabs.

[Click on Codes, Comparability, and Universe.]

For now, let's just add this variable to our "Data Cart" by clicking the 
"Add to Cart" button.

[Click the "ADD TO CART" button.]

Notice that our Data Cart has updated to indicate that we have selected 1 
variable and 7 samples.

To continue choosing variables, we can click the "SELECT DATA" link at the top 
of the page to return to the top level variables page.

[Click the "SELECT DATA" link at the top of the page.]

In addition to browsing the variable menus as we did to find our geography
variable, we can also use the variable search feature.

[Click the "SEARCH" button.]

As you can see, the search feature by default searches across variable names, 
labels, value labels, and descriptions, and only includes harmonized variables, 
which are variables that have been made consistent across samples. If we search 
for "phone", we should find any variable pertaining to access to a phone line.

[Type "phone" in the search box and click "SEARCH".]

This first variable named "PHONE" looks good, and it's available across all the 
samples we've selected, so let's add it to our cart by clicking the plus sign to 
the left of the variable name.

[Click plus sign to add "PHONE" to cart.]

Now let's use the search feature to find an education variable.

[Click Search button. On Search page, enter "education" in the search box and 
click the "SEARCH" button.]

Here we see there are a lot of variables that mention education, so we have to 
skim over the variable labels to find what we want, which is this "Educational 
attainment" variable down here. Let's add it to our cart.

[Click the plus sign to add "EDUC" to our cart.]

Now that we've got our geography, phone access, and education variables, we are 
ready to submit our extract for processing. The first step in doing that is to 
click the "VIEW CART" link up here.

[Click the "VIEW CART" link.]

Here we see that in addition to the variables we added to our cart, there are a
number of preselected variables that are useful for most analyses, such as the
sample identifier variable "SAMPLE" and the household identifier variable
"SERIAL". If we've got all the variables and samples we want, we clicked "Create
Data Extract".

[Click "CREATE DATA EXTRACT" button.]

Before submitting our extract, we have a few more useful options, which you can 
see under the "OPTIONS" heading. One of the options I want to highlight here is 
the "SELECT CASES" option. Notice that we have an estimated extract size here 
right above the OPTIONS heading, and it's saying that our data file is likely to 
be about 4GB, which is pretty large, and might be slow to analyze. Depending on 
the analysis you are planning, it's often useful to reduce the size of your data 
file by limiting it to just the cases that you are interested in. For this 
example, we're going to limit our extract to only households from Minnesota. To 
do that, we first click the "SELECT CASES" button.

[Click "SELECT CASES".]

Next, we select the variable or variables that we want to use to select cases. 
For this example, we just need to select the STATEFIP variable.

[Click the check box for "STATEFIP", then click SUBMIT.]

Finally, we can select the values that we want to include in our dataset. If we 
select only the value for Minnesota, our data file will only include households 
from Minnesota, which should make the size of our dataset much more manageable.

[Scroll down to and select Minnesota, then click SUBMIT.]

Now we just add a description for our extract, "Phone availability over time in 
Minnesota", then click Submit.

[Add description and click SUBMIT. You should be taken to the log in screen.]

So, you don't need an IPUMS account to browse the data and build an extract, but 
you do need an account to submit that extract request and actually download the 
data. The first step is to create an account, which you can do from here or from 
the IPUMS USA home page.

[Click "Create an account" link.]

By filling out this registration form, you will be registering for access to 
IPUMS USA, but if you want to use data from other IPUMS data collections, you 
will have to complete a separate registration form. If you're using the data for 
a course assignment, make sure to mention that in the "General Research 
Statement" field, and also give a brief description of the analysis you are 
planning.

[Click the back button.]

Since I already have an account, I can log in to finish submitting my extract.

[Log in, then click SUBMIT EXTRACT. Submitted at 11:33am.]

You'll get an email when your extract is ready to download. This extract ended 
up including 860,000 records and 15 variables, and when I submitted it last 
week, it took about 12 minutes to process. Bigger extracts can take up to 
several hours to complete. If I wouldn't have limited cases to Minnesota only, 
I would have had over 50 million records, which would have taken a few hours to 
process and would have been difficult to analyze, so it's good to keep that 
select cases option in mind.

[This script took me about 10.5 minutes when I practiced it.]
