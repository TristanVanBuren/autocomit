<pre>
windows
paste into vscode command line that is in project directory

FOR /L %i IN (0,1,3) DO (timeout 600 & git add . & git commit -m "10min autosave wip" & git push -u origin main)

</pre>
<pre>
bash
place in a script chmod +x it and run in the folder comtaining the project 
this will also run in a vs terminal just tested


for run in {1..10}; do
  sleep 600
  git add .
  git commit -m "10 min autosave wip"
  git push -u origin main
done

  
</pre>

please add an issue in the issue tab or email me at vanburent10@mycu.concord.edu if it isn't working
