Run the bot in the terminal:
```
rasa shell
```

To get a new project:
```
conda create -y python=3.7 --name rasa 
conda activate rasa  
pip install rasa==2.6.2
rasa init
```

Change the contents of the files (nlu, domain, stories)

```
rasa data validate
rasa train --fixed-model-name contact_bot 
```

Note: \
Rasa x not supported anymore \
Won't recognize the names which weren't trained before
