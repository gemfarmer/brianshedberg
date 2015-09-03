---
layout: page
permalink: /new/
---
#In Python, Not in JS

Compare this code carefully to the two previous examples. When we say “with X as Y” we are defining the variable Y to be the result of running X. This begins a block of code where we can use our new variable as usual (in this case, my_input_file). The added benefit with using the with keyword is that we no longer have to worry about closing the file; once our “with block” is finished, the clean-up work (closing of the file) will be managed for us automatically.

for example:
{% highlight python %}# open types 'a' (append), 'w' (write), 'r' (read)

write_file = open("raw.text", 'a')

write_file.writelines("> \n")
# if you have opened, make sure to close
write_file.close()

# creates list of lines from that file
read_file = open("raw.text", 'r')

print read_file.readlines()
# if you have opened, make sure to close
read_file.close()


with open("raw.text", "r") as my_input_file:
    for line in my_input_file.readlines():
        print line
{% endhighlight %}