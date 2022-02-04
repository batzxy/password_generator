# rust_password_generator
Simple password generator in Rust.
Since this project is shifted from Python3, I have posted the Python3 version of the code for future purposes.
```
#!/usr/bin/env python3
import random, string, argparse
parser = argparse.ArgumentParser()
parser.add_argument("passwordLength", type=int,
                    help="How much character long?")
args = parser.parse_args()
print (''.join(random.choice(string.ascii_letters + string.digits + string.punctuation) for i in range(args.passwordLength)))
```
Note: Yeah I did not used argument helpers in this project.
