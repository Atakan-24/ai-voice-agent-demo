<!-- Hands-on Fallstudie: die Empfangs-Demo auf der Webseite. Keine Interna, keine Schlüssel. -->
# The reception demo: a guided call you can try in the browser

A visitor picks a trade (heating and air, plumbing, roofing, solar), "calls", and talks or types to Alex. At the end a sample appointment card shows what was captured.

Try it: [teamgoldllc.de/voice-agent](https://teamgoldllc.de/voice-agent) (English) · [/voice-agent/de](https://teamgoldllc.de/voice-agent/de) (German)

## The idea

Most AI demos either cost money per visitor or sound like a robot. I wanted one that is **free to run, sounds human, and never goes off-script**.

So the demo is a guided conversation with fixed answer variants, not a live language model. Every sentence Alex can say was recorded once in advance. The page only decides which recording to play next.

## How it plays

1. Pick a business. The greeting and the questions change with the trade.
2. Alex asks what the call is about, then one trade-specific question (repair or new installation).
3. Name, then contact details. A spoken email like "name at example dot com" is understood.
4. Alex names three sample time slots, you pick one, Alex repeats it and asks for confirmation.
5. A test appointment appears on screen. Nothing is booked, sent or stored.

Details that made it feel real:

- **A call screen**, not a chat box: connection status, timer, animated receiver, hang-up button.
- **Speak or type.** Speaking starts by itself after the greeting and sends when you pause. Mute and hang-up are always on top.
- **Honest limits.** "Tomorrow at 8" gets a polite "that is not one of the sample times" plus the alternatives, never a wrong confirmation. A price question gets an answer without losing the thread.
- **Your voice stays on your device.** Speech recognition runs locally in the browser, so no audio is uploaded and there is no per-visitor cost.

## What I learned

- **Fixed recordings beat a live model for a public demo.** It cannot say anything embarrassing, it costs nothing per visitor, and it answers instantly.
- **Pause detection is the product.** Too short and it cuts you off, too long and it feels dead. The demo waits for about 1.8 seconds of silence before it answers.
- **Say the abbreviations out loud properly.** "HVAC" is spoken as the full words, otherwise it sounds like a machine.
- **Say what it is.** The page states plainly that it is a guided demo with an AI voice. Nobody feels tricked, and it reads as more professional.
- **Still open:** a long test with real human speech from several people. Small speech models make recognition mistakes, which is why typing stays available.

Back to the [overview](../README.md).
