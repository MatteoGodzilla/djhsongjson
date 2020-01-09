# djhsongjson
JSON file format for custom tracks made for the DJ Hero series of games and the tools provided for them.

## What's in the repository

#### README.md
This file. Documentation for the file.

#### song.json
Example file with empty, zero or false values for all fields.

## Structure
- ``song`` - *This and all contents required.*
  - ``first`` - ``table``
    - ``name`` - ``string``
    - ``artist`` - ``string``
    - ``album`` - ``string``
    - ``genre`` - ``string``
    - ``year`` - ``int``
  - ``second``
    - ``name`` - ``string``
    - ``artist`` - ``string``
    - ``album`` - ``string``
    - ``genre`` - ``string``
    - ``year`` - ``int``
  - ``dj`` - ``string``
  - ``charter`` - ``string``
  - ``song_length`` - ``float``
  - ``preview_start_time`` - ``float``
  - ``preview_end_time`` - ``float``
- ``difficulty`` - ``table`` - *This and all contents required.*
  - ``bpm`` - ``float``
  - ``deck_speed`` - ``table``
    - ``deck_speed_beginner`` - ``float``
    - ``deck_speed_easy`` - ``float``
    - ``deck_speed_medium`` - ``float``
    - ``deck_speed_hard`` - ``float``
    - ``deck_speed_expert`` - ``float``
  - ``complexity`` - ``table``
    - ``track_complexity`` - ``float``
    - ``tap_complexity`` - ``float``
    - ``cross_complexity`` - ``float``
    - ``scratch_complexity`` - ``float``
- ``extra`` - ``table`` - *Required, contents not required.*
  - ``megamix`` - ``table``
    - ``playlist_track`` - ``string``
    - ``megamix_name`` - ``string``
    - ``megamix_has_intro`` - ``boolean``
    - ``megamix_highway_offset`` - ``boolean``
    - ``megamix_transitions`` - ``boolean``
  - ``id`` - ``table``
    - ``id_name`` - ``string``
    - ``id_artist`` - ``string``
    - ``id_name2`` - ``string``
    - ``id_artist2`` - ``string``
  - ``env_start_time`` - ``float``
  - ``battle_music`` - ``boolean``
  - ``guitar_mix`` - ``boolean``
  - ``menu_music`` - ``boolean``
  - ``additional_xml`` - ``string``
  - ``sort_artists`` - ``array`` - *This array should only contain strings.*
