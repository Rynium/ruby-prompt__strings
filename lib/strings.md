---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a group of characters that are "strung" together. 


# What are some examples of information that would be Strings as opposed to some other data type?

Names, numbers(numerical or names), sentences, or even entire paragraphs could be contained in a string. Any time the 'puts' method or 'gets' methods are used, they are collecting strings from the user as input, or they are used to put strings out.


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

If we wanted to extract a single character from a string, we could set the string equal to a variable, and then use the variable and the index, of the character we wanted to retrieve. For example if our string was      class_name = "Fenrir"      and we wanted to retrive the letter 'n' from the name we could do it by typying the vaiable name and index. In this case    "class_name[2]"   would return the string "n". If we tried to retreive a character that didn't exist or was at an index that was too large for our number, say    class_name[7]    then we would just retrun a nil value. When describing characters, our convential location references start at 1 (the '1st letter). When referring to indecies, our reference starts at the number 0. So to reference the last letter of a string with a length of 4, we would reference an index of 3 (string[3])


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

If we use the name and reference an index with a negative value, we will return letters at an index counting backwords from the end of the word. For example    class_name[-1]     would return 'r'. Our index value inserted could only go do to the negative length of our string. After this point it would return 'nil'.


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

If we want to replace a certain cahracter in a string, we can use the .gsub() method to accomplish this. The g in gsub is referencinng the fact that this will change the string variable on the global level and that all uses of this variable after this point will contain the sting with the substituted units. For example if we wanted to replace the "r" values in    class_name = Fenrir   with '9' we could use class_name.gsub('r', '9') and as a result our string value will now be "Fen9i9" anytime class_name is called. 
