# gnome-shell-extensions-notes
random findings about extensions create and debugging


## lg
get access to your extension settings with convenience

    settings=imports.misc.extensionUtils.extensions[Object.keys(imports.misc.extensionUtils.extensions).filter(e=>e.match('^run-or-raise'))[0]].imports.convenience.getSettings()
    settings.list_keys()
    settings.get_value('switch-back-when-focused').get_boolean()
    settings.get_boolean('switch-back-when-focused') // same
    settings.set_boolean('switch-back-when-focused') // same
    
    
