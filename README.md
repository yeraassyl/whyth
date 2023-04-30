# AI Teaching Assistant app

Use at https://whyth.app or deploy your own. 

## Development setup

First of all, update subomdules:
`git submodule update --remote --recursive`

### Backend

>Note: You need **redis-server** running on your machine

1. Create `.env` 
2. Set `API_KEY` environrment variable
2. Run `main.go`

Refer to `.env.example` and `config.go` for the complete list of env variables.
  
### Frontend

1. `npm install`
2. Uncomment `setupProxy.js` (for CORS issues)
3. `npm start`