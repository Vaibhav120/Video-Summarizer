# Video-Summarizer

### Application
Like the webinars are too long approx. 1-2 hours.
Attending the full webinar might not be possible all the times.
So using this, you can achieve a audio/text summary, include the key points.
This can have many more applications for researchers/teachers etc.
This can work the link of any downloadable link, YouTube video link and, Google cloud sharing link as well.

### Working
Takes downloadable link to video/audio/text as input.
---Video to text---
Extraction of audio from video is done.
Now, this audio is broken to small chunks, based on pauses, like "." .
Then audio chucks are converted to text sentences using Google's Speech Recognition API.
These sentences are merged together to form a complete text of content.
Extractive summary is made from this text.
---Implementation of Extractive Summary---
TF-IDF tokenization of the text.
Now, sentences are tokenized.
Based on the word_tokens those sentences consists, they are assigned weight.
30% sentences with highest weight are considred for summary.
---Text to Audio---
Finally, this summary is converted to audio using Speech Synthesis API.
