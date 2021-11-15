# TO USE: skygvinn/welcome-express

# To make this files:
# docker run --rm -it -v $(pwd)/:/usr/src/app -p 3000:3000 node:15 bash
# cd usr/src/app
# npm init
# npm install express --save

# index.js
# const express = require('express')
# const app = express()
# const port = 3000

# app.get('/', (req,res) => {
#   res.send('<h1>Welcome!</h1>')
# })

# app.listen(port, ()=> {
#   console.log('listening on port' + port)
# })

FROM node:15

LABEL name="Node.js 15 + NPM + Express" \
      version="1.0" \
      author="Marcelo Toledo, aka Skygvinn"

WORKDIR /usr/src/app

# COPY . .

EXPOSE 3000

CMD [ "node", "index.js" ]
