# Navigation commands
pwd - prints working directory 
ls - Lists the contents of the current directory
cd - change into a directory - cd.. moves up one level - cd~ takes you to home directory
file - tells tells you what type of thing (file. content, directory) something is

# File operations commands
touch test.txt
mkdir -p projects/demo
cp test.txt projects/demo/
mv projects/demo/test.txt projects/demo/backup.txt
rm projects/demo/backup.txt

# Viewing files
cat /etc/passwd
less /var/log/syslog
head -n 20 /etc/services
tail -f /var/log/auth.log
strings <file> extracts readable text from a binary file — the go-to when a password is buried inside something that isn't plain text.
