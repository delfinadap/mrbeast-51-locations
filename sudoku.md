Seems like \*a new session always goes to 271829.pdf now, with pdfIndex of 271828 (Euler's number). It's always at https://qvrvlqffqftxlxflcmzc.supabase.co/storage/v1/object/sign/hopscotch-files/271829.pdf, but you can't directly open it because you need a key.

pdfIndex is an index returned from the server when requesting a new puzzle.

The mechanism seems to be:
- New users have joined onemil.xyz, and each user got assigned a new "fingerprint" (based on their browser), which was mapped to a PDF file
- After a certain number of users (hundreds of thousands?) were assigned fingerprints -> PDF files, the server decided to only assign 271829.pdf for all new unique fingerprints but no other puzzle anymore
- ^This may be why they said "you need a million friends" - because they needed hundreds of thousands of unique fingerprints to get to the state where they only serve 271829.pdf 
- (Technical details) there have been claims that these PDF numbers were sequentially incremented. It seems like it started around 100,000, meaning it took roughly 200,000 unique visitors to reach 271,829. This may have been their way of slowing down our progress.

What we can deduct from this: 
- 271829.pdf is the one we should be looking at the most, most likely.
- It corresponds to the pdfIndex of 271828, which is roughly Euler's number * 10^5

\*A new session with a unique browser fingerprint
