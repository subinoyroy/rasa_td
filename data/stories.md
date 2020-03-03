## hospital search happy path
* greet
  - utter_how_cah_I_help
* search_provider{"facility_type":"hospital","location":"Arizona"}
  - action_facility_search
* thanks
  - utter_goodbye

## hospital search + location
* greet
  - utter_how_cah_I_help
* search_provider{"facility_type":"hospital"}
  - utter_ask_for_location
* search_provider{"location":"New York"}
  - action_facility_search
* thanks
  - utter_goodbye

## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot