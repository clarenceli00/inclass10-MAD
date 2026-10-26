# inclass10

Why must the app keep form validation local even when it can ask an AI for a tip? Give one example of a bad decision if AI were allowed to approve signup.
The app should keep form validation local because there's no telling where your information will be sent if AI were to approve signup. It is also a massive security risk for both the company and the user data since you don't know where the AI is sending your login information and nor does the company. If AI were to approve signup, it could also hallucinate and make some sort of mistake that could end in catastrophic failure.


Which local test case changed what you implemented? Describe what you observed.
I implemented the password strength indicator. Any password without symbols and less than 11 length is returned as "weak". This is the case even when the user is not typing or has not input a password. I then tested the tips button which put out tips at random, but I wanted it to be deterministic instead of random, so I made it cycle by adding an incrementing index that would loop to the beginning of the list when pressed enough times.

https://github.com/clarenceli00/inclass10-MAD