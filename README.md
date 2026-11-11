# Mutation patterns in treated and control samples of fission yeast
## Aim:

The aim of this program is to identify and compare DNA mismatches in six samples of yeast. Half are treated with a genotoxic agent, and the other half are untreated controls. 

## How to access and run:

The program is a Google Colab file that can be accessed in the main branch of this repo, and there should be a button in the preview to open it directly in Colab.

## Inputs and outputs:

The expected inputs are the provided sequences of all six samples; tests can also be done with self-made data. The outputs for the final bit of the Colab should produce a summary table, a substitution table, and three result sentences for Welch's test.

## Code design:

For the summary function, I decided to make a function within it to separately print out the summary tables. I took the variable that I stored the summary data in and put it into the table function. I made sure invalid reads weren't utilised at any point by doing if statements, and in the case a read wasn't valid, a message would print out without crashing the program. In the summarise function, I also decided to write out each substitution combination straight into the sample summary dictionary so I can just do a short if statement to find the key and add to that substitution count.

## Testing:

I ran some normal case tests to make sure valid data was accepted. Also did some edge cases to see how they would handle unexpected data, and this helped me improve the robustness of my compare function as I added some code in case of "None" values. I also did some length tests to make sure my loops were working correctly and storing data in dictionaries and lists without overwriting anything


