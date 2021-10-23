# LogsParser
Common log parser and analyzer

## Project structure

***
```
\docs - contains docs files (uml and etc)
    UML.pdf
\gui - page for working with User interface
    __init__.py
    design.py - autogenerated py file from main.ui with using pyuic
    main_app.py - contains class MainApp for working UI
    main.ui - PyQt5 file (user interface)
\logs_analyzer - contains files for analize logs and builds graphics
    __init__.py
    \analyzer.py - contains LogsAnalyzer class
    \plots.py - contains classes of different types of graphs
\mongodb - package for working with mongodb
    __init__.py
    config.py - contains DevelopingConfig class
    models.py - contains classes:GoodLog, BadLog, ReportLogs, LogFile
\parser_logs - package for working with parser class
    __init__.py
    filter.py - contains differents classes filter for logs
    log_structure.py - LogStruct class
    logs_reader.py - function for reading logs
    logs_writer.py - different functions for writining to txt, csv, ...
    parser.py - file contains class for parsing logs
.gitignore
docker-compose.yml
main_analyzer.py - entry point for logs analyzing (console interface)
main_client.py - entry point for logs parsing and analyzing (console interface)
main_parser.py - entry point for log parsing (console interface)
poetry.lock
pyproject.toml
split_logs.py - script for splitting a large file into small ones
```
***
## Arhitecture contex diagram

![image](https://user-images.githubusercontent.com/25473820/138543868-2eca1741-7ae4-47ba-bd86-05437461cb20.png)

## Arhitecture contex diagram subsystem analyzing logs

![image](https://user-images.githubusercontent.com/25473820/138544040-7a3b44d3-ab84-49d1-a2ca-c6c97add5184.png)

## Arhitecture contex diagram subsystem parsing logs

![image](https://user-images.githubusercontent.com/25473820/138544117-9b6c7e76-af6e-443a-a1ab-a08eec31b344.png)

## UML diagram

![image](https://user-images.githubusercontent.com/25473820/138544987-9a0e92aa-5bf8-4589-bdab-12bbd741b155.png)

