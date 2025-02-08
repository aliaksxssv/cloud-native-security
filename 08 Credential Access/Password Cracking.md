### Crack hashes
``` bash
git clone https://github.com/openwall/john -b bleeding-jumbo john
cd john/src/
./configure
make -s clean && make -sj4
``` bash
Then navigate to the run directory ( cd ../run/ ) and run the command below.
``` bash
./john ../../user_hash.list --format=Raw-SHA256 --wordlist=rockyou.txt --fork=4
``` bash