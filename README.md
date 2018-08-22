# Tinycoin

This project is created to learn blockchain by creating a small blockchain and it's own coin. 

# How to run?

- `git clone https://github.com/prakashpandey/tinycoin`

- `cd tinycoin`

- `./start.sh`

By default the application will run on port `5000`

# Configuration

Open file `start.sh`. 
You can set the values of following environment variables according to your needs.

- `HOST="0.0.0.0"`

- `PORT=5000`

- `PEERS="192.168.1.11:5000,192.168.1.12:5000"`

# API'S

##### Create a transaction

- `Method = Post`
- `Url = 127.0.0.1:5000/transaction`
- Body ```
        {
            "from": "71238uqirbfh894-random-public-key-a-alkjdflakjfewn204ij",
            "to": "ppdpp-dvfgf-fredgdsdf-gdsfgsd-35vr433-ee2eass4d",
            "amount": 2
        }
    ```
- API response `Transaction submission successful` or `Transaction unsuccessful`

##### start mining

- `Method = Get`

- `Url = localhost:5000/mine`

- API response `Mined block in JSON format`

##### start mining

- `Method = Get`

- `Url = localhost:5000/blocks`

- API response `Blockchain in JSON format`

# Project Screenshot 

![Screenshot](media/screenshot-1.png)

# Resource
This learning project is created just for learning and based on open blog articles on internet.

