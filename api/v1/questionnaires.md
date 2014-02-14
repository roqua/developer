API v1: Questionnaires
==============

Access the questionnaires available in the system

## Retrieve the dossier of a given patient:
    GET /api/v1/questionnaires/{:questionnaire_key}

Provide de following parameters:

 * `questionnaire_key` - The Quby key of the questionnaire

example result:

```json
{
   "key":"quby_key",
   "title":"Questionnaire title",
   "description":"",
   "outcome_description":"",
   "short_description":"",
   "panels":[
      {
         "class":"Quby::Items::Panel",
         "title":"Panel title",
         "items":[
            {
              "class":"Quby::Items::Question",
              "key":"v_1",
              "title":"Question described here",
              "description":null,
              "type":"textarea",
              "validations":[

              ],
              "unit":null,
              "hidden":false,
              "display_modes":null,
              "default_invisible":false,
              "viewSelector":"#item_v_1",
              "parentKey":null,
              "parentOptionKey":null,
              "deselectable":false,
              "autocomplete":"off"
            }
         ]
      }
   ]
}
```
