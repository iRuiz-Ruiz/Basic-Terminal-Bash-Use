```
(snakemake) raven@IT099295:~$ mamba create -c conda-forge -c bioconda -n snakemake snakemake

Error while loading conda entry point: anaconda-cloud-auth (cannot import name 'ChannelAuthBase' from 'conda.plugins.types' (/home/raven/anaconda3/lib/python3.11/site-packages/conda/plugins/types.py))
Error while loading conda entry point: anaconda-cloud-auth (cannot import name 'ChannelAuthBase' from 'conda.plugins.types' (/home/raven/anaconda3/lib/python3.11/site-packages/conda/plugins/types.py))
argument COMMAND: conflicting subparser: repoquery

# >>>>>>>>>>>>>>>>>>>>>> ERROR REPORT <<<<<<<<<<<<<<<<<<<<<<

    Traceback (most recent call last):
      File "/home/raven/anaconda3/lib/python3.11/site-packages/conda/exception_handler.py", line 17, in __call__
        return func(*args, **kwargs)
               ^^^^^^^^^^^^^^^^^^^^^
      File "/home/raven/anaconda3/lib/python3.11/site-packages/mamba/mamba.py", line 945, in exception_converter
        raise e
      File "/home/raven/anaconda3/lib/python3.11/site-packages/mamba/mamba.py", line 938, in exception_converter
        exit_code = _wrapped_main(*args, **kwargs)
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
      File "/home/raven/anaconda3/lib/python3.11/site-packages/mamba/mamba.py", line 877, in _wrapped_main
        configure_parser_repoquery(p._subparsers._group_actions[0])
      File "/home/raven/anaconda3/lib/python3.11/site-packages/mamba/mamba.py", line 805, in configure_parser_repoquery
        p = sub_parsers.add_parser(
            ^^^^^^^^^^^^^^^^^^^^^^^
      File "/home/raven/anaconda3/lib/python3.11/argparse.py", line 1192, in add_parser
        raise ArgumentError(self, _('conflicting subparser: %s') % name)
    argparse.ArgumentError: argument COMMAND: conflicting subparser: repoquery

`$ /home/raven/anaconda3/condabin/mamba create -c conda-forge -c bioconda -n snakemake snakemake`

  environment variables:
                 CIO_TEST=<not set>
        CONDA_DEFAULT_ENV=snakemake
                CONDA_EXE=/home/raven/anaconda3/bin/conda
             CONDA_PREFIX=/home/raven/anaconda3/envs/snakemake
           CONDA_PREFIX_1=/home/raven/anaconda3
    CONDA_PROMPT_MODIFIER=(snakemake)
         CONDA_PYTHON_EXE=/home/raven/anaconda3/bin/python
               CONDA_ROOT=/home/raven/anaconda3
              CONDA_SHLVL=2
           CURL_CA_BUNDLE=<not set>
               LD_PRELOAD=<not set>
                     PATH=/home/raven/.local/bin:/home/raven/paml/bin:/home/raven/anaconda3/envs
                          /snakemake/bin:/home/raven/anaconda3/condabin:/usr/local/sbin:/usr/loc
                          al/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/mnt/
                          c/Program Files/WindowsApps/CanonicalGroupLimited.Ubuntu20.04LTS_2004.
                          6.16.0_x64__79rhkp1fndgsc:/mnt/c/Program Files (x86)/Common Files/Orac
                          le/Java/javapath:/mnt/c/Windows/system32:/mnt/c/Windows:/mnt/c/Windows
                          /System32/Wbem:/mnt/c/Windows/System32/WindowsPowerShell/v1.0:/mnt/c/W
                          indows/System32/OpenSSH:/mnt/c/Program Files/dotnet:/mnt/c/Program
                          Files (x86)/NVIDIA Corporation/PhysX/Common:/mnt/c/Program
                          Files/MEGA11:/mnt/c/Program Files/Git/cmd:/mnt/c/Program
                          Files/Geneious Prime:/mnt/c/texlive/2023/bin/windows:/mnt/c/Users/ek23
                          810/AppData/Local/Microsoft/WindowsApps:/mnt/c/Users/ek23810/AppData/L
                          ocal/Programs/MiKTeX/miktex/bin/x64:/mnt/c/Users/ek23810/AppData/Local
                          /GitHubDesktop/bin:/mnt/c/Users/ek23810/AppData/Local/Programs/Microso
                          ft VS Code/bin:/mnt/c/Users/ek23810/AppData/Local/Pandoc:/snap/bin
       REQUESTS_CA_BUNDLE=<not set>
            SSL_CERT_FILE=<not set>

     active environment : snakemake
    active env location : /home/raven/anaconda3/envs/snakemake
            shell level : 2
       user config file : /home/raven/.condarc
 populated config files :
          conda version : 23.7.4
    conda-build version : 24.3.0
         python version : 3.11.5.final.0
       virtual packages : __archspec=1=broadwell
                          __glibc=2.31=0
                          __linux=4.4.0=0
                          __unix=0=0
       base environment : /home/raven/anaconda3  (writable)
      conda av data dir : /home/raven/anaconda3/etc/conda
  conda av metadata url : None
           channel URLs : https://repo.anaconda.com/pkgs/main/linux-64
                          https://repo.anaconda.com/pkgs/main/noarch
                          https://repo.anaconda.com/pkgs/r/linux-64
                          https://repo.anaconda.com/pkgs/r/noarch
          package cache : /home/raven/anaconda3/pkgs
                          /home/raven/.conda/pkgs
       envs directories : /home/raven/anaconda3/envs
                          /home/raven/.conda/envs
               platform : linux-64
             user-agent : conda/23.7.4 requests/2.31.0 CPython/3.11.5 Linux/4.4.0-19041-Microsoft ubuntu/20.04.6 glibc/2.31
                UID:GID : 1000:1000
             netrc file : None
           offline mode : False


An unexpected error has occurred. Conda has prepared the above report.
If you suspect this error is being caused by a malfunctioning plugin,
consider using the --no-plugins option to turn off plugins.

Example: conda --no-plugins install <package>

Alternatively, you can set the CONDA_NO_PLUGINS environment variable on
the command line to run the command without plugins enabled.

Example: CONDA_NO_PLUGINS=true conda install <package>
```
