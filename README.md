Creates and manages web socket connections.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
    ></web-socket>

It may include optional properties for attaching callbacks to lifecycle events.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
        on-open="subscribeSocket"
        on-message="showMessage"
        on-error="showError"
        on-close="endSocket"
    ></web-socket>

You can also include optional properties causing the component to attempt to establish a socket when loaded.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
        auto
    ></web-socket>

and/or optional properties causing the component to log events to the console.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
        debug
    ></web-socket>