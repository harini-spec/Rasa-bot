Reference: https://towardsdatascience.com/building-a-chatbot-with-rasa-3f03ecc5b324

Run the bot in the terminal:
```
conda create -y python=3.7 --name rasa 
conda activate rasa  
pip install -r requirements.txt
rasa train --fixed-model-name contact_bot 
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
