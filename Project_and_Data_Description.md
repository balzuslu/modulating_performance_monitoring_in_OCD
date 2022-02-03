<!--
Project and Data Description
-->

## Project Overview
&nbsp;

- In this preregistered study, we investigated the effects of tDCS (transcranial direct current stimulation) on performance monitoring in patients with obsessive-compulsive disorder (OCD) and healthy individuals. Cathodal and sham tDCS was applied over the presupplementary motor area (pre-SMA) in two separate sessions, each followed by EEG recording during performance of a flanker task. 

&nbsp;

## Procedure 
&nbsp;

- The study employed a randomized, double-blind, sham-controlled, crossover design. Patients with OCD and matched healthy control (HC) participants were invited for two experimental sessions and received one session of cathodal and one of sham tDCS.
	- The cathodal electrode was positioned over the pre-SMA (electrode site FCz) and the anodal reference electrode was placed on the right cheek. 
	- In the active tDCS condition, a direct current of 1.5 mA was administered for 20 min. In the sham condition, the current was applied for only 40 s at the beginning of the 20 min period. 

&nbsp;

- Following the stimulation, participants performed an arrow version of the flanker task while EEG was recorded.
	- Stimuli consisted of five vertically arranged arrows pointing to the left or right.
	- Participants were instructed to indicate the direction of the central target arrow as quickly and accurately as possible by button press. 
	- The central target arrow was flanked by arrows pointing in the same direction (50% congruent trials) or by arrows pointing in the opposite direction (50% incongruent trials). 

&nbsp;

## Hypotheses 
&nbsp; 

- We expected that inhibitory pre-SMA stimulation by cathodal tDCS would reduce performance monitoring processes, leading to increased error rates and attenuated behavioral adaptation after error commission, that is, reduced post-error slowing (PES).
&nbsp;

- In addition, we hypothesized that compared to sham tDCS, cathodal tDCS would reduce the error-related negativity (ERN) amplitude. 
&nbsp;

- Regarding group differences, we predicted increased ERN amplitudes in patients with OCD compared to healthy participants in the sham condition. 
&nbsp;

- We expected the ERN attenuation to be more pronounced in the patient group compared to the control group. 
&nbsp;

- To explore effects of tDCS on performance monitoring during correct responses, we additionally analyzed the correct-response negativity (CRN). 
&nbsp;

- Moreover, we examined whether cathodal tDCS would increase the amplitude of the error positivity (Pe).

&nbsp;

## Preregistration
&nbsp;

- Hypotheses, experimental design, sample size, and analysis plan of this study were preregistered on the Open Science Framework (https://osf.io/7z8hj/).

&nbsp;

## Data Description  
&nbsp;

- Data set: 'Single_Trial_Data.rda' 
- 53760 observations (56 participants, 2 sessions per participant, 480 trials per session), 13 variables

&nbsp;

| VARIABLE                                      	| DESCRIPTION                                                                             | VALUES                                                                                               |
|-------------------------------------------------------|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| participant_id                                    	| Participant identifier                                                                  | C_01 to C_30 and P_01 to P_30                                                                        |
| group                                        	        | Participant group                                                                       | HC = healthy control participant <br> OCD = patient with OCD                                         |
| session                                    	        | Experimental session                                                                    | T1 = first experimental session <br> T2 = second experimental session                                |
| stimulation                                    	| Stimulation condition                                                                   | verum = cathodal tDCS <br> sham = placebo tDCS                                                       |
| trial                                         	| Trial number within the flanker task                                                    | 1 to 480 per participant and session                                                                 |
| stimulus_type                                         | Stimulus type in the flanker task                                                       | congruent = congruent stimulus <br> incongruent = incongruent stimulus                               |
| response_type                             	        | Response type in the flanker task                                                       | correct = correct response <br> incorrect = incorrect response <br> miss = missing response          |
| rt                                        	        | RT in the flanker task                                                                  | RT in milliseconds <br> NAs for trials in which no response was made (miss)                          |
| rt_log                                	        | Log-transformed RT in the flanker task                                                  | log(RT) in milliseconds <br> NAs for trials in which no response was made (miss)                     |
| rt_invalid                                	        | Indication whether RT in the flanker task was < 100 ms or > 800 ms                      | TRUE <br> FALSE <br> NAs for trials in which no response was made (miss)                             |
| MFN_0_100_FCz                                 	| Medial-frontal negativity (MFN); response-locked ERP from 0 to 100 ms at electrode FCz  | Mean amplitude in microvolts <br> NAs for trials with EEG artifact                                   |
| Pe_200_400_Pz                                 	| Error positivity (Pe); response-locked ERP from 200 to 400 ms at electrode Pz           | Mean amplitude in microvolts <br> NAs for trials with EEG artifact                                   |
| P3_300_500_CPz                                        | P300; stimulus-locked ERP from 300 to 500 ms at electrode CPz                           | Mean amplitude in microvolts <br> NAs for trials with EEG artifact                                   |
 
&nbsp;
