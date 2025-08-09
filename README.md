# cowsay-fortune

This project contains two simple scripts that I use to display a weather report, date, time, and a fortune plus some ascii art using the cowsay command.

![example image](./images/default_output.png)

## Dependencies

Ensure you have the `fortune`, `cowsay`, and the `figlet` command installed along with figlet's `contessa` font. You will also need to install cowsay-files next to these scripts.

Currently there is no configuration file/system for these scripts. They are mainly for my personal use and for anyone that wants to install and modify them. You might need to slightly adjust or tweak certain things like the column variables in `./now` for different horizontal spacing, or if you are using MacOS you might need to use `gshuf` instead of `shuf` in the `./cowsay-fortune script`. When in doubt, run one of the scripts and look for a dependency needed, or tweak as liked. 

## Potential Improvements/Future Considerations

Here are a couple of small tweaks that could improve this repository:

- Script Structure
  - It would be better if the cowsay-files script was simplified for debugging, and maybe most of the logic could be migrated to another file for better isolation
- Configuration
  - For displaying the weather, I use curl to make a request to `wttr.in`. By default I am requesting a weather report for LA, USA. It would be best if this could be overidden with a config of some sort.
