zaakpay-php-kit
===============

Zaakpay Integration Kit for PHP

This is a ReadMe for the Zaakpay PHP kit.


Zaakpay API is made up of 3 different APIs, which are described below.


TRANSACT API : This is the primary API used to perform a transaction.
It makes use of the following files.
test_merchant_input.html : This is the HTML file which takes input from user & posts data.

<b>posttozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the TRANSACT API.

<b>response.php</b> : The TRANSACT API completes the transaction & redirects user to this file.


<b>STATUS CHECK API :</b> Merchants can use this API to check the status of a prior transaction.

It makes use of the following files.

<b>test_status_check_input.html</b> : This is the HTML file which takes input from user & posts data.

<b>poststatuschecktozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the STATUS CHECK API.
<b>Note : </b> We provide a checksum in the response xml. Please use it to verify the validity of the response.


<b>STATUS UPDATE API :</b> Merchants can use this API to update the status of a prior transaction.

It makes use of the following files.

<b>test_mtx_update_input.html </b>: This is the HTML file which takes input from user & posts data.

<b>postmtxupdatetozaakpay.php</b> : This is the file which accepts input, sanitizes it & posts it to the STATUS UPDATE API.
<b>Note : </b> We provide a checksum in the response xml. Please use it to verify the validity of the response.
