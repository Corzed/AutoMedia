# AutoMedia

AutoMedia creates short-form videos and automatically uploads them you youtube. 

###How it works:
It fetches the video that you are aiming to clip, it then sends the transcript to gpt3.5 api and asks what the most engading segment is. it then finds the associated time frame in the transcript and cuts the video using moviepy accordingly. It then uses ffmpeg and whisper to create another transcript (I know this is inefficient but its easier to do) for the cut clip and uses that transcript to add captions that are insync with the person speaking. This is best used for podcasts/interviews, for example joe rogan or lex fridman, or tv shows, like young sheldon.
