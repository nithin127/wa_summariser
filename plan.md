
1. Clean sentences
2. Do NER to collect all the named entities. For each entity we gather context from Google and store it. 
3. With a chatGPT API call, we can figure out if that message belongs to any of the previous topics -- if it does, we append that message (along with the googled context) to the topic.

In the end, we'll have a bunch of topics, messages, and context for each entity within that message. Then we do an API call to summarize each topic.