# Context

See @PLAN.md for context.

# Find a task to complete

Look under the ./swarm/todo/ folder for a file suffixed with ".pending.md" - and claim it as a task by renaming it to ".{SWARM_TASK_ID}.processing.md".
Make sure the file you choose doesn't have any dependencies that are not completed.
Make sure your work won't conflict with other work that is already in progress.
If no tasks are found - skip the "Execute the task" step and go to the "If nothing to do" step.

# Implement the task

Then read the file and execute the task to completion, adding tests and testing when you think you need to.
When done, rename the file to ".completed.md" and add a note about what you did to the task.

If you can't complete the task, rename the file to ".pending.md" and add a note about what went wrong to the file.
When you're done, `git add .`, `git commit -m "a suitable message"`, and `git push` your changes to the remote repository.

# Post-task

After the task is complete, update the @ANALYSIS.md file which is a summary of the main points derived from your analysis. You don't necessarily have to update it, it should always contain the best summary possible of the stock.

Push everything to git after each iteration.

# If nothing to do

If there are no pending tasks found, look at what needs to be done next and plan a task and write it to ./swarm/todo/{task-name}.pending.md
Use a sequential number in the name so that it's clear which tasks come first. Once finished planning the task - exit immediately!