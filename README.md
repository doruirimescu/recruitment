# recruitment: developer assignment (LabVIEW)
Hi! Really nice to hear that you may be interested in joining our development team. We are a leading provider of RFID test & measuremnent solutions when it comes to RFID tag design AND mass production & personalization.

Our stack consists of:
- LabVIEW
- embedded C
- Node.js, Express
- AWS (API gateway, Lambda, DynamoDB, etc.)
- We work close to hardware and design our own test&measurement equipment and accessories.

Here is a very simple LabVIEW example on how to authenticate with Winston (that's what we call our little but continuously smarter and more helpful backend).

What we'd ask you to do is to take a look at the example and take it a bit further. The idea is a LabVIEW application that can query the list of known tag ICs ("chips"), show it to the user and - perhaps if you'd like - user could select a chip from the list and get more information on their screen about that particular chip. When it comes to GUI look and feel, error handling, etc., we let you show in code what is your opinion of good code.

We will then talk in person about the code, life, culture and working at Voyantic if we like your style and you liked the little assigment!

When done, please just make a pull request!

Here's an example on how you could call the Winston resource you need for chip list and chip information:
`curl -X GET https://gikr1vhulg.execute-api.eu-west-1.amazonaws.com/playground/v1/chips/tags -H 'X-API-Key: [guess what goes here]' -H 'Authorization: Bearer [got dʒɒt?]'`

For detailed chip information you need to combine manufacturer ID (e.g. 001) and tag ID (e.g.190) which will look like `001-190`. Same endpoint, just remember to tell it what you want: `...chips/tags/001-001` should work as an example.

Hope you like it!

Ah, yes, one more thing, if you do not have received an API key and licenseHash from us, please contact `recruiting@voyantic.com`
