Limpiar la caché del sistema

Libera espacio y mejora la velocidad del sistema:sudo rm -rf ~/Library/Caches/*
sudo rm -rf /Library/Caches/*
rm -rf ~/Library/Safari/*
iberar memoria RAM

Reduce la dependencia del disco y mejora la fluidez:sudo purge
 Optimizar Finder

Haz que Finder cargue más rápido:
defaults write com.apple.finder FXPreferredViewStyle -string "Nlsv"
defaults write com.apple.finder QLInlinePreview -bool false
killall Finder
Desactivar animaciones innecesarias

Reduce el uso de recursos visuales:defaults write com.apple.dock reduce-motion -bool true; killall Dock
defaults write NSGlobalDomain NSAutomaticWindowAnimationsEnabled -bool false
defaults write com.apple.dock expose-animation-duration -float 0.1; killall Dock
 Eliminar elementos de inicio de sesión

Evita que apps innecesarias se ejecuten al iniciar:
osascript -e 'tell application "System Events" to get the name of every login item'
osascript -e 'tell application "System Events" to delete login item "NombreApp"'
Mantener el Mac despierto

Evita que entre en reposo mientras trabajas:

caffeinate






















