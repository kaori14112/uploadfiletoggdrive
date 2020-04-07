# uploadfiletoggdrive
python script to upload file into google drive
Sources: https://gist.github.com/jmlrt/f524e1a45205a0b9f169eb713a223330
This version has been modified to work normally on my computer.
##How to use:
python3 gdrive_upload_folder.py -s source_folder -d destination_folder_in_google_drive -p parent_directory
(script will automatically create destination folder if it not yet created)
Notice problem happen with httplib2 and google-api-python-client, if you got error "httplib2.RedirectMissingLocation: Redirected but the response is missing a Location: header."
Just remove httplib2 and reinstall with older version:
check version: pip3 freeze
remove current httplib2: pip3 uninstall httplib2
reinstall with working version: pip3 install httplib2==0.15.0
More bugs please respond, thank you.
