When we want to use packages from our private git projects, we might get an error that our code cant see or use a package from another private git project.  
We could solve this by below aproach:  
```bash
# our gitlab private token
git config --global http.extraheader "PRIVATE-TOKEN: YOUR_PRIVATE_TOKEN"

# configuring git to athenticate with ssh key instead of http
git config --global url."git@gitlab.mycompany.com:".insteadOf "https://gitlab.mycompany.com/"
```
