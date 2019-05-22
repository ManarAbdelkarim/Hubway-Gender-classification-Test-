# Hubway-Gender-classification-Test-
Hub way Trips data:
• Filtered male \female from blank variables(empty)
• Birth date and zip code removed due to the small amount and huge amount
missing.
• All rest data no blank variables in it.
• Balance the male and female amount through filter. Male was (314722), Female
was (103974)
• Remove start date and end date since we would like to predict duration suitable
for male and female not months and seasons.
• Convert seconds to min to make it more reasonable.
• Subscription type & Status are not required since they are unbalanced and noisy
data will add only nothing since its one class.
6
• From station number we merge both datasets to add station name and station
location.
• Remove two end stations because their status are “Removed”.
1. Duration :The length of the trip, in seconds. We wanted to use
the duration to look at what sort of trips riders were taking. We
wanted to define each trip as either a leisure ride or a purposeful
ride. For our purposes, we converted this to minutes, eliminating
any trip that was less than 60 seconds. (Often, those trips are
"trials" by people(
2. Start + End Stations :Each station has a unique ID number as
well as the station name. The start station is where the bicycle is
checked out from and the end station is where the bicycle is
checked back into. We can use the end station information to
ensure the riders are students.
3. Location name: the street the contains Hubway stations. We need
to know which station is near to a university or a central library
domain.
1. Preprocessing contains many sub-process:
• Define target ( we chose gender to be our label)
• Should discretize? (we desecrated single: Age > type of data)
• Map values
• Remove column? (We removed selected column that we do not need
it).
2. Replace missing value: in 4 steps we replace nominal, positive infinity,
negative infinity and numerical missing values by "missing"
3. Recorder attributes (we ordered columns alphabetically "ascending")
4. Filter examples
