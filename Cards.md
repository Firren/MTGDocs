# Cards

All functions will return an array with one or more objects.

## Get by Id

/cards/id/:id

If you want to find the id for a card you can try to do a search against the API by card name, explained later in this chapter.
The id can also be found by searching for a card at http://gatherer.wizards.com/Pages/Default.aspx. 
You will get a link looking like the value of gatherer_link below. 

### Response

```json
[
  {
    "id":"235595",
    "name":"Abbey Griffin",
    "gatherer_link":"http://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=235595",
    "power":"2",
    "toughness":"2",
    "set":"Innistrad",
    "type":"Creature — Griffin",
    "cost":"3W",
    "converted_manacost":"4",
    "artist":"Jaime Jones",
    "flavor":"The darkness crawls with vampires and ghouls, but we are not without allies.",
    "number":"1",
    "rarity":"Common",
    "rating":"2.422",
    "rules_text":"Flying, vigilance",
    "gatherer_img":"http://gatherer.wizards.com/Handlers/Image.ashx?multiverseid=235595&type=card",
    "votes":"45"
  }
]
```

## Get by Name

/cards/name/:name

### Response

Looks the same as for id above with the exception that the array can contain multiple (card) objects.