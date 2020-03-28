## happy_path
* greet
    - find_facility_types
* inform{"facility_type": "xubh-q36u"}    
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
    - slot{"location":"Chicago"}
* inform{"facility_id": 4245}
    - find_healthcare_address
    - slot {"facility_address":"St. Marys Hospital"}    
    - utter_address
* thanks
    - utter_noworries

## happy_path_multi_requests
* greet
    - find_facility_types
* inform{"facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
    - slot{"location":"Chicago"}
* inform{"facility_id": "747604"}
    - find_healthcare_address
    - slot {"facility_address":"St. Marys Hospital"}    
    - utter_address
* search_provider{"facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
    - slot{"location":"Chicago"}
* inform{"facility_id": 4245}   
    - find_healthcare_address
    - slot {"facility_address":"St. Marys Hospital"}    
    - utter_address

## happy_path2
* search_provider{"location": "Austin", "facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
* inform{"facility_id": "450871"}
    - slot {"facility_address":"St. Marys Hospital"}    
    - find_healthcare_address
    - utter_address
* thanks
    - utter_noworries

## story_goodbye
* goodbye
    - utter_goodbye

## story_thankyou
* thanks
    - utter_noworries

    
## interactive_story_1
* greet
    - find_facility_types
* inform{"facility_type": "9wzi-peqs"}
    - slot{"facility_type": "9wzi-peqs"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "9wzi-peqs"}
    - slot{"facility_type": "9wzi-peqs"}
    - slot{"requested_slot": "location"}
* form: inform{"location": "El Paso"}
    - slot{"location": "El Paso"}
    - form: facility_form
    - slot{"location": "El Paso"}
    - form{"name": null}
    - slot{"requested_slot": null}
* inform{"facility_id": "453140"}
    - slot{"facility_id": "453140"}
    - find_healthcare_address
    - slot{"facility_address": "5950 Alameda Avenue, El Paso, TX 79905"}
    - utter_address
* inform{"location": "Amarillo"}
    - slot{"location": "Amarillo"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "9wzi-peqs"}
    - slot{"location": "Amarillo"}
    - slot{"location": "Amarillo"}
    - form{"name": null}
    - slot{"requested_slot": null}

## interactive_story_2
* search_provider{"facility_type": "xubh-q36u"}
    - slot{"facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "xubh-q36u"}
    - slot{"facility_type": "xubh-q36u"}
    - slot{"requested_slot": "location"}
* form: inform{"location": "New York"}
    - slot{"location": "New York"}
    - form: facility_form
    - slot{"location": "New York"}
    - form{"name": null}
    - slot{"requested_slot": null}
* inform{"facility_id": "330199"}
    - slot{"facility_id": "330199"}
    - find_healthcare_address
    - slot{"facility_address": "1901 First Avenue, New York, NY 10029"}
    - utter_address
* inform{"facility_type": "b27b-2uc7"}
    - slot{"facility_type": "b27b-2uc7"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "b27b-2uc7"}
    - slot{"location": "New York"}
    - slot{"facility_type": "b27b-2uc7"}
    - form{"name": null}
    - slot{"requested_slot": null}
* inform{"facility_id": "335522"}
    - slot{"facility_id": "335522"}
    - find_healthcare_address
    - slot{"facility_address": "30 West 138Th Street, New York, NY 10037"}
    - utter_address
* inform{"location": "Cape"}
    - slot{"location": "Cape"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "b27b-2uc7"}
    - slot{"location": "Cape"}
    - slot{"location": "Cape"}
    - form{"name": null}
    - slot{"requested_slot": null}
* inform{"facility_type": "b27b-2uc7"}
    - slot{"facility_type": "b27b-2uc7"}
    - facility_form
    - form{"name": "facility_form"}
    - slot{"facility_type": "b27b-2uc7"}
    - slot{"location": "Cape"}
    - slot{"facility_type": "b27b-2uc7"}
    - form{"name": null}
    - slot{"requested_slot": null}

