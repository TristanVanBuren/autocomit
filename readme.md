
windows
FOR /L %i IN (0,1,3) DO (timeout 600 & git add . & git commit -m "10min autosave wip" & git push -u origin main)


bash
place in a script chmod +x it and run in dir in proj folder
for run in {1..10}; do
  sleep 600
  git add .
  git commit -m "10 min autosave wip"
  git push -u origin main
done
