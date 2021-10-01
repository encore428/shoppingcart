
 

# Take Home Homework (Day 3)

<a href="./Day 3 homework.pdf">Page 95 and 96</a> of Day 3 presentation slide sets out the framework for the Homework as below:

Create a new application using Create React App:
- When it first load, shows the login page: refers to https://transition-to-react-playground.vercel.app/login for how it look like
- When user login successfully, shows the marketplace page.https://transition-to-react-playground.vercel.app/marketplace-mock
- When there is no items, show empty message like this page: https://transition-to-react-playground.vercel.app/marketplace-empty

Notes:
- To add item to cart, use https://\<your-service>.herokuapp.com/docs/#/marketplace/addCartItem
- To get items in cart, use https://\<your-service>.herokuapp.com/docs/#/marketplace/listCartItems
- To remove item from cart, use https://\<your-service>.herokuapp.com/docs/#/marketplace/removeCartItem

You should use React styleguidist to documents your presentation components.

Deploy the site and the styleguidist site to Netlify and submit the URLs together with the link to your repository.
 
# Deployment

The app contined from the app of Homework Day 1 and Day 2, and added on the functinality required for Homework Day 3.  The app has been deployed to Netlify as below:

https://confident-golick-a02a49.netlify.app 

For the shoppingCart functionality required for Homework Day 3, it is accessible under the navigation item 'shopping' on top right.
 
The styleguidist site has been deployed to Netlify as below:

https://trusting-austin-c3dcde.netlify.app/ 
 
# Special Notes

During the app deployment, there was one additional task required just because of Netlify:

CI=False, refer to this [article](https://stackoverflow.com/questions/62415804/how-to-prevent-netlify-from-treating-warnings-as-errors-because-process-env-ci).

1. On Netlify, go to Deploys -> [Deployment Settings](https://app.netlify.com/sites/confident-golick-a02a49/settings/deploys).
1. Schroll down to see Environment tab.
1. Click Environment Variables -> Edit Variables
1. Key: CI Value: False
1. Redeploy with clearing cache.
 
![CI=False setting on Netlify](./CIFalse.png)
