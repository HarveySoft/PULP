# PULP
PHP Universal Loading Program
The program provide a simple interface to update MySQL/MariaDB tebles feeding a plain text.
each row in the text must begin witht a 2part token
each row is trimmed before being parses
epmty rows are ignored
each row with an invalid token will be discarded and reported as error

The following directives may (optionally) applied:
SESS.HALT 500 will instruct PULP to terminate the processing after having encountered 500 errors. By default, PULP stops after the first error detected.
SESS.LOGF logfilename will instruct pulp to write the log on filename. By default, logfilename is created using the inputfilename with the extesion .log instead of .inp 
