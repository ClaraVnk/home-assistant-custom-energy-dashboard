This is based on @zatoufly 's work (available on Github https://github.com/zatoufly)

How customize the colors of your energy dashboard on Home Assistant ?

Here we are based on a french electricity contract named "Tempo", which allow 3 colors and 6 options (high or low price for each color).

1) Create a "themes" folder

In your File Editor, add a new folder named "themes" in your home assistant.
   
2) Create a "theme_tempo.yaml" file

In your new "Themes" folder, add a new file named "theme_tempo.yaml".

3) Edit your configuration.yaml

In this file, in order to see the changes, you should write :
```
# Load frontend themes from the themes folder
frontend:
  themes: !include_dir_merge_named themes
```

4) Check the configuration :

On the Developpment tools, check your configuration. If everything is okay, juste restart your Home Assistant.

5) Apply the theme :

Select your profile, then you can choose your theme and if you prefer dark or light mode.
