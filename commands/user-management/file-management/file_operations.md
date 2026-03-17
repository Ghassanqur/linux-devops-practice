# File Management in Linux

## Create Files & Directories
touch file.txt
mkdir new_folder
mkdir -p dir1/dir2

## Copy Files
cp file.txt copy.txt
cp -r folder1 folder2

## Move / Rename Files
mv file.txt newfile.txt
mv file.txt /home/user/

## Delete Files
rm file.txt
rm -r folder

## View Files
cat file.txt
less file.txt
head file.txt
tail file.txt

## File Permissions
chmod 755 file.sh
chmod +x script.sh

## Ownership
chown user:user file.txt
