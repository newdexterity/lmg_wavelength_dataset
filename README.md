# lmg_wavelength_dataset

This dataset contains lightmyography data from 10 subjects using different light wavelength configurations.

Each file is named subj{number}_{light_configuration}{repetition}_lmg.csv

Where {number} is the subject number

{light_configuration} is either green, ir, 250both or 125both referring to the light configuration
- green light only
- ir light only
- both green and ir lights blinking alternately at 250ms
- both green and ir lights blinking alternately at 125ms
  
{repetition} is the repetition number from 1 to 5

In each file, the first row is a header numbering each column from 0 to 40.

Columns 0 to 39 inclusive is each of the 40 LMG channels, the value is the measured voltage.

Column 40 is the gesture label from 0 to 5 (rest, pinch, tripod, full, key, extension).

Subject Information including age, sex, handedness, and the order of data collection is found in **SubjectInfo.xlsx**


###################################################################################################################
UPDATE 30/07/2025

This dataset has been expanded to include lightmyography data from 21 subjects.
The same wavelegnth configurations have been used, however instead of gesturing, grip force data was collected.
This data can be found in LMGDataForce

Similarly, each file is named subj{number}_{light_configuration}{set}_lmg.csv

{set} is the set number from 1 to 2 represent which set of data was collected, 1 at quarter of the participants maximum force, and 2 at half the participants maximum force.

Columns 0 to 39 inclusive is each of the 40 LMG channels, the value is the measured voltage.

Column 40 is a trigger label from 0 for resting and 1 when the subject is applying force.

Column 41 includes the force data collected using a dynamometer.

Subject Information including age, sex, handedness, maximum force and the order of data collection has been included in **SubjectInfo.xlsx**
