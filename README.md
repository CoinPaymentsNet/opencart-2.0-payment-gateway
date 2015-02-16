OpenCart 2.0 Payment Gateway plugin for CoinPayments.net
========================

To install:
1) Upload the contents of the upload folder into your OpenCart root folder.
2) Go to the Payment extensions area and click the Install button.
3) Edit the plugin settings with your CoinPayments Merchant ID and IPN Secret and set the status to Enabled.
4) Switch to the Order Status tab to set your order statuses. Good defaults are:
	a) Cancelled/Timed Out: Canceled
	b) Completed: Processing
	c) Pending: Pending

This version includes a fix for OpenCart's 3 digit currency limitation so you can use currencies with more than 3 digits like DOGE, NOBLE, and MINT. If you want to list items in those currencies directly use the currency codes DOG, NBL, and MNT respectively.
See the top of catalog/controller/payment/coinpayments.php for a full list of shortened codes.
You can still use the full 4 digit code for the "Symbol Right" setting so your users probably won't even notice the change.
