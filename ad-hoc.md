# Copy ssh key
`ansible debian1 -m authorized_key -a "user='root' state='present' key='{{ lookup('file','/Users/din/.ssh/id_rsa.pub')}}'" -b -k -K`
