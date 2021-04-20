Fraud Order Identification
=============================

We use extension 'Signifyd_Connect' to identify the order is fraud one or not. And we make some changs during integration to make it suit Toolots, here's the things need to pay attention to

#. Just orders paid with braintree credit card are allowed to send to signifyd

   .. image:: fraudIdentification/restrictionExceptBraintreeCrediCard.png

#. To make signifyd identify 'Will Call' order , we made some change followed by signifyd's guidance

   .. image:: fraudIdentification/pickupInStoreRequestChanges.png

#. Invoice generation should be triggered after that one order are approved by signifyd

   .. image:: fraudIdentification/autoInvoice.png