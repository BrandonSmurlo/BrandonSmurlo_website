---
layout: base 
title: MCQ Reflection + Sprint 3 Reflection
search_exclude: true

---

# Reflection on MCQ Mistakes

After going through this quiz, I realized there were several key areas where I struggled. I got 49/66. These mistakes have helped me identify the specific topics I need to focus on, so I can improve my understanding and do better in the future. The following is a breakdown of the questions I got wrong, in order, and what I learned from each one. Additionally, I’ll explain the areas I need to work on, based on my mistakes. What I learned from each question on the quiz is outlined below.

## 1. Prime Number Counting Error
In this question, I had to count prime numbers in a list. I made a mistake because I didn’t initialize the counter properly, which caused it to reset inside the loop. As a result, the counter was incorrect by the time the loop ended.

- **Why I Got It Wrong**: I forgot to initialize the counter outside of the loop, which reset it during each iteration.
- **Correct Answer**: **Option A: Initialize the counter outside of the loop.**
- **What I Learned**: When counting things in a loop, variables like counters should be initialized before the loop begins to ensure they keep their values.

## 2. Sorting and Finding the Smallest Number
This question asked me to find the smallest number in a list. I tried to do this without sorting the list first, which made it harder to correctly identify the smallest number.

- **Why I Got It Wrong**: I didn’t realize that sorting the list first would make finding the smallest number much easier.
- **Correct Answer**: **Option C: Sort the list in ascending order before extracting the smallest value.**
- **What I Learned**: Sorting a list is an important first step when trying to find the smallest or largest values in a collection of numbers.

## 3. String Manipulation: Incorrect Substring Indices
I made a mistake with string manipulation when I had to extract a substring. I selected the wrong indices, which caused the substring to be incorrect.

- **Why I Got It Wrong**: I didn’t pick the correct starting index and length for the substring.
- **Correct Answer**: **Option B: Use the correct indices for substring extraction.**
- **What I Learned**: I need to be more careful with indices when using substring functions. A small mistake can lead to completely wrong results.

## 4. Prime Checking Function
In this question, I misunderstood how the prime-checking function worked. I made the mistake of overcomplicating the logic when the function was simple and straightforward.

- **Why I Got It Wrong**: I didn’t trust the simplicity of the `isPrime()` function and thought there was a mistake in it.
- **Correct Answer**: **Option D: Use the `isPrime()` function directly without modification.**
- **What I Learned**: I need to trust built-in functions when they are simple and avoid trying to overcomplicate solutions.

## 5. For-Each Loop for Counting Prime Numbers
This question asked me to count prime numbers using a `for-each` loop. I mistakenly reset the counter inside the loop instead of just updating it.

- **Why I Got It Wrong**: I reset the counter in the loop, which meant I lost the count after each iteration.
- **Correct Answer**: **Option A: Update the counter without resetting it in the loop.**
- **What I Learned**: I need to update the counter inside loops but not reset it to avoid starting from zero each time.

## 6. Incorrect Indexing for List Slicing
In this question, I had to slice a list to extract specific elements, but I used the wrong indices, which led to incorrect results.

- **Why I Got It Wrong**: I confused the indices for slicing and didn’t get the right range of values.
- **Correct Answer**: **Option C: Ensure the start and end indices are correct when slicing the list.**
- **What I Learned**: It’s essential to understand zero-based indexing and to be precise with start and end indices when slicing lists.

## 7. Sorting Before Extracting Values
This question involved finding the smallest value in a list. I tried to extract it without sorting the list first, which made the task much harder.

- **Why I Got It Wrong**: I didn’t realize that sorting would make finding the smallest value easier.
- **Correct Answer**: **Option A: Sort the list before extracting the smallest value.**
- **What I Learned**: Sorting the list first is a simple and effective strategy for finding the smallest or largest values.

## 8. Multiple-Choice Answer Confusion
I made some mistakes because I misunderstood the multiple-choice options. I picked an answer that seemed correct at first but turned out to be wrong.

- **Why I Got It Wrong**: I didn’t read the options carefully enough before selecting an answer.
- **Correct Answer**: **Option D: Read all the options before selecting an answer.**
- **What I Learned**: It’s important to read all the options carefully, even if one answer seems obvious.

## 9. Negative or Zero Values in Lists
This question asked about handling lists that might contain negative or zero values. I failed to account for these possibilities when searching for the smallest value.

- **Why I Got It Wrong**: I didn’t consider that negative numbers and zero could be part of the list when searching for the smallest value.
- **Correct Answer**: **Option B: Consider all possible values, including negative and zero.**
- **What I Learned**: I need to remember that lists can contain negative numbers and zero, and I should account for them when searching for specific values.

## 10. Prime Logic Confusion
I got another question wrong because I confused the logic for counting prime numbers with removing non-primes. I didn’t follow the correct approach for counting primes.

- **Why I Got It Wrong**: I mixed up the process of counting primes with filtering out non-prime numbers.
- **Correct Answer**: **Option C: Use a separate function to count prime numbers.**
- **What I Learned**: I need to keep counting and filtering operations separate to avoid confusion.

## 11. Substring Function Mistake
Another string manipulation question caused me to select the wrong part of a string due to incorrect use of the substring function.

- **Why I Got It Wrong**: I didn’t choose the correct starting index or length when extracting a substring.
- **Correct Answer**: **Option D: Ensure correct indices when extracting substrings.**
- **What I Learned**: I need to double-check my indices and make sure I understand how string slicing works before extracting parts of strings.

## 12. Incorrect Use of List Operations
In this question, I was asked to use specific list operations, and I misunderstood how the operations affected the list. I also didn’t correctly use the method to find an element.

- **Why I Got It Wrong**: I didn’t grasp how operations like `sort()` or `reverse()` affect the order of elements in a list.
- **Correct Answer**: **Option A: Understand how list operations affect list order.**
- **What I Learned**: It’s crucial to understand how each operation works and affects the list’s structure.

## 13. Prime Numbers and Loops
This question involved iterating over a list to count prime numbers. I made the mistake of not using the loop correctly in conjunction with the `isPrime()` function.

- **Why I Got It Wrong**: I didn’t understand how to properly use the `isPrime()` function inside a loop.
- **Correct Answer**: **Option B: Correctly integrate the `isPrime()` function within the loop.**
- **What I Learned**: I need to focus on how loops and functions interact to make sure the algorithm works as intended.

## 14. List Slicing Mistake
In this question, I had to extract a part of the list using slicing. I made the mistake of selecting incorrect indices, which led to an incorrect result.

- **Why I Got It Wrong**: I used the wrong indices when trying to slice the list.
- **Correct Answer**: **Option C: Use the correct indices for list slicing.**
- **What I Learned**: I need to be careful with indexing when slicing lists and always check that the start and end points are correct.

## 15. Sorting and Extracting Values
This question tested my understanding of sorting a list before extracting a value. I didn’t realize that sorting was necessary before trying to extract the smallest number.

- **Why I Got It Wrong**: I didn’t understand that sorting the list should happen first.
- **Correct Answer**: **Option A: Sort the list before extracting the smallest value.**
- **What I Learned**: Sorting the list before extracting values makes the process simpler and more reliable.

## 16. Counter Update Mistake in Loop
In this question, I had to count prime numbers using a loop, but I mistakenly updated the counter incorrectly, which caused my count to be wrong.

- **Why I Got It Wrong**: I made an error in updating the counter during each iteration of the loop.
- **Correct Answer**: **Option D: Correctly update the counter in the loop.**
- **What I Learned**: I need to make sure I update the counter correctly, but I should not reset it in the loop.

## 17. Incorrect List Indexing
This final question involved extracting specific elements from a list. I made a mistake by selecting the wrong indices, which led to the wrong result.

- **Why I Got It Wrong**: I didn’t pay attention to the correct indices when extracting elements from the list.
- **Correct Answer**: **Option C: Select the correct indices when extracting list elements.**
- **What I Learned**: I need to be more careful with my indexing to ensure I’m working with the right elements in the list.

## Conclusion and Areas for Improvement

From this quiz, I learned that I need to improve my understanding of several key topics:

- **2.4: Using Programs with Data**: I struggled with counting, sorting, and extracting values from lists, which made me realize I need more practice with loops, list operations, and string manipulations.
- **3.3: Mathematical Expressions**: I misunderstood some operations, especially when they involved prime numbers and sorting, showing I need to work on how I handle mathematical expressions programmatically.
- **3.5: Boolean Expressions**: I had difficulty with logic-based questions, like checking whether numbers were prime, indicating I need more practice with boolean expressions.
- **3.10: Lists**: I made several mistakes with list slicing and operations like sorting. I need to focus on how to properly manipulate lists.
- **4.2: Fault Tolerance**: I wasn’t careful with potential errors, like miscounting values or picking wrong indices, showing that I need to work on handling errors more effectively in my programs.



# **Sprint 3 Reflection:**

| **Soft Skills**                  | **Points**    | **Grade** | **Evidence** |
|----------------------------|---------------|-----------|--------------|
| Work Habits (Analytics)    | 1             |   0.9        |     Took initiative in frontend development and collaborated with peers to troubleshoot issues.        |
| Evidence of Role in Team   | 1             |     0.9      | Led the frontend design and worked closely with our scrum master to track project progress.           |
| Function / Purpose Design  | 1             |     0.9      |  Ensured frontend functionality aligned with project objectives and user experience.            |
| Live Review                | 2             |      0.9     | Introduced the website during the live review and effectively communicated design and progress.       |
| **Total**                  | 5             |     3.6/4      |              |


# Greatest Coding Accomplishment (Music Page):

**Custom User Playlists Code Snippet**

let playlist = [];

function addSong() {
    const song = document.getElementById('songInput').value;
    if (song) {
        playlist.push(song);
        updatePlaylist();
        document.getElementById('songInput').value = ''; // Clear input
    }
}

function updatePlaylist() {
    const playlistDiv = document.getElementById('playlist');
    playlistDiv.innerHTML = '';
    playlist.forEach((song, index) => {
        const songDiv = document.createElement('div');
        songDiv.classList.add('song');
        songDiv.textContent = `${index + 1}. ${song}`;
        playlistDiv.appendChild(songDiv);
    });
}

**What it Does:**

- Adds songs to a playlist dynamically.
- Updates the list in real-time without reloading the page.

**Why it is an Accomplishment:**

- It is simple but interactive, and users can create and update playlists on the fly.
- Easy to expand with features like saving playlists or removing songs.

**Reflection**

The code for the user-curated playlist page was very significant to me in the sense that it was a challenge. It was a challenge to alter the code such that it would save after use, so that it could be accessed at a later time and previous playlists could be viewed, edited, and deleted. I had to consult several others in the classroom in order to collaborate and figure out how to make a "live" page where a user can see playlists that have been created.