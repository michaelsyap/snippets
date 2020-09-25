<!-- From remote to local -->
scp -P PORT_NUMBER SSH_USER@HOST:/directory_here/file_here ./download_destination


<!-- From local to remote -->
scp -P PORT_NUMBER local_file_here SSH_USER@HOST:/remote_directory_here