
windows
FOR /L %i IN (0,1,3) DO (timeout 600 & git add . & git commit -m "10min autosave wip" & git push -u origin main)


bash
for i in {1..5}; git add . ; git commit -m "10min autosave wip" : git push -u origin main; done
