# Find-the-Private-Key-within-the-specific-key-range-by-the-target-Hash160
This is intended only for the BTC-Puzzle. Do not use this for any other things.

**USAGE:**

Before you run the Python file, make sure to edit the start and end range of the private key you are trying to search.

Example:
start = int("40000000000000000", 16)
end = int("7ffffffffffffffff", 16)

Then input the target Hash160:
target_hash = "739437bb3dd6d1983e66629c5f08c70e52769371"  # Replace this with your actual target hash



**Run the script:**
python privkey.py



**Explanation:**
Range: Iterates from start range to end range (hex range).

SHA-256: Hashes each private key in hexadecimal format.

RIPEMD-160: Applies the RIPEMD-160 hashing on top of SHA-256 to get the Hash160.

Matching: Compares the result with the provided target_hash.



**Execution:**

Run this script. It will begin iterating through your range and computing Hash160 for each private key.

If it finds a match, it will print the corresponding private key.
