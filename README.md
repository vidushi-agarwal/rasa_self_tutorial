![](rasax_healthcarebot.gif)
This bot tells the user about following health care facilities-
1. Hospital
2. Nursing Homes
3. Home Health Agency
at following cities namely Chicago, San Francisco and all other important cities around the world.

Try out the <a href="http://35.200.162.2/guest/conversations/production/94b86ec57ab44b8ba9c2ad4abbb5bd04"> bot</a> yourself.

## How do I use this directory?
Train the assistant using the command:  
`rasa train`

Test the assistant using the command:  
`rasa run actions & rasa shell`

## What do you need to follow?

This  requires you to have Rasa installed on your machine:  
```pip3 install rasa-x --extra-index-url https://pypi.rasa.com/simple```

In addition to this you need to install additional dependency to run Rasa on Jupyter 
notebooks:  
```pip install nest_asyncio```
