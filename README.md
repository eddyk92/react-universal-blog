#React Universal Blog
#####[View a demo here](http://tonyspiro.com:5000/)
#####[Go to Cosmic JS to set up a bucket for your blog content](https://cosmicjs.com/)

#####About
The React Universal Blog is a portfolio blog app that renders html on the server side to make all pages visible to search engines. Then after initial load from the server, the app is converted to a single page application to allow for fast navigation between pages.  

I tried to keep the organization as simple as possible.  There are no client, server or shared component folders.  All components are shared and the only difference between client and server are the entry points (app-client.js, app-server.js, app-deploy.js). 

It uses the following:
<br>
1. [React](http://facebook.github.io/react/) for UI views<br>
2. [Express](http://expressjs.com/) for server side rendering<br>
3. [React Router](https://github.com/rackt/react-router) for routing<br>
4. [Flux](https://facebook.github.io/flux/) for data flow<br>
5. [Cosmic JS](https://cosmicjs.com) for content management
#####Install
```
git clone https://github.com/tonyspiro/react-universal-blog
cd react-universal-blog
npm install
```
#####Run webpack dev
```
npm run dev
```
Go to [http://localhost:8080/webpack-dev-server](http://localhost:8080/webpack-dev-server)
#####Run production
```
npm run prod
```
Go to [http://localhost:3000](http://localhost:3000)
#####Configure
After setting up your blog on [Cosmic JS](https://cosmicjs.com), edit the ```config.js``` file and edit the slug to point to the slug of your bucket:
```javascript
// config.js
export default {
  bucket: {
    slug: 'react-universal-blog',
    read_key: '',
    write_key: ''
  }
}
```
