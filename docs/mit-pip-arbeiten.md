# Mit pip arbeiten

Mit der Installation von Python wird auch der Paketmanager `pip` installiert. Mit `pip` können alle Python-Pakete, welche auf [PyPI](https://pypi.org/) veröffentlicht werden, installiert werden.


## Globale Installationen

Die globale Installation installiert ein Python-Paket systemweit. Das Paket findet sich nach der Installation im Unterordner `Libs/site-packages` des `Python Home Verzeichnises`.

Mit der Python Installation wurden zwei Verzeichnisse in der Umgebungsvariable `PATH` angelegt. Ein Pfad führt zum `Python Home Verzeichnis` und ein Pfad führt zum `Python Scripts Verzeichnis`. Wenn mit `pip` ein Paket installiert wird, welches ein Kommandozeilen Programm mitführt, wird dieses im `Python Scripts Verzeichnis` abgelegt. Da sich das `Python Scripts Verzeichnis` in der `PATH` Variable befindet, sind alle dort installierten Programme auch direkt über die Shell ausführbar.

---

_**Wichtig:** Global kann nur eine spezifische Version eines Python-Pakets installiert werden. Wenn 2 Anwendungen unterschiedliche Versionen des Pakets benötigen würden, kommt es zu einem Konflikt._



## Beispiel: Installation Jupyter Notebook

Es kann die Windows Powershell geöffnet werden und der Installationbefehl `pip install jupyter` ausgeführt werden. `jupyter` ist der Paketname der Software `Jupyter Notebooks` (siehe [PyPI](https://pypi.org/)).

Das `jupyter` Paket führt ein Kommandozeilenprogramm mit, welche im `Python Scripts Verzeichnis` abgelegt wurde. Da sich dieses Verzeichnis in der `PATH` Variable befindet, ist nun der Befehl `jupyter` über die Shell (zB Powershell) verfügbar.

Mit dem Befehl `jupyter notebook` kann nun die Software `Jupyter Notebooks` gestartet werden. Das Verzeichnis in dem der Befehl `jupyter notebook` ausgeführt wurde, fungiert dann als das Hauptverzeichnis der `Jupyter Notebooks` Anwendung.

## Beispiele: Wichtige pip Befehle

#### Numpy installieren

```
pip install numpy
```

#### Numpy installieren (Version 1.15.4)

```
pip install numpy==1.15.4
```

#### Alle installierten Pakete auflisten

```
pip list
```

#### Numpy deinstallieren

```
pip unistall numpy
```

#### Installierte Pakete in requirements.txt schreiben

```
pip freeze > requirements.txt
```
