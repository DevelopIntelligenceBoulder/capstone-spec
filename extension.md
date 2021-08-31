We underestimated the tech savviness of our customers, and it seems that very few of them, if any at all, want to order over the phone. Drats!

That’s ok though! This should just be a small addition considering how great my engineering team is. At least that’s what I told my boss… and I’m your boss, so that’s how it is.

Here’s what we need to add. We need customers to be able to authenticate against the application just like the CSRs, but with diminished capabilities. The customers should have views where they are able to see their account details, view the product catalog, and interactively add items from the product catalog into a cart. From the cart, the customers should be able to submit their order.

The customer’s order request should then be added to a queue hosted in the cloud. CSRs will be responsible for draining that queue of pending orders, either accepting or rejecting the order. This mini-ticketing system will also need a view. If accepted, the order will be added to the DB and the normal order processing flow should occur. If rejected, the order will be thrown away, and the customer will need to be informed. The customer should always be able to retrieve the latest status of their orders from their portal.

Not all of our customers are the most trustworthy, so I’m expecting you’ll take the appropriate measures to lock down the APIs we are exposing since they will now be processing potentially malicious input.
