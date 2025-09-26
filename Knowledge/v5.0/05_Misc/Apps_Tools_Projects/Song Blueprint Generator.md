# AI-Powered Song Blueprint Generator

A web application that uses AI (via AI-SDK smart provider routing and openai_base_url compatible provider APIs for model selection with BYO api keys) to automatically generate detailed song blueprints from song titles and lyrics.


Providers Integrated (default):

- OpenRouter via AI-SDK (openai base url drop in replacement, 200+ models, dynamic model availability pulls all models from their models api, model selection can be narrowed down by user for specific features such as cost per tokens, release date, and more)
- Gemini API via AI-SDK (openai base url drop in replacement, user api key, model selection from drop down menu of dynamically fetched api offerings from [https://ai.google.dev/gemini-api/docs/models](https://ai.google.dev/gemini-api/docs/models)



## Features

- Account / Profile Setup
    - username (email), password
    - settings:
        - ai settings: setup openai api compatible base url, save api key safely
        - default ai model settings selections: broken down by task (advanced) or single model for all processes (simple)
        - 
- 
- Song BluePrints from Lyric Analysis
    - lyric text inputs:
        - title
        - style of music (optional)
        - lyrics to analyze
        - additional context (user provided / optional layer of context or instructions to further tailor generated blueprint)
    - pre analysis ai menu with optional settings if user wants to edit them from default setup
        - features a green or red status light to signal that the AI is set up and ready or it says what the user needs to still provide to complete the setup / or notifies what changes need to be made to ai configuration to address api error messages -- essentially this is a live status / health indicator to reduce failed api calls
        - AI settings: model, temperature, max tokens, top p, top k, banned/restricted word)
        - setup and settings save button behind passworded user account
    - Song Blueprint generation settings:
        - Title: DO / DO NOT INCLUDE title from original song in the blueprint
        - Style of Music and Metatag Guidance: [Include / Exclude]
        - Output Style: Specifies how the AI should generate stylistic elements and how specific the additions should be.
            - Specificity of AI-generated Additions: [normal or high]
            - Inclusion of Original Lyrics: [avoid or strict exclusion] (If 'Strict Exclusion' is selected, the AI processing the song and developing the blueprint must not use even a single phrase or keyword from the original lyrics, to preserve originality and encourage critical creative thinking.)
                - Normal: guidance provided at the section level with a suggested rhyme scheme and syllable count pattern, examples given sparingly
                - High: template guides users line by line with prescribed rhyme scheme, syllable counts, and broad theme and energy metatag guidance with examples

        The default options for these setting if user does not wish to customize are:

        - title included
        - style of music and metatag guidance included
        - output style: normal specificity, avoid inclusion of original song lyrics, and normal guidance level
    - Response should be provided in sections so that if the user wishes a certain edit or alteration be made the entire response is not lost or reproduced
    - Save Button: takes the sectioned response and merges them together into a markdown song template for the user to download and stores the data in a JSON as part of the user data and made available in a library of completed Song BluePrints that can be called on for later downstream songwriting tasks or to edit.
    - Advanced: allow users to upload song blue prints by filling in a form that generates a JSON and saves the user data for downstream songwriting or edits. 

## Tech Stack

- Frontend:
- Backend:
- AI: AI-SDK (smart routing for many providers and integrations)
- Build:
- 