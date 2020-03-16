# Custom-Linux-Shell
A custom linux shell built in Ubuntu

Prerequisite packages:

For Ubuntu:
  - sudo apt install sox
  - sudo apt install crontab
  - sudo apt install graphviz
  - sudo apt install dot
  - sudo apt install python3
  - sudo apt install python3-pip
 
Newly introduced commands:
  - myfg <PID> : brings a paused job to the foreground
  - mybg <PID> : brings a paused job to the background
  - pause <PID> : pauses a job (State T)
  - myjobs: lists all jobs of the current user
  - alarm <hh.mm> <audio file> : sets a daily cronjob alarm to play the specified audio.
  - psvis <PID> <output file> : generates a .png image that shows a process tree with the given PID and its children. Also,
                                execution time processes are included in the output image.
  - google: enables to search a query on google and returns first 5 results as website link.
  - sendmail: enables to send an email, however user should give permission on the mail service, e.g. Gmail or Outlook.
  
  Supported utilities:
    - Auto complete with tab key.
    - Background job with & symbol
    - I/O redirection with <, > and >> symbols.
      - < as stdin, > as stdout but truncate the file, >> as stdout but append the file. Stderr redirection is not supported.
    - Pipe commands with | symbol.
   
   
Other prerequisites:
  - psvis command requires a call to "make" to generate kernel object files, e.g. .ko files.
  
