This is a fork of [cjslack/grok-debugger](https://github.com/cjslack/grok-debugger)

---

Access at:
[grok-debugger.shoellein.de](https://grok-debugger.shoellein.de)

This client-side application uses WebAssembly to emulate the logstash grok library in the browser. It is responsive, feature-rich, and can help you quickly debug your grok patterns. Although it works well in most cases, it is not an exact port of logstash grok, so be sure to test your patterns in your environment before deploying. 

**Features:**

- Real-time processing (see changes as you type)
- Autocomplete
- Match highlighting
- Syntax highlighting
- Multiline debugging
- 20+ pattern sets (AWS, Grok, firewalls, Java, etc.)
- Add more pattern sets with a URL
- Save and use your own custom patterns

**Limitations:**

- Does not support explicitly defined output types e.g. `%{NUMBER:status:int}`
- Does not support inline flag modifiers e.g. `(?i)opid=%{NOTSPACE:event_operation_id}` https://github.com/cjslack/grok-debugger/issues/6

**Run locally:**

Must have [node.js](https://nodejs.org/en) installed
```
git clone https://github.com/cjslack/grok-debugger.git
cd grok-debugger
npm install
npm start
```