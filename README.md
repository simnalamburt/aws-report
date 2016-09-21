AWS Report Downloader
========

```bash
# Requires nodejs ≥6.0.0
npm install

# Fill in your AWS account info
cp secret.toml secret.toml.example
vim secret.json

./run
```

#### Running headlessly on ubuntu
```bash
# Install dependencies
sudo apt-get install -y \
    libgtk2.0-0 libgconf-2-4 \
    libasound2 libxtst6 libxss1 libnss3 xvfb

# Start Xvfb
Xvfb -ac -screen scrn 1280x2000x24 :9.0

# Run headlessly
DISPLAY=:9.0 ./run > out.csv
```

--------

[MIT License](LICENSE.md)
