<h1>Predefined Signals</h1>
The following pre-defined signals MUST be supported by both the client and the server implementing the Messaging API Specification:

<h2 id="message-accepted">Message Accepted</h2>
<b>Status:</b> 202<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#message-accepted<BR />
<b>Detail:</b> Sent when the message is properly validated. It may include a status monitor that can provide the user with an estimate of when the request will be fulfilled (see [RFC7231])<BR />

<h2 id="message-validation-failed">Validation Failed</h2>
<b>Status:</b> 400<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#message-validation-failed<BR />
<b>Detail:</b> Sent when the message fails the validation process<BR />

<h2 id="invalid-message-id">Invalid or Duplicate Message ID</h2>
<b>Status:</b> 400<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#invalid-message-id<BR />
<b>Detail:</b> Sent when the MessageId is not valid<BR />

<h2 id="invalid-message-signature">Invalid Message Signature</h2>
<b>Status:</b> 400<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#invalid-message-signature<BR />
<b>Detail:</b> Sent when the message signature cannot be verified<BR />

<h2 id="invalid-addressing">Invalid Addressing</h2>
<b>Status:</b> 400<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#invalid-addressing<BR />
<b>Detail:</b> Sent when the Original Sender or Final Recipient(s) cannot be resolved<BR />

<h2 id="invalid-format">Invalid Message Format</h2>
<b>Status:</b> 400<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md#invalid-format<BR />
<b>Detail:</b> Sent when the message format does not adhere to the specification<BR />

<h2 id="internal-server-error">Internal Server Error</h2>
<b>Status:</b> 500<BR />
<b>Type:</b> https://github.com/isa2-api4ips/rest-api-profile/blob/main/messaging-api-specification/signal.md/internal-server-error<BR />
<b>Detail:</b> The server encountered an unexpected condition that prevented it from fulfilling the request<BR />
