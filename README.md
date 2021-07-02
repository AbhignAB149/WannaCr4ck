# WannaCr4ck
Includes a write-up with solutions and tool codes used

# Write-up
Let us start from last tasks  (P.S: My mothertoungue is not URDU,xD)

[Task-3 : *Flag in Funny audio*] (To be frank,its not that funny,xD)

I will share my whole thought process from my initial wrong appraoch to final correct approach.
<br>
Secret data hidden in an audio file(funny audio file).<br>
As soon as I read the problem statement (just listening for first 7secs of audio)I instinctly decided to decode the audio mp3 file into binary data.I converted the audio file into ASCII format and put it in my notepad.Then I was pondering on where do I search for the secret in this whole bunch of random text!?<br>
So,I decided to scale down my approach and listened to the audio :) in a common man approach.Then I realised I took a whole long (wrong too) journey to reach the same point.The logic is in the audio clip.It has only 2 phrases being repeated over and over consecutively in some manner which is nothing but a sequence with one phrase as '1' and other phrase as '0' (actually choice of 1 to particular phrase is specific inorder to meet the range of ASCII values which is required to crack the secret).<br>So I manually recorded the sequence in a binary fashion by listening to the audio clip.
![Screenshot (244)](https://user-images.githubusercontent.com/54037421/124306892-a4ae8980-db84-11eb-81d9-5f227137ca9a.png)
<br>
I used an <a href="https://www.binaryhexconverter.com/binary-to-ascii-text-converter">online</a> binary to ASCII character converter to decipher the hidden flag.
<br>
![Screenshot (245)](https://user-images.githubusercontent.com/54037421/124307664-c52b1380-db85-11eb-978b-4ae1d63d5c77.png)

[Finally the Secret is] : *Audio is Nice*
Now I understood why it is called funny audio , had fun doing this task!

[Task-2 : *Flag in Code*]

This task demanded me to have an instant short blind date with Julia.I referred to Julia language documentation inorder to understand given code.Came to important conclusions regarding these lines:
![Screenshot (247)](https://user-images.githubusercontent.com/54037421/124308335-ca3c9280-db86-11eb-979a-5b67238fbd7a.png)

Those lines indicate that y is complement of x and x,y together form complete set s.And those x,y are converted as INT and FLOAT for compatibility of function f.

We can decode the flag which is the input by understand the set of output values which are odd when entry is FLOAT and which are even when entry is INT.So I wrote a <a href="https://github.com/AbhignAB149/WannaCr4ck/blob/main/helper_Code"> helper code <a> (uploaded in repo too!) to automate the deciphering process.
  
 ![Screenshot (249)](https://user-images.githubusercontent.com/54037421/124309532-7af76180-db88-11eb-829e-0a2730e07416.png)

  
What we obtained are sequence of ASCII values(Uint8) which needs to be converted into characters to decipher the string.
  
  ![Screenshot (250)](https://user-images.githubusercontent.com/54037421/124309299-2522b980-db88-11eb-8878-a8587d339e9b.png)

 [Julia's Secret is] : *multiple dispatch is awesome* (Seems like she enjoyed the date :) )
  
[Task-1 : *Free Flag Yay!*]
  
  Reporting Flags:
  
  ![Screenshot (255)](https://user-images.githubusercontent.com/54037421/124311800-ec84df00-db8b-11eb-9459-6a7203394744.png)

  
 

 

 
