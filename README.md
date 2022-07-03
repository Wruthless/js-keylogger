# JavaScript Keylogger

Nothing better than writing some malware, I always say!

The impetus was to experiment with `Promises` and `async` functionality in JavaScript. A single class exists that sets up a queu utilizing Promises, which pushes the keystrokes into an array. Currently, the keypresses report back to the console. Consider the following:

<pre>
async function handleKeys() {
    // Get a stream of keypress events and loop once for each one
    for await (const event of eventStream(document, "keypress")) {
        console.log(event.key); // report keystrokes
    }
}
</pre>

The above highlights where you want to change the functionality to do something more clever to gain access to the keystrokes data :-) As usual, this was created for educational purposes only.
