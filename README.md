# ET_Labeller
A python based framework and GUI to label eyetracking data based on the emanalyser framework creted by charlie connell. Provides a way to analysis a full file of eyetracking data for analysis or labelling to train ML models.

It recieves a pickle dictionary that can have a flexible data structure to take different types of raw data files but there must be another data structure that converts it to the ET_Data framework wihich contains at least the 5 columns. t-time, x - x-coordinate, y - y-coordinate, status - status of etdata quality, evt - event type.
       Below are the event types
        0: 'gray',  #0. Undefined
        1: 'b',     #1. Fixation
        2: 'r',     #2. Saccade
        3: 'y',     #3. Post-saccadic oscillation
        4: 'm',     #4. Smooth pursuit
        5: 'k',     #5. Blink
        9: 'k',     #9. Other

There are multiple optional columns that can be included but not requred, these include, pupil_height, pupil_width, pupil_size.
