mkdir my-frontend-project
cd my-frontend-project

npm init -y

npm install react react-dom
npm install --save-dev webpack webpack-cli babel-loader @babel/core @babel/preset-env @babel/preset-react
const path = require('path');

module.exports = {
  entry: './src/index.js',
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'bundle.js',
  },
  module: {
    rules: [
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: 'babel-loader',
        },
      },
    ],
  },
  resolve: {
    extensions: ['.js', '.jsx'],
  },
  devServer: {
    contentBase: path.join(__dirname, 'dist'),
    compress: true,
    port: 9000,
  },
};

{
  "presets": ["@babel/preset-env", "@babel/preset-react"]
}


import React from 'react';
import ReactDOM from 'react-dom';

const App = () => <h1>Hello, world!</h1>;

ReactDOM.render(<App />, document.getElementById('root'));

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Frontend Project</title>
</head>
<body>
  <div id="root"></div>
  <script src="bundle.js"></script>
</body>
</html>

npm start

# Frontend Setup

## Prerequisites
- Node.js and npm
- Code editor (e.g., VS Code)

## Steps

1. **Set Up Your Development Environment**
   - Install Node.js and npm from Node.js website.
   - Install VS Code.

2. **Initialize Your Project**
   - Create a new directory and initialize npm.

3. **Install Dependencies**
   - Install React, Webpack, and Babel.

4. **Configure Webpack**
   - Create `webpack.config.js`.

5. **Configure Babel**
   - Create `.babelrc`.

6. **Create Source Files**
   - Create `src/index.js`.

7. **Set Up HTML Template**
   - Create `dist/index.html`.

8. **Update `package.json` Scripts**
   - Add start and build scripts.

9. **Run Your Project**
   - Start the development server and open `http://localhost:9000`.

const { CleanWebpackPlugin } = require('clean-webpack-plugin');
const HtmlWebpackPlugin = require('html-webpack-plugin');
const path = require('path');

module.exports = {
  entry: './src/index.js',
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'bundle.js',
  },
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', 'css-loader'],
      },
      {
        test: /\.html$/,
        use: ['html-loader'],
      },
      {
        test: /\.(png|jpe?g|gif|svg)$/i,
        loader: 'file-loader',
       Pay with Pi leading payment app
Use Pay with pi for the fastest, most secure online and in-store payments! Pay for movie tickets, food, coffee, fashion, gas, and many more in Pay with Pi.

Quick, easy, convenient and secure.

**Send / Receive Payments**

Pay in store or send money to friends. No need to carry cash or worry about loose change!

**Online Top-Ups and Utility Bill Payments**

Top-up your mobile phone, pay your utility and internet bills or settle your monthly insurance premiums bills through Pay with Pi.

**Add Money to your Pay with Pi Wallet**

Add money to your Pay with pi app via Pay&Go machines or transfer from multiple online banking apps cash-in at all Banks branches and agent world wide.

**Explore Nearby**

Explore places near you that accept payment through Pay with pi wallet. Cinemas, restaurants, coffee shops, supermarkets, and gas stations are all joining forces with Pay with Pi to make your life more connected and more mobile.

Don’t forget to look out for great deals exclusively for Pay with pi users! Start enjoying the amazing benefits of Pay with Pi. Download it now..

https://facebook.com/events/s/pay-with-pi/8422884491088457/

https://forms.gle/NBzpicuQ1SXQSH4e6

