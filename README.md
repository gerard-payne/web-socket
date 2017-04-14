[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/gerard-payne/web-socket)

Polymer component to create and manage web socket connections.

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

It may also optional property causing the component to attempt to establish a socket when loaded.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
        auto
    ></web-socket>

and/or optional property causing the component to log events to the console.

    <web-socket
        url="ws://127.0.0.1:8080/socket"
        debug
    ></web-socket>

# Methods
    web-socket.open()
Open the socket

    web-socket.send(oMessage)
Send sMessage <Object> across an open socket

    web-socket.close()
Close the socket.
