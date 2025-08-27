# DELACRUZ_2ECE-B_ECE2112

1. ALPHABET SOUP PROBLEM
For this one, the goal is just to rearrange the letters of a word so they come out in alphabetical order. First, we make a function that
takes in a word. Then we use the sorted() function, which automatically puts the letters in order. Since sorted() gives back a list, we use
"".join() to stick the letters back together into a word. After that, we just print it out to see the result.

def alphabet_soup(word):                 # make a function that takes in a word
return "".join(sorted(word))             # sort the letters then join them back together

print(alphabet_soup("hello"))            # try it out
print(alphabet_soup("hacker"))


2. EMOTICON PROBLEM
This one is about replacing certain words with emoticons. We make a function called emotify, and inside it, we use .replace() to swap
words with their matching emojis. For example, "smile" becomes :), "grin" becomes :D, "sad" turns into :(, and "mad" becomes >:(.
So whenever those words show up in a sentence, they get changed into the emoji version.

def emotify(text):                        # make the function
text = text.replace("smile", ":)")        # swap words for emojis
text = text.replace("grin", ":D")
text = text.replace("sad", ":(")
text = text.replace("mad", ">:(")
return text

print(emotify("Make me smile"))           # test it out
print(emotify("I am mad"))
print(emotify("What a grin"))
print(emotify("I am so sad"))


3. UNPACKING LIST PROBLEM
For this problem, we start with a list of numbers [1, 2, 3, 4, 5, 6]. We then split it into three parts: the first part only takes the
very first number in the list, the middle part takes everything between the first and the last, and the last part just takes the final
number in the list. We do this by using indexing—[0] gets the first number, [1:-1] slices out everything in the middle, and [-1] always
points to the last element. After setting them up, we print each one to see the results.

lst = [1, 2, 3, 4, 5, 6]                # create a list
first = [lst[0]]                        # grab the first number
middle = lst[1:-1]                      # grab everything except first and last
last = [lst[-1]]                        # grab the last number

print("first:", first)                  # show first
print("middle:", middle)                # show middle
print("last:", last)                    # show last
