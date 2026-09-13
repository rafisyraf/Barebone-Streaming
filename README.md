# Barebone Streaming
A simple, cheap, yet practical setup for streaming. Ensuring portability for a hassle-free setup.

<img width="300" height="500" alt="Documentation" src="https://github.com/user-attachments/assets/70e1924e-5e5d-4b24-83e8-d5d29d5e603b" /> <img width="270" height="585" alt="Live View" src="https://github.com/user-attachments/assets/26b106f6-8d21-440a-b305-e3ea0a1cdc4f" />


## Background
This setup was needed by a client within a special request. Where i need to come up with a portable streaming solution with the company's limmited streaming gear without needing to buy anything new. Unlike many complex rigs, this setup has been fully tested, assembled, deployed, and tested by the client successfully, bringing a stable 2k views on tiktok. Which is proven to deliver real world performance while keeping the costs minimum.

## The Gear
* **ROG Ally:** Shocking, Used as a computer to stream
* **JSAUX USB hub:** Crucial to bridge all the device with stability
* **Portable Monitor (Optional):** To monitor the live feed
* **Sony a5100 with 35mm lens:** Used to capture the audience and the host
* **USB capture card:** Connects the camera feed to the ROG Ally
* **Hollyland mic:** Used for an audio capture with excellent battery life and noise cancelling

## The Software
* **Tiktok LIVE studio:** As the main application to stream requested by the client

## Wiring Diagram
```mermaid
graph TD
    %% Main Host Computer
    ROG[ROG Ally <br/><i>Streaming PC</i>] 

    %% Core Bridge
    Hub[JSAUX USB Hub]

    %% Peripherals & Inputs
    Monitor[Portable Monitor <br/><i>Optional Feed Monitor</i>]
    CapCard[USB Capture Card]
    Mic[Hollyland Mic <br/><i>Audio Capture</i>]
    
    %% Video Source
    Cam[Sony a5100 Camera <br/><i>w/ 35mm Lens</i>]

    %% Connections
    ROG --- Hub
    Hub --> Monitor
    Hub --> CapCard
    Hub --> Mic
    Cam --> CapCard

    %% Styling
    style ROG fill:#f9f,stroke:#333,stroke-width:2px
    style Hub fill:#bbf,stroke:#333,stroke-width:2px
    style Monitor fill:#eee,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
    style Cam fill:#f96,stroke:#333,stroke-width:1px

```
