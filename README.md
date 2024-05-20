Replace substring in a string
In this article we are going to make a java program to replace substring in a string . we will be asking the user to input a base string, than we will ask for a substring which is to replaced, and finally we will ask for the string which is to be placed on the place of substring and by using replaceAll() we will replace old string with new one.

Java Program to Replace Substring in a String
Algorithm: Replace Substring in a String
Start with the original string, the substring to replace, and the replacement string.
Define a method replaceSubstring that takes these three inputs:

original (original string)
toReplace (substring to be replaced)
replacement (string to replace the substring with)
Inside the replaceSubstring method:

Check if the original string contains the toReplace substring using the contains method.

If the toReplace substring is not found in the original string, return the original string as it is.

If the toReplace substring is found: 

Use the replaceAll method to replace all occurrences of the toReplace substring with the replacement string. 

Store the modified string in a variable (modified). d. Return the modified string.

In the main method:

Initialize the original String with the input string.

Initialize the substring ToReplace with the substring you want to replace.

Initialize the replacement with the string you want to replace the substring with.

Call the replace Substring method with original String, substring To Replace, and replacement as arguments to perform the replacement.

Print the original string and the modified string to the console.

End the program.

Java (Replace Substring in a String Java)
Run
public class Main {
    public static void main(String[] args) {
        String originalString = "Hello, World!";
        String substringToReplace = "World";
        String replacement = "Java";

        // Replace the substring
        String modifiedString = replaceSubstring(originalString, substringToReplace, replacement);

        // Print the modified string
        System.out.println("Original String: " + originalString);
        System.out.println("Modified String: " + modifiedString);
    }

    public static String replaceSubstring(String original, String toReplace, String replacement) {
        // Check if the original string contains the substring to replace
        if (!original.contains(toReplace)) {
            return original; // If not, return the original string as it is
        }

        // Use the replaceAll method to replace all occurrences of the substring
        String modified = original.replaceAll(toReplace, replacement);
return modified;
}
}
Output
Original String: Hello, World!
Modified String: Hello, Java!
