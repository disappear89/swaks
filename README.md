# How to run
## No auth
docker run --rm disappear/swaks -f from@mail.dev -t to@mail.dev -s hostname -p 25
## NTLM Auth
docker run --rm disappear/swaks -f from@mail.dev -t to@mail.dev -s hostname -p 25 --auth NTLM --auth-user test-user --auth-password 1234
## NTLM Auth + TLS
docker run --rm disappear/swaks -f from@mail.dev -t to@mail.dev -s hostname -p 25 --auth NTLM --auth-user test-user --auth-password 1234 --tls
