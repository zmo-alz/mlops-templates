ssh-keygen -t ed25519 -C "zach.olinske@gmail.com"

eval "$(ssh-agent -s)" 
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub

bash mlops-v2/sparse_checkout.sh