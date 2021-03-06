#cool-old-term

##Description
cool-old-term is a terminal emulator which tries to mimic the look and feel of the old cathode tube screens.
It has been designed to be eye-candy, customizable, and reasonably lightweight.

It now uses the konsole engine which is powerful and mature.

This terminal emulator requires Qt 5.2 or higher to run.

##Screenshots
![Image](<http://i.imgur.com/NUfvnlu.png>)
![Image](<http://i.imgur.com/4LpfLF8.png>)
![Image](<http://i.imgur.com/MMmM6Ht.png>)

##Build instruction
First of all we need to retrieve the dependencies.

###Ubuntu 14.04
    sudo apt-get install build-essential qmlscene qt5-qmake qt5-default qtdeclarative5-dev qtdeclarative5-controls-plugin qtdeclarative5-qtquick2-plugin libqt5qml-graphicaleffects qtdeclarative5-dialogs-plugin qtdeclarative5-localstorage-plugin qtdeclarative5-window-plugin

###Arch Linux
    sudo pacman -S qt5-base qt5-declarative qt5-quickcontrols qt5-graphicaleffects

###Anyone else
Install Qt directly from here http://qt-project.org/downloads . Once done export them in you path (replace "_/opt/Qt5.3.1/5.3/gcc_64/bin_" with your correct folder):
    
    export PATH=/opt/Qt5.3.1/5.3/gcc_64/bin/:$PATH

###Compile
Once Qt are installed and in your path you need to compile and run the application: 

	git clone https://github.com/Swordifish90/cool-old-term.git
    cd cool-old-term
    cd konsole-qml-plugin
    qmake && make && make install
    cd ..
	./cool-old-term

