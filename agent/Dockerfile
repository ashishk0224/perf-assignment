FROM node:14

# Create app directory
WORKDIR /Users/ashishkumar/Downloads/assignment/pkg

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 9997

#Define conf_dir as variable
ENV conf_dir target
CMD node app.js ${conf_dir}
