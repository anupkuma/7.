7.
==

10)  Assume you have a method isSubstring which checks if one word is a substring of another.Given two strings, s1 and s2, write code to check if s2 is a rotation of s1 using only one call to isSubstring (i.e., “waterbottle” is a rotation of “erbottlewat”).


Here we have  created a temporary string to store concatenation of str1 to str1. Then checking if String s2 is present in tmp. If present then s2 is rotation of s1, else not.

class CheckStringRotation {

  public static void main(String[] args) {
		String s1 = "company";
		String s2 = "parade";

		String tmp = s1.concat(s1);
		System.out.println(tmp);

		if (tmp.contains(s2)) {
			System.out.println("Contains");
			System.exit(1);
		}

		System.out.println("does not contains");
	}

}
