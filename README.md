zaakpay-php-kit
===============

Zaakpay Integration Kit for PHP

This is a ReadMe for the Zaakpay PHP kit.


Zaakpay API is made up of 3 different APIs, which are described below.


TRANSACT API : This is the primary API used to perform a transaction.
It makes use of the following files.
test_merchant_input.html : This is the HTML file which takes input from user & posts data.

<b>posttozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the TRANSACT API.<br />

<b>response.php</b> : The TRANSACT API completes the transaction & redirects user to this file.<br /><br />


<b>STATUS CHECK API :</b> Merchants can use this API to check the status of a prior transaction.<br />

It makes use of the following files.<br />

<b><a href="test_status_check_input.html" style="color:#00D9FF; font:bold 15px/22px Arial, Helvetica, sans-serif;">test_status_check_input.html</a></b> : This is the HTML file which takes input from user & posts data.<br />

<b>poststatuschecktozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the STATUS CHECK API.<br />
<b>Note : </b> We provide a checksum in the response xml. Please use it to verify the validity of the response.<br /><br />


<b>STATUS UPDATE API :</b> Merchants can use this API to update the status of a prior transaction.<br />

It makes use of the following files.<br />

<b><a href="test_mtx_update_input.html" style="color:#00D9FF; font:bold 15px/22px Arial, Helvetica, sans-serif;">test_mtx_update_input.html </a></b>: This is the HTML file which takes input from user & posts data.<br />

<b>postmtxupdatetozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the STATUS UPDATE API.<br />
<b>Note : </b> We provide a checksum in the response xml. Please use it to verify the validity of the response.
