## Feedback 

Nice work on this project, you can consider it complete. I'm going to read your files in order and give you feedback
as I move through them, from Task 1 to Task 3. 

It's a little odd to do what's really your "readme" as a notebook. Typically these are .md files. You wrote 

> I think it would be valuable to emphasize the importance of troubleshooting the data with a smaller set of the transactions

Yeah, in the future perhaps I will hit this harder. I provided those small transactions files (just the first 10K rows) and encouraged people
do get all their code working on those, but I didn't really push anyone to use it. 


### Task 1

I'm surprised that this line worked for you: 

```
if not first_line.startswith('"datetime"') and not first_line.startswith('datetime'):
    content = ','.join(headers) + '\n' + content
```
You're working with files that have a two different delimiters and some have quotes. Maybe 
all of the files that are missing headers are commas, but you're really depending on some happenstance to keep this working. 

The rest of this looks good, though I'm slightly surprised everything worked since tehre are some places where your code seems a little fragile. But you got it done!

### Task 2

* Nice job on this task. 
* It'd be worth thinking through how you'd do this the reproducible way. That'd involve selecting distinct card numbers, pulling them down to python, calling `random.sample` and then building a query that could use them all. Let me know if it's not clear how you'd do that. 


### Task 3

* Nice job on this, very efficient.
* This notebook has a runtime error in it. For assignments, just run everything through so I
can see that it worked. Outside of classes, just clear all output and the do the save and commit. 


