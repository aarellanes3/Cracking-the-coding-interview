# Cracking-the-coding-interview
IsUnique
	Identify the problem- Does a string have all different letters 
	Define the goals – The solution should be simple you check one character with all the other characters in the string
	Explore-
1.	Work small examples by hand-aba returns false, abc returns true, “” return false, f returns true 
2.	Write down what you did in words (algorithm)-
i.	Take a string
ii.	Check the length of a string 
iii.	Compare each letter to the rest
iv.	If the letter is the same it is false
v.	Otherwise keep comparing to you finish the String
vi.	Return true
3.	Find patterns- characters should not be repeated in the string
4.	Work another example by hand (does your algorithm work) grape returns true
5.	Translate to code-
public static boolean isUnique(String str){
		for(int i =0; i<str.length(); i++){
			for(int j = i+1; j<str.length(); j++){
				if(str.charAt(i) == str.charAt(j)){
					return false;
				}
			}
		}
		return true;
6.	Test several cases-trap returns true asdfghijklmn returns true, reep returns false, 
7.	Debug failed test cases- Need to take the numbers into consideration as well
